---
title: Compartilhar uma coleção
seo-title: Compartilhar uma coleção
description: Os administradores do portal de marcas do AEM Assets podem compartilhar e não compartilhar uma coleção ou uma coleção inteligente com usuários autorizados. Os editores podem exibir e compartilhar somente as coleções criadas por eles, compartilhadas com eles e coleções públicas.
seo-description: Os administradores do portal de marcas do AEM Assets podem compartilhar e não compartilhar uma coleção ou uma coleção inteligente com usuários autorizados. Os editores podem exibir e compartilhar somente as coleções criadas por eles, compartilhadas com eles e coleções públicas.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Compartilhar coleções no Brand Portal {#share-collections-bp}

Os administradores do portal de marcas do AEM Assets podem compartilhar e não compartilhar uma coleção ou uma coleção inteligente com usuários autorizados. Os editores podem exibir e compartilhar somente as coleções criadas por eles, compartilhadas com eles e coleções públicas. No entanto, os editores não podem alterar uma coleção pública para uma coleção não pública.

>[!NOTE]
>
>Os editores não podem alterar uma coleção pública para uma coleção não pública e, portanto, não têm a caixa de seleção Coleção ****pública disponível na caixa de diálogo Configurações**[!UICONTROL  da]** coleção.

## Compartilhar uma coleção {#share-collection}

Para compartilhar uma coleção, siga estas etapas:

1. Clique no ícone de sobreposição à esquerda e escolha **[!UICONTROL Navegação]**.

   ![](assets/contenttree-1.png)

1. Do lado esquerdo, clique em **[!UICONTROL Coleções]**.

   ![](assets/access_collections.png)

1. No console **[!UICONTROL Coleções]**, execute um dos procedimentos a seguir:

   * Passe o ponteiro do mouse sobre a coleção que deseja compartilhar. Nas miniaturas de ação rápida disponíveis para a coleção, clique no ícone **[!UICONTROL Configurações]**.
   ![](assets/settings_thumbnail.png)

   * Selecione a coleção que deseja compartilhar. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Configurações]**.
   ![](assets/collection-sharing.png)

1. Na caixa de diálogo Configurações [!UICONTROL da] coleção, selecione os usuários ou grupos com os quais você deseja compartilhar a coleção e selecione a função para um usuário ou grupo que corresponda à sua função global. Por exemplo, atribua a função Editor a um editor global, a função Visualizador a um visualizador global.

   Como alternativa, para disponibilizar a coleção para todos os usuários, independentemente de sua associação e função, torne-a pública selecionando a caixa de seleção Coleção ****pública.

   >[!NOTE]
   >
   >No entanto, usuários não administradores podem ser restringidos da criação de coleções públicas, para evitar a existência de várias coleções públicas, de modo que o espaço do sistema possa ser salvo. As organizações podem desativar a configuração de criação ****Permitir coleções públicas nas configurações[!UICONTROL Gerais]disponíveis no painel Ferramentas administrativas.

   ![](assets/collection_sharingadduser.png)

   Os editores não podem alterar uma coleção pública para uma coleção não pública e, portanto, não têm a caixa de seleção Coleção ****pública disponível na caixa de diálogo Configurações**[!UICONTROL  da]** coleção.

   ![](assets/collection-setting-editor.png)

1. Selecione **[!UICONTROL Adicionar]**e, em seguida,**[!UICONTROL  Salvar]**. A coleção é compartilhada com os usuários escolhidos.

   >[!NOTE]
   >
   >A função de um usuário governa o acesso aos ativos e pastas dentro de uma coleção. Se um usuário não tiver acesso aos ativos, uma coleção vazia será compartilhada com o usuário. Além disso, a função de um usuário governa as ações disponíveis para coleções.

## Cancelar compartilhamento de uma coleção {#unshare-a-collection}

Para cancelar o compartilhamento de uma coleção compartilhada anteriormente, faça o seguinte:

1. No console **[!UICONTROL Coleções]**, selecione a coleção que deseja cancelar o compartilhamento.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. Na caixa de diálogo Configurações **[!UICONTROL da]**coleção, em**[!UICONTROL  Membros]**, clique no símbolo **[!UICONTROL x]**ao lado de usuários ou grupos para removê-los da lista de usuários com os quais você compartilhou a coleção.

   ![](assets/unshare_collection.png)

1. Na caixa de mensagem de aviso, clique em **[!UICONTROL Confirmar]**para confirmar o cancelamento do compartilhamento.

   Clique em **[!UICONTROL Salvar]**.

1. Faça logon no Brand Portal com as credenciais do usuário que você removeu da lista compartilhada. A coleção é removida do console **[!UICONTROL Coleções]**.
