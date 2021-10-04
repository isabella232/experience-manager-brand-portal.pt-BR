---
title: Compartilhar uma coleção
seo-title: Share a collection
description: Os administradores do Experience Manager Assets Brand Portal podem compartilhar e cancelar o compartilhamento de uma coleção ou de uma coleção inteligente com usuários autorizados. Os editores podem exibir e compartilhar apenas as coleções criadas por eles, compartilhadas com eles e coleções públicas.
seo-description: Experience Manager Assets Brand Portal Administrators can share and unshare a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
exl-id: 29b877f6-4200-4299-9b8d-81d88f4e8221
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---

# Compartilhar coleções {#share-collections}

Uma coleção representa um grupo de ativos relacionados armazenados juntos no Adobe Experience Manager Assets Brand Portal. Os usuários podem criar coleções inteligentes ao [aplicar pesquisa omnisearch ou facet para filtrar ativos relacionados](brand-portal-searching.md) e armazená-los juntos para fácil acesso e compartilhá-los com outros usuários do Brand Portal.

Os administradores podem compartilhar e cancelar o compartilhamento de uma coleção com os usuários autorizados do Brand Portal. Editores e visualizadores podem exibir e compartilhar as coleções criadas por eles, compartilhadas com eles e coleções públicas.

>[!NOTE]
>
>Os editores não podem alterar uma coleção pública para uma coleção não pública e, portanto, não têm a caixa de seleção **[!UICONTROL Coleção pública]** disponível na caixa de diálogo **[!UICONTROL Configurações da coleção]**.

## Compartilhar uma coleção {#share-collection}

A seguir estão as etapas para compartilhar uma coleção com usuários autorizados do Brand Portal:

1. Faça logon no locatário do Brand Portal. Por padrão, a visualização **[!UICONTROL Arquivos]** é aberta e contém todos os ativos e pastas publicados.

1. Nas navegações rápidas na parte superior, clique em **[!UICONTROL Collections]**.

1. No console **[!UICONTROL Collections]**, execute um dos seguintes procedimentos:

   * Passe o ponteiro do mouse sobre a coleção que deseja compartilhar. Nas miniaturas de ação rápida disponíveis para a coleção, clique no ícone **[!UICONTROL Settings]**.

      ![](assets/settings-icon.png)

   * Selecione a coleção que deseja compartilhar. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Configurações]**.

      ![](assets/collection-console.png)

1. Na caixa de diálogo **[!UICONTROL Configurações da coleção]**, selecione os usuários com quem deseja compartilhar a coleção e selecione a função do usuário para corresponder à função global. Por exemplo, atribua a função de Editor a um editor global, a função de Visualizador a um visualizador global.

   Como alternativa, para disponibilizar a coleção para todos os usuários, independentemente de sua associação e função de grupo, torne-a pública, marcando a caixa de seleção **[!UICONTROL Coleção pública]**.

   >[!NOTE]
   >
   >No entanto, os usuários não administradores podem ser restritos à criação de coleções públicas, para evitar muitas coleções públicas e para que o espaço do sistema possa ser salvo. As organizações podem desabilitar a configuração **[!UICONTROL Permitir criação de coleções públicas]** das configurações **[!UICONTROL Geral]** disponíveis no painel Ferramentas administrativas.

   ![](assets/collection_sharingadduser.png)

   Os editores não podem alterar uma coleção pública para uma coleção não pública e, portanto, não têm a caixa de seleção **[!UICONTROL Coleção pública]** disponível na caixa de diálogo **[!UICONTROL Configurações da coleção]**.

   ![](assets/collection-setting-editor.png)

1. Clique no botão **[!UICONTROL Adicionar]** para adicionar o usuário e clique em **[!UICONTROL Salvar]**. A coleção é compartilhada com os usuários.

   >[!NOTE]
   >
   >A função de um usuário governa o acesso aos ativos e pastas dentro de uma coleção. Se um usuário não tiver acesso aos ativos, uma coleção vazia será compartilhada com o usuário. Além disso, a função de um usuário governa as ações disponíveis para coleções.

## Cancelar compartilhamento de uma coleção {#unshare-a-collection}

Para cancelar o compartilhamento de uma coleção compartilhada anteriormente, faça o seguinte:

1. No console **[!UICONTROL Collections]**, selecione a coleção que deseja cancelar o compartilhamento.

   Na barra de ferramentas na parte superior, clique em **[!UICONTROL Configurações]**.

   ![](assets/collection_settings.png)

1. Na caixa de diálogo **[!UICONTROL Configurações da coleção]**, na seção **[!UICONTROL Membros]**, clique no símbolo **[!UICONTROL x]** ao lado dos usuários para removê-los da lista de usuários que têm acesso à coleção.

   ![](assets/unshare_collection.png)

1. Uma mensagem de aviso é exibida. Clique em **[!UICONTROL Confirm]** para cancelar o compartilhamento da coleção.

1. Clique em **[!UICONTROL Save]** para aplicar as alterações.

   Depois que o usuário é removido da lista compartilhada, a coleção não compartilhada é removida do console **[!UICONTROL Collections]** do usuário.

<!--
1. Click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. From the **[!UICONTROL Collections]** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **[!UICONTROL Settings]** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **[!UICONTROL Settings]**.
    
   ![](assets/collection-sharing.png)

1. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **[!UICONTROL Public Collection]** check-box available in **[!UICONTROL Collection Settings]** dialog.

   ![](assets/collection-setting-editor.png)

1. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **[!UICONTROL Collections]** console, select the collection you want to unshare.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. On the **[!UICONTROL Collection Settings]** dialog box, under **[!UICONTROL Members]**, click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **[!UICONTROL Confirm]** to confirm unshare.

   Click **[!UICONTROL Save]**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **[!UICONTROL Collections]** console.
-->
