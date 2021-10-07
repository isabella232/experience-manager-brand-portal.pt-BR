---
title: Publicar marcações no Brand Portal
seo-title: Publish tags to Brand Portal
description: Saiba como publicar tags do Experience Manager Assets para o Brand Portal.
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# Publicar marcações no Brand Portal {#publish-tags-to-brand-portal}

Saiba como publicar tags do Experience Manager Assets para o Brand Portal.

As tags são úteis na organização de ativos e aprimoram a capacidade de pesquisa de ativos aos quais estão associadas. As tags podem ser consideradas palavras-chave ou rótulos (metadados) anexados a ativos e permitem que os ativos sejam encontrados rapidamente como o resultado de uma pesquisa. Para saber como atribuir tags a ativos no Experience Manager Assets, consulte [usar tags para organizar ativos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

As tags (associadas aos ativos e coleções no AEM) são publicadas automaticamente no Brand Portal quando os ativos (e coleções) com as tags associadas são publicados no Brand Portal. As tags publicadas são úteis na ativação das pesquisas para localizar os ativos associados.

>[!NOTE]
>
>No entanto, é recomendável publicar tags exclusivamente no Brand Portal antes de publicar os ativos (e coleções) com os quais as tags estão associadas. Isso garante uma publicação mais rápida dos ativos (e das coleções) na Brand Portal.

## Gerenciar tags {#manage-tags}

Você pode usar as tags pré-existentes para anexar a um ativo ou criar novas tags AEM console Tags (**[!UICONTROL Ferramentas | Marcação | Tags de AEM]**). Em ambos os cenários, você deve primeiro publicar as tags na Brand Portal e associá-las aos ativos apropriados.

Para criar tags no AEM, publicar as tags no Brand Portal e associar as tags aos ativos apropriados (ou coleções), siga estas etapas:

1. **Criar**
tagsFaça logon na instância do autor do AEM com privilégios administrativos e acesse  **[!UICONTROL AEM console]** Tags na navegação global:

   1. Selecione **[!UICONTROL Ferramentas]**

   1. Selecione **[!UICONTROL Geral]**

   1. Selecione **[!UICONTROL Marcação]**

1. Selecione **[!UICONTROL Criar]** e selecione a opção **[!UICONTROL Criar tag]**.
1. Especifique:

   * **[!UICONTROL Título]**

      *(obrigatório)* Um título de exibição para a tag.
   * **[!UICONTROL Nome]**
      *(obrigatório)* Um nome para a tag. Se não especificado, um nome de nó válido é criado a partir do Título. Consulte [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **Descrição**

      *(opcional)* Uma descrição da tag.
   * **Marque o caminho**
PathJCR da tag.

1. Selecione **[!UICONTROL Enviar]** para criar a tag.

   Depois de criar uma tag AEM instância, a tag estará disponível para ser anexada a um ativo (usando a seção Propriedades ou a seção Gerenciar tags desse ativo).

1. **Publique a tag no Brand Portal**.

   Vá para o console **[!UICONTROL AEM Tags]** ([!UICONTROL Ferramentas | Marcação | Tags de AEM]), selecione a tag desejada e Publique no Brand Portal.

1. **Anexe a tag a um ativo (ou coleção)**.

   Selecione um ativo (ou coleção) e anexe a tag desejada usando a seção Propriedades ou a seção Gerenciar tags desse ativo. Para saber mais sobre como atribuir tags a ativos no AEM Assets, consulte [usar tags para organizar ativos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **Publicar ativos (ou coleções) no Brand Portal**.\
   Ao publicar um ativo (ou coleção) no Brand Portal, a tag anexada também está disponível no Brand Portal.

   Para ver a tag anexada no respectivo ativo (ou coleção) no Brand Portal, faça logon no Brand Portal e selecione o ativo, na seção Propriedades, você verá a Tag anexada.

## Pesquisar Promover {#search-promote}

O AEM Assets Brand Portal permite que você faça com que ativos específicos sejam fornecidos como os principais resultados das pesquisas com base em uma tag de palavra-chave.

Para elevar um ativo para uma palavra-chave de pesquisa, siga estas etapas:

1. Abra a página **[!UICONTROL Propriedades]** de um ativo AEM instância do autor.
1. Vá para a guia **[!UICONTROL Advanced]**.
1. Em **[!UICONTROL Pesquisar Forçar]** na seção **[!UICONTROL Elevar para palavras-chave de pesquisa]**, selecione **[!UICONTROL Adicionar]** para adicionar as palavras-chave de pesquisa ou tags.

   ![](assets/search-promote.png)

1. Salve as alterações.
1. Publicar o ativo no Brand Portal.
1. Faça logon no Brand Portal. Exiba a guia **[!UICONTROL Avançado]** na seção **[!UICONTROL Propriedades]** do ativo.
Observe que a palavra-chave **[!UICONTROL Promover de pesquisa]** também está visível nas Propriedades desse ativo.
