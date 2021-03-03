---
title: 'Configurar e publicar a pasta de contribuição do AEM Assets no Brand Portal '
seo-title: Configurar e publicar a pasta de contribuição do AEM Assets no Brand Portal
description: Obtenha informações sobre como configurar e publicar uma pasta de contribuição do AEM Assets no Brand Portal.
seo-description: Obtenha informações sobre como configurar e publicar uma pasta de contribuição do AEM Assets no Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: d70817274ac7be84528778352f34934a0d4a60fc
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 0%

---


# Configurar a pasta de contribuição no AEM Assets {#configure-contribution-folder}

Para o fornecimento de ativos colaborativos, os usuários do AEM (administradores e usuários não administradores com permissão) podem criar novas pastas do tipo **Contribuição de ativos**, garantindo que a nova pasta criada esteja aberta para o envio de ativos por usuários do Brand Portal.  Isso aciona automaticamente um workflow que cria duas subpastas adicionais, chamadas **SHARED** e **NEW**, na pasta recém-criada **Contribution**.

O usuário do AEM então define os requisitos do ativo carregando um resumo sobre os tipos de ativos que devem ser adicionados à pasta de contribuição, bem como um conjunto de ativos da linha de base, à pasta **SHARED** para garantir que os usuários do Brand Portal tenham as informações necessárias. O administrador pode conceder acesso aos usuários ativos do Brand Portal à pasta de contribuição antes de publicar a pasta de Contribuição recém-criada no Brand Portal.

O vídeo a seguir demonstra como configurar uma pasta Contribuição no AEM Assets:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

O usuário do AEM executa as seguintes atividades ao configurar uma pasta de contribuição:

* [Criar pasta de contribuição](#create-contribution-folder)
* [Fazer upload dos requisitos de ativos e atribuir colaboradores](#configure-contribution-folder-properties)
* [Fazer upload de ativos da linha de base](#uplad-new-assets-to-contribution-folder)
* [Publicar a pasta de contribuição do AEM Assets no Brand Portal](#publish-contribution-folder-to-brand-portal)

## Criar pasta de contribuição {#create-contribution-folder}


Administradores do AEM e usuários não administradores com permissão para criar uma nova pasta podem criar uma pasta de contribuição no AEM Assets.
Para criar uma pasta de contribuição, crie uma nova pasta do tipo Contribuição de ativo, garantindo que a nova pasta criada esteja aberta para o envio de ativos pelos usuários do Brand Portal.  Isso aciona automaticamente um workflow que cria duas subpastas adicionais, chamadas SHARED e NEW, na pasta de contribuição.


>[!NOTE]
>
>Você pode criar várias pastas de contribuição em uma pasta. Não crie uma pasta de contribuição dentro de outra pasta de contribuição.

Você pode configurar as propriedades da pasta de contribuição separadamente e ao criar a pasta de contribuição. Neste exemplo, estamos configurando as propriedades separadamente.

**Para criar uma pasta de contribuição:**
1. Faça logon na instância do AEM Assets.

1. Navegue até **[!UICONTROL Assets]** > **[!UICONTROL Arquivos]**. Ela lista todas as pastas existentes no repositório do AEM Assets.

1. Clique em **[!UICONTROL Criar]** para criar uma nova pasta. **[!UICONTROL A caixa de diálogo Criar]** pasta é aberta.

1. Insira **[!UICONTROL Título]** e **[!UICONTROL Nome]** da pasta e selecione a caixa de seleção **[!UICONTROL Contribuição do ativo]**.
É recomendável usar letras minúsculas sem espaço para nomear a pasta.

1. Clique em **[!UICONTROL Criar]**. Você pode ver a pasta de contribuição listada no repositório do AEM Assets.

   >[!NOTE]
   >
   >Um usuário não administrador pode criar e compartilhar uma pasta de contribuição de ativos, mas não pode modificá-la ou excluí-la.


   ![](assets/create-contribution-folder.png)

1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL SHARED]** e **[!UICONTROL NEW]** são criadas automaticamente na pasta de contribuição.

   ![](assets/contribution-folder.png)


## Configurar as propriedades da pasta de contribuição {#configure-contribution-folder-properties}

O administrador do AEM executa as seguintes atividades ao configurar as propriedades de uma pasta de contribuição.

* **Adicionar descrição**: Forneça uma descrição de alto nível da pasta de contribuição.
* **Upload breve**: Fazer upload do documento de Requisito de ativo contendo informações relacionadas ao ativo.
* **Adicionar colaboradores**: Adicione usuários do Brand Portal para conceder acesso à pasta de contribuição.

O requisito de ativos refere-se aos detalhes fornecidos pelos administradores para ajudar os colaboradores (usuários do Brand Portal) a entender a necessidade e os requisitos da pasta de contribuição. O administrador faz upload de um documento de requisito de ativo que contém um resumo sobre o tipo de ativos que devem ser adicionados à pasta de contribuição e às informações relacionadas a ativos, por exemplo, finalidade, tipo de imagens, tamanho máximo etc.

**Para configurar as propriedades da pasta de contribuição:**

1. Faça logon na instância do AEM Assets.

1. Navegue até **[!UICONTROL Assets > Files]** e localize a pasta de contribuição.
1. Selecione a pasta de contribuição e clique em **[!UICONTROL Properties]** para abrir a janela Propriedades da pasta.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navegue até a guia **[!UICONTROL Contribuição do ativo]**.
1. Insira **[!UICONTROL Descrição]** de alto nível da pasta de contribuição.
1. Clique em **[!UICONTROL Fazer upload do resumo]** para navegar do computador local e fazer upload de um **Documento de requisitos de ativos**.

   ![](assets/upload.png)

1. No campo **[!UICONTROL Adicionar usuário]**, adicione usuários do Brand Portal com quem deseja compartilhar a pasta de contribuição. Esses usuários podem acessar e fazer upload de conteúdo para a pasta de contribuição usando a interface do Brand Portal.
1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Os resultados da pesquisa são baseados na lista de usuários do Brand Portal configurada no AEM Assets. Certifique-se de ter a lista de usuários atualizada do Brand Portal.

## Fazer upload de ativos para a pasta de contribuição {#uplad-new-assets-to-contribution-folder}

Os usuários do Brand Portal podem baixar os requisitos de ativos para entender a necessidade de contribuição.
Em seguida, eles podem criar novos ativos para contribuição e carregá-los na pasta NEW na pasta de contribuição.

>[!NOTE]
>
>Os usuários do Brand Portal podem fazer upload de ativos somente para a nova pasta.
>
>O limite máximo de upload para qualquer locatário do Brand Portal é **10** GB que é aplicado cumulativamente a todas as pastas de contribuição.


Após publicar os ativos recém-criados no AEM Assets, os usuários do Brand Portal podem excluí-los da NOVA pasta. Enquanto isso, o administrador do Brand Portal pode excluir os ativos das pastas NOVO e COMPARTILHADO.

Quando o objetivo de criar a pasta de contribuição for atingido, o administrador do Brand Portal poderá excluir a pasta de contribuição para liberar o espaço de upload para outros usuários.

>[!NOTE]
>
>É recomendável liberar o espaço de upload após a publicação da pasta de contribuição nos ativos AEM para que ele fique disponível para outros usuários do Brand Portal para contribuição.
>
>Se for necessário estender o limite de upload do locatário do Brand Portal para além de **10** GB, entre em contato com o Suporte da Adobe especificando o requisito.


**Para fazer upload de novos ativos:**

1. Faça logon na instância do Brand Portal.
O painel Brand Portal reflete todas as pastas existentes permitidas para o usuário do Brand Portal junto com a pasta de contribuição recém-compartilhada.

1. Selecione a pasta de contribuição e clique em para abri-la. A pasta de contribuição contém duas subpastas - **[!UICONTROL SHARED]** e **[!UICONTROL NEW]**.

1. Clique na pasta **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets1.png)

1. Clique em **[!UICONTROL Create]** > **[!UICONTROL Files]** para carregar arquivos individuais ou pastas (.zip) contendo vários ativos.

   ![](assets/upload-new-assets2.png)

1. Navegue e faça upload de ativos (arquivos ou pastas) para a pasta **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

Depois de fazer upload de todos os ativos ou pastas para a NOVA pasta, publique a pasta de contribuição no AEM Assets.


## Publicar a pasta de contribuição no Brand Portal {#publish-contribution-folder-to-brand-portal}

Depois que a pasta de contribuição é configurada, o usuário do AEM (administrador/não administrador) pode publicar a pasta de contribuição do AEM Assets no Brand Portal. Os usuários do Brand Portal que tiverem permissão para acessar a pasta de contribuição receberão uma notificação por e-mail/pulso ao concluir a ação de publicação.


**Para publicar a pasta de contribuição:**

1. Faça logon na instância do AEM Assets.

1. Navegue até **[!UICONTROL Assets > Files]** e localize a pasta de contribuição na qual deseja publicar no Brand Portal.
1. Selecione a pasta de contribuição e clique em **[!UICONTROL Publicação rápida]** > **[!UICONTROL Publicar no Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Você receberá uma mensagem de sucesso assim que a pasta de contribuição for publicada no Brand Portal.

Uma notificação por e-mail/pulso é enviada aos usuários do Brand Portal atribuídos à pasta de contribuição. Os usuários do Brand Portal podem acessar a pasta de contribuição e iniciar a contribuição. Consulte [Fazer upload de ativos para a pasta de contribuição e publicar no AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
