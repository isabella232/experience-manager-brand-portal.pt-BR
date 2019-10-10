---
title: Criar pasta de contribuição
seo-title: Criar pasta de contribuição
description: 'Saiba mais sobre como criar uma pasta de contribuição nos ativos AEM. '
seo-description: Saiba mais sobre como criar uma pasta de contribuição nos ativos AEM.
uuid: null
content-type: referência
topic-tags: portal de marcas
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Create contribution folder {#create-contribution-folder}

Os usuários do AEM (administradores/usuários não administradores) podem criar novas pastas no AEM Assets com uma propriedade adicional de contribuição **** de ativos, garantindo que a nova pasta criada esteja aberta para envio de ativos por usuários do Brand Portal.  Isso aciona automaticamente um fluxo de trabalho que cria duas subpastas adicionais, chamadas de **COMPARTILHADO** e **NOVO**, na pasta recém-criada **Contribuição** .

**Para criar uma nova pasta de contribuição:**
1. Faça logon na instância do autor de AEMURL padrão: http:// localhost:4502/aem/start.html
1. Navegue até **[!UICONTROL Ativos &gt; Arquivos]** Ele lista todas as pastas existentes no repositório do AEM Assets.
1. Click **[!UICONTROL Create]** to create a new folder. A janela pop-up Criar pasta é aberta.
1. Digite **[!UICONTROL Título]** e **[!UICONTROL Nome]** da pasta e marque a caixa de seleção **[!UICONTROL Contribuição]**do ativo.
É recomendável usar pequenos alfabetos sem espaço para nomear a pasta.
1. Clique em **[!UICONTROL Criar]**.
   ![](assets/create-contribution-folder.png)
1. Você pode ver a pasta de contribuição recém-criada listada no repositório do AEM Assets.
1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL COMPARTILHADO]** e **[!UICONTROL NOVO]** são criadas automaticamente na pasta de contribuição.\
   ![](assets/contribution-folder.png)

Agora, você pode configurar as propriedades da pasta Contribuição recém-criada. Consulte [Configurar propriedades](brand-portal-configure-contribution-folder-properties.md)da pasta Contribuição.