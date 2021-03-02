---
title: Perguntas frequentes
seo-title: null
description: Obtenha informações sobre as perguntas frequentes no Portal de marcas do Adobe Experience Manager Assets.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4983e2e160b5cfb213e249f731e1858fab2cf972
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 1%

---


# Perguntas frequentes {#frequently-asked-questions}

As perguntas frequentes do Brand Portal se concentram nas consultas e problemas que os usuários finais podem encontrar ao trabalhar com a versão mais recente do AEM Assets Brand Portal 6.4.6 ou versões anteriores.


## Perguntas frequentes do Brand Portal 6.4.6 {#faqs-bp646}

**Ques. O endpoint OAuth existente (`https://legacy-oauth.cloud.adobe.io/login`) herdado não está funcionando. Qual poderia ser o motivo possível?**

**Ans.** A configuração herdada de OAuth está obsoleta. Você deve atualizar as instâncias de autor do AEM Assets para o service pack mais recente e configurá-las por meio do Console do desenvolvedor. Consulte [Configurar o AEM Assets com o Brand Portal](configure-aem-assets-with-brand-portal.md) para obter detalhes. No entanto, para que a configuração Legacy OAuth funcione até a atualização, atualize o endpoint Legacy OAuth para `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Não consigo publicar os ativos da pasta de contribuição do Brand Portal para o AEM Assets após atualizar para o Console do desenvolvedor. Minha instância do autor está no AEM 6.5.4. Qual pode ser o motivo possível?**

**Ans.** Sim, há um problema conhecido ao publicar os ativos da pasta de contribuição no AEM Assets no AEM 6.5.4 por meio do Console do desenvolvedor.

O problema é corrigido no AEM 6.5.5. Você pode atualizar a instância do AEM Assets para o service pack mais recente do AEM 6.5.5 e [atualizar suas configurações](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) no Console do desenvolvedor.

Para uma correção imediata no AEM 6.5.4, é recomendável [baixar o hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalar na instância do autor do AEM.

**Ques. Não vejo o conteúdo da pasta de contribuição publicado no Brand Portal no AEM Assets. Qual poderia ser o motivo possível?**

**Ans.** Entre em contato com o administrador do AEM Assets para verificar as configurações e garantir que o locatário do Brand Portal esteja configurado com apenas uma instância do autor do AEM Assets.

Esse problema pode ocorrer quando você configurou um locatário do Brand Portal em várias instâncias de autor do AEM Assets. Por exemplo, o administrador configura o mesmo locatário do Brand Portal na instância de autor do AEM Assets do ambiente de preparo e produção. Nesse caso, a publicação de ativos é acionada no Brand Portal, mas a instância do autor do AEM Assets não pôde importar o cuz do ativo que o agente de replicação não recebe o token de solicitação.


**Ques. Não consigo publicar ativos do AEM Assets no Brand Portal. O log de replicação declara que a conexão atingiu o tempo limite. Existe uma correção rápida?**

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


## Perguntas frequentes do Brand Portal 6.4.5 {#faqs-bp645}

**Ques. Qual é a principal mudança na versão 6.4.5 do Brand Portal?**

**Ans.** O AEM Assets Brand Portal 6.4.5 é uma versão de recurso que permite que os usuários do Brand Portal façam upload de conteúdo da instância do Brand Portal e publiquem a pasta Contribuição de volta nos AEM Assets sem precisar de direitos de administrador.
Para obter mais informações, consulte [Origem de ativos no Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Perderei o acesso a quaisquer ativos, recursos ou configurações existentes que criei?**

**Ans.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não serão afetados e seu conteúdo permanecerá intacto.



**Ques. Quando estou migrando para a nova versão do Brand Portal?**

**Ans.** O Brand Portal 6.4.5 foi lançado para produção em outubro de 2019. E a próxima versão do Brand Portal deverá ser lançada no terceiro trimestre de 2020.
Para atualizações e alterações de versão, é recomendável rastrear as [Notas de versão](brand-portal-release-notes.md) e [Novidades no Brand Portal](whats-new.md).



**Ques. Meus usuários serão afetados?**

**Ans.** A versão 6.4.5 do Brand Portal está exclusivamente no Brand Portal, portanto, não há impacto para os usuários finais.



**Ques. Há alguma ação necessária da minha parte como usuário do Brand Portal?**

**Ans.** A versão 6.4.5 do Brand Portal vem com um novo recurso chamado origem dos ativos. O administrador do AEM deve configurar o recurso de origem dos ativos no AEM Assets para habilitar o recurso para os usuários do Brand Portal. Para obter mais informações, consulte [Ativar origem de ativos](brand-portal-asset-sourcing.md).



**Ques. Quem pode criar uma pasta de Contribuição?**

**Ans.** Qualquer usuário do AEM que tenha permissões para criar uma nova pasta no AEM Assets pode criar uma pasta  **** Contribuição. Para criar uma pasta **Contribuição**, crie uma nova pasta do tipo **Contribuição de ativos**.
Essa pasta é compartilhada com os usuários ativos do Brand Portal para contribuição.



**Ques. O que uma pasta Contribuição contém?**

**Ans.** **** A pasta Contribuição contém duas subpastas  **** NEWe  **SHARED**. Inicialmente, a NOVA pasta está em branco e a pasta COMPARTILHADA contém o conteúdo de referência (ativos reutilizáveis) para os usuários do Brand Portal.
Os usuários do Brand Portal acessam a pasta **Contribuição** e fazem upload de conteúdo na pasta **NEW**.



**Ques.  Posso modificar o nome de uma pasta de Contribuição existente?**

**Ans.** **Não**, você não pode modificar o nome de uma pasta  **** Contribuição existente.



**Ques. Quais são os requisitos de ativos com contribuição de r.t?**

**Ans.** O  **** Briefdocument anexado à pasta  **** Contribuição e o conteúdo de referência (ativos reutilizáveis) carregados na pasta  **** SHARED ajuda o usuário do Brand Portal a entender a necessidade de contribuição e expectativas como um colaborador, e é chamado coletivamente de requisitos de ativos.



**Ques. Posso fazer upload de ativos para qualquer pasta permitida?**

**Ans.** Nem todas as pastas permitidas. Um usuário do Brand Portal pode fazer upload de conteúdo somente para a pasta **Contribuição** que é compartilhada pelo administrador do AEM ou do Brand Portal.



**Ques. Como obtenho acesso a uma pasta de Contribuição?**

**Ans.** Você pode acessar uma pasta  **** Contribuição somente se ela tiver sido compartilhada com você. Você receberá uma notificação por email/pulso sempre que uma pasta de Contribuição for compartilhada com você. Você pode acessar a pasta Contribuição por meio do link compartilhado no email ou fazer logon na instância do Brand Portal e navegar até o ícone de sino para obter notificações para acessar a pasta Contribuição.

>[!NOTE]
>
>Se você não for um usuário existente do Brand Portal, solicite ao administrador do AEM que crie seu usuário no Admin Console do AEM e adicione seu perfil ao arquivo de configuração do usuário na lista de usuários do Brand Portal.

**Ques. Qual é o formato do arquivo CSV para importação do usuário?**

**Ans.** O formato é igual ao compatível com o Admin Console para importação de usuários em massa. Email, nome e sobrenome são obrigatórios.



**Ques. O que preenche a lista de usuários (colaboradores do Brand Portal) no menu suspenso do usuário de Contribuição de ativos?**

**Ans.** Os usuários na lista suspensa são preenchidos a partir do arquivo de configuração de usuário (.csv) do Brand Portal carregado no AEM.



**Ques. Onde posso ver o status dos trabalhos de importação e publicação?**

**Ans.** No AEM, você pode ver o status de uma importação na página  **** assíncrono. No Brand Portal, você pode ver o status de um trabalho de publicação em **[!UICONTROL Ferramentas > Status de contribuição de ativos]**.



**Ques. Qual é a frequência de um trabalho de importação que é executado periodicamente no AEM?**

**Ans.** No AEM, a pesquisa é executada a cada 5 minutos.



**Ques. Existe algum limite no número de vezes que uma pasta pode ser publicada do Brand Portal para o AEM Assets?**

**Ans.** Não, todos os ativos na pasta  **** NEWsão publicados no AEM Assets independentemente do fato de terem sido publicados anteriormente. Sempre que uma pasta **Contribuição** é publicada no Brand Portal para o AEM Assets, ela substitui o conteúdo da pasta **NEW**.



**Ques. Como fazer upload de novos ativos em uma pasta de Contribuição?**

**Ans.** Consulte a documentação detalhada para  [Fazer upload de ativos na pasta Contribuição](brand-portal-publish-contribution-folder-to-brand-portal.md) .



**Ques. Não vejo miniaturas/visualizações nos ativos carregados na pasta NOVA por um usuário do Brand Portal?**

**Ans.** Como projetado, pois não há fluxo de trabalho sendo executado no Brand Portal.



**Ques. O que acontece se uma pasta é publicada no AEM Assets no Brand Portal que está em fluxo?**

**Ans.** No AEM, os logs são mantidos por cada vez que uma pasta é publicada no Brand Portal. No momento da publicação, todos os ativos que não são publicados no Brand Portal são colocados em uma fila de replicação. Qualquer ativo adicionado à pasta após o trabalho de publicação ser acionado não é publicado no Brand Portal. Quando o usuário do AEM publica a pasta novamente, somente os ativos que não foram publicados anteriormente (existentes na fila de replicação) são publicados no Brand Portal.
Isso é verdadeiro para qualquer pasta publicada do AEM Assets no Brand Portal e para a pasta COMPARTILHADA em uma pasta Contribuição.

**Ques. Com quem eu faço contato?**

**Ans.** Entre em contato com o Gerente de conta da Adobe ou com o Suporte ao cliente.

>[!NOTE]
>
>A programação de versões é provisória e está sujeita a alterações. Entre em contato com o Gerente de conta da Adobe ou com o Suporte ao cliente para obter o cronograma atualizado.


## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente do e precisar de acesso, entre em contato com o gerente de conta da Adobe.

* [](https://daycare.day.com) [Acesso ao produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html)
