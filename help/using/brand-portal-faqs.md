---
title: 'Perguntas frequentes '
seo-title: null
description: Saiba mais sobre as perguntas mais frequentes na Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 67a745fed6a13cfdb30e26062eecc3c8d1775e36
workflow-type: tm+mt
source-wordcount: '1468'
ht-degree: 1%

---

# Perguntas frequentes  {#frequently-asked-questions}

As Perguntas frequentes do Brand Portal se concentram nas consultas e problemas que os usuários finais podem ter ao trabalhar com a versão mais recente do AEM Assets Brand Portal 6.4.6 ou versões anteriores.


## Perguntas frequentes sobre o Brand Portal 6.4.6  {#faqs-bp646}

**Ques. O endpoint OAuth existente (`https://legacy-oauth.cloud.adobe.io/login`) herdado não está funcionando. Qual poderia ser o motivo possível?**

**Ans.** A configuração herdada de OAuth está obsoleta. Você deve atualizar as instâncias de autor do AEM Assets para o service pack mais recente e configurá-las por meio do Console do desenvolvedor do Adobe. Consulte [Configurar o AEM Assets com Brand Portal](configure-aem-assets-with-brand-portal.md) para obter detalhes. No entanto, para que a configuração Legacy OAuth funcione até a atualização, atualize o endpoint Legacy OAuth para `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Não consigo publicar os ativos da pasta de contribuição do Brand Portal para o AEM Assets após atualizar para o Console do desenvolvedor do Adobe. Minha instância do autor está no AEM 6.5.4. Qual pode ser o motivo possível?**

**Ans.** Sim, há um problema conhecido ao publicar os ativos da pasta de contribuição no AEM Assets no AEM 6.5.4 por meio do Console do desenvolvedor do Adobe.

O problema é corrigido no AEM 6.5.5. Você pode atualizar sua instância do AEM Assets para o service pack mais recente AEM 6.5.5 e [atualizar suas configurações](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) no Console do Desenvolvedor do Adobe.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. Não vejo o conteúdo da pasta de contribuição publicado no Brand Portal no AEM Assets. Qual poderia ser o motivo possível?**

**Ans.** Entre em contato com o administrador do AEM Assets para verificar as configurações e garantir que o locatário do Brand Portal esteja configurado com apenas uma instância do autor do AEM Assets.

Esse problema pode ocorrer quando você configurou um locatário do Brand Portal em várias instâncias do autor do AEM Assets. Por exemplo, o administrador configura o mesmo locatário do Brand Portal na instância do autor do AEM Assets do ambiente de preparo e produção. Nesse caso, a publicação de ativos é acionada no Brand Portal, mas a instância do autor do AEM Assets não pôde importar o cuz do ativo, pois o agente de replicação não recebe o token de solicitação.


**Ques. Não consigo publicar ativos do AEM Assets para o Brand Portal. O log de replicação declara que a conexão atingiu o tempo limite. Existe uma correção rápida?**

**Ans.** Geralmente, a publicação falha com um erro de tempo limite se houver várias solicitações pendentes na fila de replicação. Para resolver esse problema, verifique se os agentes de replicação estão configurados para evitar o tempo limite.

Execute as seguintes etapas para configurar o agente de replicação:

1. Faça logon na instância do autor do AEM Assets.
1. No painel **Ferramentas**, navegue até **[!UICONTROL Implantação]** > **[!UICONTROL Replicação]**.
1. Na página Replicação , clique em **[!UICONTROL Agentes no autor]**. Você pode ver os quatro agentes de replicação do seu locatário do Brand Portal.
1. Clique no URL do agente de replicação para abrir os detalhes do agente.
1. Clique em **[!UICONTROL Editar]** para modificar as configurações do agente de replicação.
1. Em Configurações do agente, clique na guia **[!UICONTROL Extended]**.
1. Marque a caixa de seleção **[!UICONTROL Fechar conexão]**.
1. Repita as etapas 4 a 7 para configurar todos os quatro agentes de replicação.
1. Reinicie o servidor e verifique a conexão.


## Perguntas frequentes sobre o Brand Portal 6.4.5  {#faqs-bp645}

**Ques. Qual é a maior alteração na versão 6.4.5 do Brand Portal?**

**Ans.** O AEM Assets Brand Portal 6.4.5 é uma versão de recurso que permite que os usuários do Brand Portal façam upload de conteúdo dentro da instância do Brand Portal e publiquem a pasta Contribuição de volta no AEM Assets sem precisar de direitos de administrador.
Para obter mais informações, consulte [Origem de ativos no Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Perderei o acesso a quaisquer ativos, recursos ou configurações existentes que criei?**

**Ans.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não serão afetados e seu conteúdo permanecerá intacto.



**Ques. Quando estou migrando para a nova versão do Brand Portal?**

**Ans.** O Brand Portal 6.4.5 foi lançado para produção em outubro de 2019. E a próxima versão do Brand Portal deverá ser lançada no terceiro trimestre de 2020.
Para atualizações e alterações de versão, é recomendável rastrear as [Notas de versão](brand-portal-release-notes.md) e [Novidades no Brand Portal](whats-new.md).



**Ques. Meus usuários serão afetados?**

**Ans.** A versão do Brand Portal 6.4.5 é exclusivamente no Brand Portal, portanto, não há impacto para os usuários finais.



**Ques. Existe alguma ação necessária da minha parte como usuário do Brand Portal?**

**Ans.** A versão 6.4.5 do Brand Portal vem com um novo recurso chamado origem dos ativos. AEM administrador deve configurar o recurso de origem dos ativos no AEM Assets para habilitar o recurso para os usuários do Brand Portal. Para obter mais informações, consulte [Ativar origem de ativos](brand-portal-asset-sourcing.md).



**Ques. Quem pode criar uma pasta de Contribuição?**

**Ans.** Qualquer usuário AEM que tenha permissões para criar uma nova pasta no AEM Assets pode criar uma pasta  **** Contribuição. Para criar uma pasta **Contribuição**, crie uma nova pasta do tipo **Contribuição de ativos**.
Essa pasta é compartilhada com os usuários ativos da Brand Portal para contribuição.



**Ques. O que uma pasta Contribuição contém?**

**Ans.** **** A pasta Contribuição contém duas subpastas  **** NEWe  **SHARED**. Inicialmente, a NOVA pasta está em branco e a pasta COMPARTILHADA contém o conteúdo de referência (ativos reutilizáveis) para os usuários do Brand Portal.
Os usuários do Brand Portal acessam a pasta **Contribuição** e fazem upload do conteúdo na pasta **NEW**.



**Ques.  Posso modificar o nome de uma pasta de Contribuição existente?**

**Ans.** **Não**, você não pode modificar o nome de uma pasta  **** Contribuição existente.



**Ques. Quais são os requisitos de ativos com contribuição de r.t?**

**Ans.** O  **** Briefdocument anexado à pasta  **** Contribuição e o conteúdo de referência (ativos reutilizáveis) carregados na pasta  **** SHARED ajuda o usuário da Brand Portal a entender a necessidade de contribuição e expectativas como um colaborador, e é chamado coletivamente de requisitos de ativos.



**Ques. Posso fazer upload de ativos para qualquer pasta permitida?**

**Ans.** Nem todas as pastas permitidas. Um usuário do Brand Portal pode fazer upload de conteúdo somente para a pasta **Contribuição** que é compartilhada pelo administrador do AEM ou Brand Portal.



**Ques. Como obtenho acesso a uma pasta de Contribuição?**

**Ans.** Você pode acessar uma pasta  **** Contribuição somente se ela tiver sido compartilhada com você. Você receberá uma notificação por email/pulso sempre que uma pasta de Contribuição for compartilhada com você. Você pode acessar a pasta Contribuição por meio do link compartilhado no email ou fazer logon na sua instância do Brand Portal e navegar até o ícone de sino para obter notificações sobre como acessar a pasta Contribuição.

>[!NOTE]
>
>Se você não for um usuário existente do Brand Portal, solicite ao administrador do AEM que crie seu usuário no Admin Console AEM e adicione seu perfil ao arquivo de configuração do usuário na lista de usuários do Brand Portal.

**Ques. Qual é o formato do arquivo CSV para importação do usuário?**

**Ans.** O formato é igual ao que é suportado pelo Admin Console para a importação de usuários em massa. Email, nome e sobrenome são obrigatórios.



**Ques. O que preenche a lista de usuários (contribuidores do Brand Portal) no menu suspenso do usuário de Contribuição de ativos?**

**Ans.** Os usuários na lista suspensa são preenchidos a partir do arquivo de configuração de usuário (.csv) do Brand Portal carregado no AEM.



**Ques. Onde posso ver o status dos trabalhos de importação e publicação?**

**Ans.** No AEM, você pode ver o status de uma importação na página  **** asyncjob. No Brand Portal, você pode ver o status de um trabalho de publicação em **[!UICONTROL Ferramentas > Status da contribuição de ativos]**.



**Ques. Qual é a frequência de um trabalho de importação que é executado periodicamente em AEM?**

**Ans.** Em AEM, a sondagem é feita a cada 5 minutos.



**Ques. Existe algum limite no número de vezes que uma pasta pode ser publicada do Brand Portal para o AEM Assets?**

**Ans.** Não, todos os ativos na  **** NEWfolder são publicados na AEM Assets, independentemente de terem sido publicados anteriormente. Toda vez que uma pasta **Contribution** é publicada do Brand Portal para o AEM Assets, ela substitui o conteúdo da pasta **NEW**.



**Ques. Como fazer upload de novos ativos em uma pasta de Contribuição?**

**Ans.** Consulte a documentação detalhada para  [Fazer upload de ativos na pasta Contribuição](brand-portal-publish-contribution-folder-to-brand-portal.md) .



**Ques. Não vejo miniaturas/visualizações nos ativos carregados na NOVA pasta por um usuário do Brand Portal?**

**Ans.** Ele foi projetado, pois não há workflow sendo executado no Brand Portal.



**Ques. O que acontece se uma pasta é publicada do AEM Assets para o Brand Portal que está em fluxo?**

**Ans.** Em AEM, os logs são mantidos por cada vez que uma pasta é publicada no Brand Portal. No momento da publicação, todos os ativos que não são publicados no Brand Portal são colocados em uma fila de replicação. Qualquer ativo adicionado à pasta após o trabalho de publicação ser acionado não é publicado na Brand Portal. Quando o usuário do AEM publica a pasta novamente, somente os ativos que não foram publicados anteriormente (existentes na fila de replicação) são publicados no Brand Portal.
Isso vale para qualquer pasta publicada do AEM Assets para a Brand Portal e da pasta COMPARTILHADA em uma pasta Contribuição.

**Ques. Com quem eu faço contato?**

**Ans.** Entre em contato com o Gerente de conta do Adobe ou com o Suporte ao cliente.

>[!NOTE]
>
>A programação de versões é provisória e está sujeita a alterações. Entre em contato com o Gerente de conta do Adobe ou com o Suporte ao cliente para obter o cronograma atualizado de lançamento.


## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente do e precisar de acesso, entre em contato com o gerente de conta do Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)
-->
