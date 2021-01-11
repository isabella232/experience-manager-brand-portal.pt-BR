---
title: Publicar na pasta Contribution no AEM Assets
seo-title: Publicar na pasta Contribution no AEM Assets
description: Saiba mais sobre a publicação da pasta de contribuição para a AEM Assets no Brand Portal.
seo-description: Saiba mais sobre a publicação da pasta de contribuição para a AEM Assets no Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6eb01e2eec7de6b704976c990fb6ffacbc67471a
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# Publicar pasta de contribuição no AEM Assets {#publish-contribution-folder-to-aem}

Os usuários do Brand Portal podem publicar a pasta de contribuição para a AEM Assets sem precisar acessar a instância do autor AEM.

Verifique se você passou pelos [requisitos de ativos](brand-portal-download-asset-requirements.md) e carregou os ativos recém-criados na pasta **NEW** na pasta de contribuição. Consulte, [Carregar ativos para a pasta de contribuição](brand-portal-upload-assets-to-contribution-folder.md).

**Para publicar a pasta de contribuição:**

1. Faça logon na instância do Brand Portal.

1. Selecione a pasta de contribuição do painel do Brand Portal.
1. Clique em **[!UICONTROL Publicar em AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

Uma notificação por email/pulso é enviada para o usuário e administradores do Brand Portal em diferentes estágios do fluxo de trabalho de publicação:
1. **Em fila**  - Uma notificação é enviada para os administradores do Brand Portal e do usuário quando um fluxo de trabalho de publicação é acionado no Brand Portal.

1. **Concluído**  - uma notificação é enviada para o usuário do Brand Portal e para os administradores do Brand Portal quando a pasta de contribuição é publicada com êxito na AEM Assets.


**Publicar status do trabalho**

Há dois relatórios que os administradores podem utilizar para visualização do status das pastas de contribuição de ativos publicadas do Brand Portal para a AEM Assets.

* No Brand Portal, navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Status de contribuição de ativos]**. Este relatório reflete o status de todos os trabalhos de publicação em diferentes estágios do fluxo de trabalho de publicação.

   ![](assets/contribution-folder-status.png)

* Na instância do autor do AEM Assets, navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Tarefas]**. Este relatório reflete o estado final (Sucesso ou Erro) de todos os trabalhos de publicação.

   ![](assets/publishing-status.png)




