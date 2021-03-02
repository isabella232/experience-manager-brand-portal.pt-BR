---
title: Faça upload de ativos e publique a pasta Contribuição do Brand Portal para o AEM Assets
seo-title: Faça upload de ativos e publique a pasta Contribuição do Brand Portal para o AEM Assets
description: Obtenha informações sobre como fazer upload de novos ativos e publicar a pasta de contribuição do Brand Portal para o AEM Assets.
seo-description: Obtenha informações sobre como fazer upload de novos ativos e publicar a pasta de contribuição do Brand Portal para o AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 268ee9dc83e98e01107f474780b658b8ccefafa4
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---


# Publicar a pasta de contribuição no AEM Assets {#using-asset-souring-in-bp}

Usuários do Brand Portal com permissões apropriadas podem fazer upload de vários ativos ou pastas contendo vários ativos para a pasta de contribuição. No entanto, os usuários do Brand Portal só podem fazer upload de ativos para a pasta **NEW**. A pasta **SHARED** destina-se à distribuição de ativos de linha de base (conteúdo de referência) que podem ser usados pelos usuários do Brand Portal ao criar novos ativos para contribuição.

O usuário do Brand Portal com permissão para acessar a pasta de contribuição pode executar as seguintes atividades:

* [Baixar requisitos de ativos](#download-asset-requirements)
* [Fazer upload de novos ativos para a pasta de contribuição](#uplad-new-assets-to-contribution-folder)
* [Publicar a pasta de contribuição no AEM Assets](#publish-contribution-folder-to-aem)

## Baixar requisitos de ativos {#download-asset-requirements}

Os usuários do Brand Portal recebem automaticamente notificações por email/pulso sempre que uma pasta de contribuição é compartilhada pelo usuário do AEM, permitindo baixar o documento resumido (requisito de ativo), bem como baixar os ativos da linha de base (conteúdo de referência), da pasta **SHARED** para garantir que compreendam os requisitos de ativos.

O usuário do Brand Portal realiza as seguintes atividades para baixar os requisitos de ativos:

* **Resumo** do download: Baixe o resumo (documento de requisito de ativo) anexado à pasta de contribuição que contém informações relacionadas ao ativo, como tipo de ativos, finalidade, formatos compatíveis, tamanho máximo do ativo etc.
* **Baixar ativos** da linha de base: Baixe os ativos da linha de base que podem ser usados para entender os tipos de ativos necessários. Os usuários do Brand Portal podem usar esses ativos como referência para criar novos ativos para contribuição.

O painel Brand Portal reflete todas as pastas existentes permitidas para o usuário do Brand Portal junto com a pasta de contribuição recém-compartilhada. Neste exemplo, o usuário do Brand Portal só tem acesso à pasta de contribuição recém-criada, nenhuma outra pasta existente é compartilhada com o usuário.

**Para baixar os requisitos de ativos:**

1. Faça logon na instância do Brand Portal.
1. Selecione a pasta de contribuição no painel Brand Portal .
1. Clique em **[!UICONTROL Propriedades]** ![](assets/properties.png). A janela Propriedade é aberta, exibindo os detalhes da pasta Contribuição do ativo.
   ![](assets/download-asset-requirement1.png)
1. Clique em **[!UICONTROL Baixar resumo]** ![](assets/download.png) para baixar o documento de requisito de ativos no computador local.
   ![](assets/download-asset-requirement2.png)
1. Volte para o painel Brand Portal .
1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL SHARED]** e **[!UICONTROL NEW]** na pasta de contribuição. A pasta COMPARTILHADA contém todos os ativos de linha de base (conteúdo de referência) compartilhados pelos administradores.
1. Você pode baixar a pasta **[!UICONTROL SHARED]** contendo todos os ativos da linha de base em sua máquina local.
Ou, você pode abrir a pasta **[!UICONTROL SHARED]** e clicar em **Download** ícone ![](assets/download.png) para baixar arquivos/pastas individuais.
   ![](assets/download-asset-requirement3.png)

Analise o resumo (documento de requisito de ativo) e consulte os ativos da linha de base para entender os requisitos de ativos. Agora, você pode criar novos ativos para contribuição e carregá-los na pasta de contribuição.


## Fazer upload de ativos para a pasta de contribuição {#uplad-new-assets-to-contribution-folder}

Após analisar os requisitos de ativos, os usuários do Brand Portal podem criar novos ativos para contribuição e carregá-los na pasta NOVA na pasta de contribuição.

>[!NOTE]
>
>Os usuários do Brand Portal podem fazer upload de ativos somente para a nova pasta.
>
>O limite máximo de upload para qualquer locatário do Brand Portal é **10** GB que é aplicado cumulativamente a todas as pastas de contribuição.

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


## Publicar a pasta de contribuição no AEM Assets {#publish-contribution-folder-to-aem}

Os usuários do Brand Portal podem publicar a pasta de contribuição no AEM Assets sem precisar acessar a instância do autor do AEM.

Certifique-se de ter passado pelos requisitos do ativo e carregado os ativos recém-criados na pasta **NEW** na pasta de contribuição.

**Para publicar a pasta de contribuição:**

1. Faça logon na instância do Brand Portal.

1. Selecione a pasta de contribuição no painel Brand Portal .
1. Clique em **[!UICONTROL Publicar no AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

Uma notificação por email/pulso é enviada ao usuário e administradores do Brand Portal em diferentes estágios do fluxo de trabalho de publicação:
1. **Em fila**  - Uma notificação é enviada ao usuário do Brand Portal e aos administradores do Brand Portal quando um fluxo de trabalho de publicação é acionado no Brand Portal.

1. **Concluído**  - Uma notificação é enviada ao usuário do Brand Portal e aos administradores do Brand Portal quando a pasta de contribuição é publicada com êxito no AEM Assets.

Após publicar os ativos recém-criados no AEM Assets, os usuários do Brand Portal podem excluí-los da NOVA pasta. Enquanto isso, o administrador do Brand Portal pode excluir os ativos das pastas NOVO e COMPARTILHADO.

Quando o objetivo de criar a pasta de contribuição for atingido, o administrador do Brand Portal poderá excluir a pasta de contribuição para liberar o espaço de upload para outros usuários.

**Publicar o status do trabalho**

Há dois relatórios que os administradores podem utilizar para visualizar o status das pastas de contribuição de ativos publicadas do Brand Portal para o AEM Assets.

* No Brand Portal, navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Status de contribuição de ativos]**. Este relatório reflete o status de todos os trabalhos de publicação em estágios diferentes do fluxo de trabalho de publicação.

   ![](assets/contribution-folder-status.png)

* Na instância do autor do AEM Assets, navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Trabalhos]**. Este relatório reflete o estado final (Sucesso ou Erro) de todos os trabalhos de publicação.

   ![](assets/publishing-status.png)

>[!NOTE]
>
>A interface do usuário do AEM Assets as a Cloud Service pode ter uma pequena diferença, mas o fluxo de trabalho permanece inalterado.






