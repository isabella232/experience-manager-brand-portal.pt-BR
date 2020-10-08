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
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}


AEM administradores e usuários não administradores com permissão para criar uma nova pasta podem criar uma pasta de contribuição no AEM Assets.
Para criar uma pasta de contribuição, crie uma nova pasta do tipo Contribuição do ativo, garantindo que a nova pasta criada esteja aberta para o envio de ativos pelos usuários do Brand Portal.  Isso aciona automaticamente um fluxo de trabalho que cria duas subpastas adicionais, chamadas COMPARTILHADO e NOVO, dentro da pasta de contribuição.

>[!NOTE]
>
>Você pode criar várias pastas de contribuição dentro de uma pasta, mas não deve criar uma pasta de contribuição dentro de outra pasta de contribuição.

Para criar uma pasta de contribuição:
1. Faça logon na instância do autor AEM.

   O URL padrão é http:// localhost:4502/aem/start.html.

1. Navegue até **[!UICONTROL Ativos]** > **[!UICONTROL Arquivos]**. Ele lista todas as pastas existentes no repositório AEM Assets.

1. Click **[!UICONTROL Create]** to create a new folder. **[!UICONTROL A caixa de diálogo Criar pasta]** é aberta.

1. Digite **[!UICONTROL Título]** e **[!UICONTROL Nome]** da pasta e marque a caixa de seleção Contribuição **[!UICONTROL do]** ativo.
É recomendável usar letras minúsculas sem espaço para nomear a pasta.

1. Clique em **[!UICONTROL Criar]**. Você pode ver a pasta de contribuição listada no repositório AEM Assets.

   >[!NOTE]
   >
   >Um usuário não administrador pode criar e compartilhar uma pasta de contribuição de ativos, mas não pode modificá-la nem excluí-la.

   ![](assets/create-contribution-folder.png)

1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL COMPARTILHADO]** e **[!UICONTROL NOVO]** são criadas automaticamente na pasta de contribuição.

   ![](assets/contribution-folder.png)

Agora você pode [configurar as propriedades](brand-portal-configure-contribution-folder-properties.md)da pasta de contribuição.


