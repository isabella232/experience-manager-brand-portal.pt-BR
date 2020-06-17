---
title: Criar pasta de contribuição
seo-title: Criar pasta de contribuição
description: 'Obtenha informações sobre como criar uma pasta de contribuição no AEM Assets. '
seo-description: Obtenha informações sobre como criar uma pasta de contribuição no AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ac5952c318baae8400928592d9a372ab966191cf
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}

Os administradores do AEM e usuários não administradores com permissão para criar uma nova pasta podem criar uma pasta **Contribuição** no AEM Assets.
Para criar uma pasta **Contribuição** , crie uma nova pasta do tipo Contribuição **de** ativo, garantindo que a nova pasta criada esteja aberta para o envio de ativos pelos usuários do Brand Portal.  Isso aciona automaticamente um fluxo de trabalho que cria duas subpastas adicionais, chamadas de **COMPARTILHADO** e **NOVO**, na pasta recém-criada **Contribuição** .

**Para criar uma nova pasta de contribuição:**
1. Faça logon na instância do autor de AEMURL padrão: http:// localhost:4502/aem/start.html
1. Navegue até **[!UICONTROL Ativos > Arquivos]** Ele lista todas as pastas existentes no repositório do AEM Assets.
1. Click **[!UICONTROL Create]** to create a new folder. A janela pop-up Criar pasta é aberta.
1. Digite **[!UICONTROL Título]** e **[!UICONTROL Nome]** da pasta e marque a caixa de seleção **[!UICONTROL Contribuição]**do ativo.
É recomendável usar pequenos alfabetos sem espaço para nomear a pasta.
1. Clique em **[!UICONTROL Criar]**.
   ![](assets/create-contribution-folder.png)
1. Você pode ver a pasta de contribuição recém-criada listada no repositório AEM Assets.
1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL COMPARTILHADO]** e **[!UICONTROL NOVO]** são criadas automaticamente na pasta de contribuição.\
   ![](assets/contribution-folder.png)

Agora você pode configurar as propriedades da pasta Contribuição. Consulte [Configurar propriedades](brand-portal-configure-contribution-folder-properties.md)da pasta Contribuição.

>[!NOTE]
>
>Certifique-se de fornecer um nome apropriado para a pasta Contribuição, pois não é possível modificar o nome da pasta após a criação.
>
>O aninhamento da pasta Contribuição não é suportado. Não crie uma pasta de contribuição dentro de outra pasta de contribuição.

