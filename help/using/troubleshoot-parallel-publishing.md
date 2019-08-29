---
title: Solução de problemas de publicação paralela no Brand Portal
seo-title: Solução de problemas de publicação paralela no Brand Portal
description: Solução de problemas de publicação paralela.
seo-description: Solução de problemas de publicação paralela.
uuid: 51 e 45 cca -8 c 96-4 c 69-84 ef -2 ef 34 f 3 bcde 2
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
topic-tags: brand-portal
discoiquuid: a 4801024-b 509-4 c 51-afd 8-e 337417 e 658 b
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Solução de problemas de publicação paralela no Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

[!DNL Brand Portal] suporta a integração com [!DNL AEM Assets] os ativos de marca aprovados perfeitamente assimilados (ou publicados) a partir da instância do autor de ativos AEM. Depois [de integrado](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), [!DNL AEM] o Autor usa um agente de replicação para replicar os ativos selecionados para [!DNL Brand Portal] o serviço em nuvem para uso aprovado pelos [!DNL Brand Portal] usuários. Vários agentes de replicação são usados [!DNL AEM 6.2 SP1-CFP5]e [!DNL AEM CFP 6.3.0.2]em etapas para permitir a publicação paralela de alta velocidade.

>[!NOTE]
>
>A Adobe recomenda atualizar para [!DNL AEM 6.4.1.0] garantir [!DNL AEM Assets Brand Portal] que seja integrado com êxito aos ativos AEM. Uma limitação em [!DNL AEM 6.4] apresenta um erro ao configurar a integração com o Brand Portal e falha na replicação.

Ao configurar o serviço de nuvem para o portal de marca em [!UICONTROL /etc/cloudservice], todos os usuários e token necessários são gerados automaticamente e salvos no repositório. A configuração de serviço da nuvem é criada, os usuários do serviço necessários para replicação e replicação para replicação de conteúdo também são criados. Isso cria quatro agentes de replicação. Assim, ao publicar vários ativos [!DNL AEM] em, [!DNL Brand Portal]eles são colocados em fila e distribuídos entre esses agentes de replicação por meio de Redondos.

No entanto, a publicação pode falhar intermitentemente devido a trabalhos de sling grandes, aumento da rede e do disco [!UICONTROL I/O] por [!DNL AEM] instância do Autor ou lentidão do desempenho da [!DNL AEM] instância do Autor. Portanto, é recomendável testar a conexão com os agentes de replicação antes de iniciar a publicação.

![](assets/test-connection.png)

## Solução de problemas de falhas na primeira publicação: Validação da configuração de publicação {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Para validar as configurações de publicação:

1. Verificar os registros de erro
2. Verificar se o agente de replicação foi criado
3. Conexão de teste

**Ao criar o serviço em nuvem**

Verificar logs de cauda. Verifique se o agente de replicação foi criado ou não. Se a criação do agente de replicação falhar, edite o serviço de nuvem fazendo pequenas alterações no serviço em nuvem. Valide e verifique novamente se o agente de replicação foi criado ou não. Caso contrário, edite o serviço novamente.

Se, durante a edição repetida, o serviço de nuvem não estiver configurado corretamente, relate um ticket de daycare.

**Testar conexão com agentes de replicação**

Exibir log, se erros forem encontrados no registro de replicação:

1. Entre em contato com o suporte da Adobe.

2. Tente [limpar](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) e criar configurações de publicação novamente.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Limpeza das configurações de publicação existentes do Brand Portal {#clean-up-existing-config}

A maioria das vezes em que a publicação não está funcionando, o motivo pode ser que o usuário que está publicando (mac-&lt; tenantid &gt;-replication) não tenha a chave privada mais recente e, portanto, publique com "401 não autorizado", e nenhum outro erro será relatado nos logs do agente de replicação. Talvez você queira evitar solucionar problemas e criar uma nova configuração. Para que a nova configuração funcione corretamente, você deve limpar o seguinte da configuração do autor de AEM:

1. ir para [!UICONTROL localhost: 4502/crx/de] (considera que você está executando a instância do autor no [!UICONTROL host localhost: 4502]):\
   i delete [!UICONTROL /etc/replication/agents.author/mp_replication &amp; # 42];\
   ii delete [!UICONTROL /etc/cloudservices/mediaportal/ &lt; config_ name &amp; gt];

2. ir para [!UICONTROL localhost: 4502/usuário]:\
   eu pesquisar pelo usuário [!UICONTROL mac-&lt; tenantid &gt;-replication]\
   ii excluir esse usuário

Agora, o sistema fica limpo. Agora, você pode tentar criar uma nova configuração de nudservice e ainda usar [!DNL JWT] o aplicativo existente em [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). Não há necessidade de criar um novo aplicativo, e apenas a chave pública precisa ser atualizada da configuração recém-criada da nuvem.

## Problema de visibilidade do locatário JWT do aplicativo JWT {#developer-connection-jwt-application-tenant-visibility-issue}

Se em [!UICONTROL https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), todas as organizações (localidades) para as quais os usuários atuais detêm o administrador do sistema serão listadas. Se você não encontrar o nome da organização aqui ou não puder criar um aplicativo para um inquilino necessário aqui, verifique se você tem direitos suficientes (administrador do sistema) para fazer isso.

Há um problema conhecido nessa interface de usuário que, para qualquer locatário somente os primeiros 10 aplicativos estão visíveis. Ao criar o aplicativo, fique na página e marque o URL. Você não precisa ir para a página de listagem do aplicativo e encontrar o aplicativo criado. Você pode atingir este URL marcado diretamente e atualizar/excluir o aplicativo sempre que necessário.

O [!DNL JWT] aplicativo pode não ser listado adequadamente. Portanto, é recomendável observar/marcar o URL ao criar o aplicativo JWT.

## A configuração para a configuração parar de funcionar {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Se um agente de replicação (que estava publicando no brand portal apenas bem) parar de processar trabalhos de publicação, verifique os logs de replicação. [!DNL AEM] tiver uma tentativa automática de tentar incorporado, de modo que se uma publicação de ativo específica falhar, ela será refeita automaticamente. Se houver algum problema intermitente, como erro de rede, ele poderá ser bem-sucedido durante a nova tentativa.

Mas se houver falhas de publicação contínuas e a fila estiver bloqueada. em seguida, verifique "test connection" e tente resolver os erros que estão sendo relatados.

Com base nos erros, você deve registrar um ticket de suporte para que a equipe [!DNL Brand Portal] de engenharia possa ajudar a resolver problemas.
