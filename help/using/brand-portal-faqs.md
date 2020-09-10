---
title: Perguntas frequentes
seo-title: null
description: Saiba mais sobre as perguntas frequentes no Portal de marcas dos Ativos Adobe Experience Manager.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: a87f85a11e8892e6f306a003d971403581a9e3d7
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 1%

---


# Perguntas frequentes {#frequently-asked-questions}

As Perguntas frequentes sobre o Brand Portal se concentram nos query e problemas dos usuários finais que podem encontrar ao trabalhar com a versão mais recente do AEM Assets Brand Portal 6.4.6 ou versões anteriores.


## Perguntas frequentes sobre o Brand Portal 6.4.6  {#faqs-bp646}

**Ques. O endpoint OAuth existente (`https://legacy-oauth.cloud.adobe.io/login`) herdado não está funcionando. Qual poderia ser a razão possível?**

**Ans.** A configuração OAuth herdada está obsoleta. Você deve atualizar as instâncias do autor do AEM Assets para o service pack mais recente e configurá-las por meio do Adobe Developer Console. Consulte [Configurar o AEM Assets com o Brand Portal](configure-aem-assets-with-brand-portal.md) para obter detalhes. No entanto, para que a configuração OAuth herdada funcione até que você atualize, atualize o terminal OAuth herdado para `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Não consigo publicar os ativos da pasta de contribuição do Brand Portal para a AEM Assets depois de atualizar para o Adobe Developer Console. A minha autora está no AEM 6.5.4. Qual poderia ser a razão possível?**

**Ans.** Sim, há um problema conhecido ao publicar os ativos da pasta de contribuição para a AEM Assets no AEM 6.5.4 por meio do Adobe Developer Console.

O problema foi corrigido no AEM 6.5.5. Você pode atualizar sua instância do AEM Assets para o service pack mais recente AEM 6.5.5 e [atualizar suas configurações](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) no Adobe Developer Console.

Para uma correção imediata no AEM 6.5.4, é recomendável [baixar a correção](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalá-la na instância AEM autor.

**Ques. Não vejo o conteúdo da pasta de contribuição publicado no Brand Portal na AEM Assets. Qual poderia ser a razão possível?**

**Ans.** Entre em contato com o administrador da AEM Assets para verificar as configurações e garantir que o locatário do Brand Portal esteja configurado com apenas uma instância do autor da AEM Assets.

Esse problema pode ocorrer quando você tiver configurado um locatário do Brand Portal em várias instâncias do autor do AEM Assets. Por exemplo, o administrador configura o mesmo locatário do Brand Portal na instância do autor da AEM Assets do ambiente de preparo e produção. Nesse caso, a publicação de ativos é acionada no Brand Portal, mas a instância do autor da AEM Assets não pôde importar o cuz do ativo que o agente de replicação não recebe o token solicitante.


**Ques. Não consigo publicar ativos do AEM Assets para o Brand Portal. O log de replicação indica que a conexão expirou. Há uma solução rápida?**

**Ans.** Normalmente, a publicação falha com um erro de tempo limite se houver várias solicitações pendentes na fila de replicação. Para resolver esse problema, verifique se os agentes de replicação estão configurados para evitar o tempo limite.

Execute as seguintes etapas para configurar o agente de replicação:
1. Faça logon na instância do autor do AEM Assets.
1. No painel **Ferramentas** , navegue até **[!UICONTROL Implantação]** > **[!UICONTROL Replicação]**.
1. Na página Replicação, clique em **[!UICONTROL Agentes no autor]**. Você pode ver os quatro agentes de replicação do seu locatário do Brand Portal.
1. Clique no URL do agente de replicação para abrir os detalhes do agente.
1. Clique em **[!UICONTROL Editar]** para modificar as configurações do agente de replicação.
1. Em Configurações do agente, clique na guia **[!UICONTROL Estendido]** .
1. Marque a caixa de seleção **[!UICONTROL Fechar conexão]** .
1. Repita as etapas de 4 a 7 para configurar todos os quatro agentes de replicação.
1. Reinicie o servidor e verifique a conexão.


## Perguntas frequentes sobre o Brand Portal 6.4.5  {#faqs-bp645}

**Ques. Qual é a grande mudança na versão 6.4.5 do Brand Portal?**

**Ans.** O AEM Assets Brand Portal 6.4.5 é uma versão de recurso que permite que os usuários do Brand Portal façam upload de conteúdo dentro da instância do Brand Portal e publiquem a pasta Contribuição de volta para a AEM Assets sem precisar de direitos de administrador.
Para obter mais informações, consulte Seleção de [recursos no Portal](brand-portal-asset-sourcing.md)da marca.



**Ques. Perderei o acesso a ativos, recursos ou configurações existentes que criei?**

**Ans.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não são afetados e seu conteúdo permanece intacto.



**Ques. Quando eu vou mudar para a nova versão do Brand Portal?**

**Ans.** O Brand Portal 6.4.5 foi lançado para produção em outubro de 2019. E a próxima versão do Brand Portal deverá ser lançada no terceiro trimestre de 2020.
Para atualizações e alterações de versão, é recomendável rastrear as Notas [de](brand-portal-release-notes.md) versão e [Novidades do Brand Portal](whats-new.md).



**Ques. Meus usuários serão afetados?**

**Ans.** A versão do Brand Portal 6.4.5 está exclusivamente no Brand Portal, portanto não há impacto para os usuários finais.



**Ques. Há alguma ação necessária da minha parte como usuário do Brand Portal?**

**Ans.** A versão 6.4.5 do Brand Portal vem com um novo recurso chamado Asset Sourcing. AEM administrador deve configurar o recurso de Seleção de ativos no AEM Assets para habilitar o recurso para os usuários do Brand Portal. Para obter mais informações, consulte [Ativar fonte](brand-portal-configure-asset-sourcing.md)de ativos.



**Ques. Quem pode criar uma pasta de contribuição?**

**Ans.** Qualquer usuário AEM com permissões para criar uma nova pasta no AEM Assets pode criar uma pasta **do Contribution** . Para criar uma pasta **Contribuição** , crie uma nova pasta do tipo Contribuição **de**ativo.
Essa pasta é compartilhada com os usuários ativos do Brand Portal para obter contribuição.



**Ques. O que uma pasta de contribuição contém?**

**Ans.** **A pasta de contribuição** contém duas subpastas **NEW** e **SHARED**. Inicialmente, a pasta NEW está em branco e a pasta SHARED contém o conteúdo de referência (ativos reutilizáveis) para os usuários do Brand Portal.
Os usuários do Brand Portal acessam a pasta **Contribution** e carregam conteúdo na pasta **NEW** .



**Ques.  É possível modificar o nome de uma pasta de contribuição existente?**

**Ans.** **Não**, não é possível modificar o nome de uma pasta **de contribuição** existente.



**Ques. Quais são os requisitos de ativos com contribuição de r l&#39;r?**

**Ans.** O **documento Brief** anexado à pasta **Contribution** e ao conteúdo de referência (ativos reutilizáveis) carregado na pasta **SHARED** ajuda o usuário do Brand Portal a entender a necessidade de contribuição e expectativas como um contribuinte, e é chamado coletivamente de requisitos de ativos.



**Ques. É possível fazer upload de ativos para qualquer pasta permitida?**

**Ans.** Nem todas as pastas permitidas. Um usuário do Brand Portal só pode carregar conteúdo para a pasta **Contribution** que é compartilhada pelo administrador do AEM ou do Brand Portal.



**Ques. Como faço para obter acesso a uma pasta de contribuição?**

**Ans.** Você pode acessar uma pasta **de contribuição** somente se ela tiver sido compartilhada com você. Você receberá uma notificação por email/pulsação sempre que uma pasta de contribuição for compartilhada com você. Você pode acessar a pasta Contribuição por meio do link compartilhado no e-mail ou fazer logon na instância do Brand Portal e navegar até o ícone de sinalizador para obter notificações para acessar a pasta Contribuição.

>[!NOTE]
>
>Se você não for um usuário existente do Brand Portal, solicite ao administrador do AEM que crie seu usuário no Admin Console AEM e adicione seu perfil ao arquivo de configuração do usuário na lista de usuários do Brand Portal. Consulte, [Adicionar usuário](brand-portal-configure-asset-sourcing.md)do Brand Portal.

**Ques. Qual é o Formato do arquivo CSV para importação de usuário?**

**Ans.** O formato é o mesmo que o Admin Console para a importação de usuários em massa. Email, nome e sobrenome são obrigatórios.



**Ques. O que preenche a lista de usuários (contribuidores do Brand Portal) no menu suspenso de usuários da Contribuição de ativos?**

**Ans.** Os usuários na lista suspensa são preenchidos a partir do arquivo de configuração de usuário (.csv) do Brand Portal carregado no AEM.



**Ques. Onde posso ver o status das tarefas de importação e publicação?**

**Ans.** Em AEM, você pode ver o status de uma importação na página de trabalho **assíncrona** . No Brand Portal, você pode ver o status de um trabalho de publicação em **[!UICONTROL Ferramentas > Status]** de contribuição de ativos.



**Ques. Qual é a frequência de um trabalho de importação que é executado periodicamente em AEM?**

**Ans.** Em AEM, a votação é feita a cada 5 minutos.



**Ques. Existe algum limite no número de vezes que uma pasta pode ser publicada do Portal de marcas para a AEM Assets?**

**Ans.** Não, todos os ativos na pasta **NEW** são publicados na AEM Assets independentemente do fato de terem sido publicados anteriormente. Sempre que uma pasta **Contribution** é publicada do Brand Portal para a AEM Assets, ela substitui o conteúdo da pasta **NEW** .



**Ques. Como fazer upload de novos ativos em uma pasta de contribuição?**

**Ans.** Consulte a documentação detalhada para [Fazer upload de ativos para a pasta](brand-portal-upload-assets-to-contribution-folder.md)Contribuição.



**Ques. Não vejo miniaturas/pré-visualizações nos ativos carregados para a pasta NEW por um usuário do Brand Portal?**

**Ans.** Como projetado, porque não há fluxo de trabalho sendo executado no Portal da Marca.



**Ques. O que acontece se uma pasta for publicada do AEM Assets para o Brand Portal que está em fluxo?**

**Ans.** Em AEM, os registros são mantidos sempre que uma pasta é publicada no Brand Portal. No momento da publicação, todos os ativos que não são publicados no Brand Portal são colocados em uma fila de replicação. Qualquer ativo adicionado à pasta depois que o trabalho de publicação é acionado não é publicado no Brand Portal. Quando o usuário AEM publica a pasta novamente, somente os ativos que não foram publicados anteriormente (existentes na fila de replicação) são publicados no Brand Portal.
Isso é válido para qualquer pasta publicada do AEM Assets para o Brand Portal e para a pasta COMPARTILHADA em uma pasta de contribuição.



**Ques. Com quem eu entro em contato com as perguntas?**

**Ans.** Entre em contato com seu Gerente de contas do Adobe ou com o Suporte ao cliente.


>[!NOTE]
>
>O cronograma de liberação é provisório e está sujeito a alterações. Entre em contato com seu Gerente de contas do Adobe ou com o Suporte ao cliente para obter o cronograma atualizado de lançamento.





## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente e precisar de acesso, entre em contato com seu gerente de contas do Adobe.

* [](https://daycare.day.com) [Acesso ao produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente Adobe](https://helpx.adobe.com/contact.html)
