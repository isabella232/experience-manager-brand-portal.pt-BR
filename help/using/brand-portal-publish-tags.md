---
title: Publicar marcações no Brand Portal
seo-title: Publish tags to Brand Portal
description: Saiba como publicar tags do Experience Manager Assets na Brand Portal.
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

Saiba como publicar tags do Experience Manager Assets na Brand Portal.

As tags são úteis na organização de ativos e melhoram a capacidade de pesquisa dos ativos aos quais estão associadas. As tags podem ser consideradas palavras-chave ou rótulos (metadados) anexados a ativos, que permitem que os ativos sejam rapidamente encontrados como resultado de uma pesquisa. Para saber como atribuir tags a ativos no Experience Manager Assets, consulte [usar tags para organizar ativos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

As tags (associadas a ativos e coleções no AEM) são publicadas automaticamente na Brand Portal quando os ativos (e coleções) com tags associadas são publicados no Brand Portal. As tags publicadas são úteis para permitir que as pesquisas localizem os ativos associados.

>[!NOTE]
>
>No entanto, é recomendável publicar tags exclusivamente no Brand Portal antes de publicar os ativos (e coleções) aos quais as tags estão associadas. Isso garante uma publicação mais rápida dos ativos (e coleções) no Brand Portal.

## Gerenciar tags {#manage-tags}

Você pode usar as tags pré-existentes para anexar a um ativo ou criar novas tags pelo console Tags do AEM (**[!UICONTROL Ferramentas | Marcação com tags | Tags do AEM]**). Em ambos os cenários, primeiro publique as tags na Brand Portal e, em seguida, associe-as aos ativos apropriados.

Para criar tags no AEM, publicar as tags no Brand Portal e associá-las aos ativos (ou coleções) apropriados, siga estas etapas:

1. **Criar tags**
Faça logon na instância do AEM Author com privilégios administrativos e acesso **[!UICONTROL Tags do AEM]** do console de navegação global:

   1. Selecionar **[!UICONTROL Ferramentas]**

   1. Selecionar **[!UICONTROL Geral]**

   1. Selecionar **[!UICONTROL Marcação]**

1. Selecionar **[!UICONTROL Criar]** e selecione **[!UICONTROL Criar tag]** opção.
1. Especifique:

   * **[!UICONTROL Título]**

      *(obrigatório)* Um título de exibição para a tag.
   * **[!UICONTROL Nome]**
      *(obrigatório)* Um nome para a tag. Se não for especificado, um nome de nó válido será criado a partir do Título. Consulte [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **Descrição**

      *(opcional)* Uma descrição da tag.
   * **Caminho da tag**
Caminho JCR da tag.

1. Selecionar **[!UICONTROL Enviar]** para criar a tag.

   Depois de criar uma tag na instância do AEM, a tag estará disponível para ser anexada a um ativo (usando a seção Propriedades ou a seção Gerenciar tags desse ativo).

1. **Publicar a tag no Brand Portal**.

   Ir para **[!UICONTROL Tags do AEM]** console ([!UICONTROL Ferramentas | Marcação com tags | Tags do AEM]), selecione a tag desejada e Publicar na Brand Portal.

1. **Anexar a tag a um ativo (ou coleção)**.

   Selecione um ativo (ou coleção) e anexe a tag desejada usando a seção Propriedades ou a seção Gerenciar tags desse ativo. Para saber mais sobre como atribuir tags a ativos no AEM Assets, consulte [usar tags para organizar ativos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **Publicar ativos (ou coleções) no Brand Portal**.\
   Ao publicar um ativo (ou coleção) no Brand Portal, a tag anexada também está disponível no Brand Portal.

   Para ver a tag anexada no respectivo ativo (ou coleção) no Brand Portal, faça logon no Brand Portal e selecione o ativo. Na seção Propriedades, você verá a tag anexada.

## Pesquisar Promover {#search-promote}

O AEM Assets Brand Portal permite fazer com que ativos específicos cheguem como os principais resultados de pesquisas baseadas em uma tag de palavra-chave.

Para elevar um ativo a uma palavra-chave de pesquisa, siga estas etapas:

1. Abra o **[!UICONTROL Propriedades]** página de um ativo na instância do autor do AEM.
1. Ir para **[!UICONTROL Avançado]** guia.
1. Entrada **[!UICONTROL Pesquisar Promover]** no prazo de **[!UICONTROL Elevar para palavras-chave de pesquisa]** , selecione **[!UICONTROL Adicionar]** para adicionar palavras-chave ou tags de pesquisa.

   ![](assets/search-promote.png)

1. Salve as alterações.
1. Publicar o ativo no Brand Portal.
1. Faça logon no Brand Portal. Exibir **[!UICONTROL Avançado]** guia em **[!UICONTROL Propriedades]** do ativo.
Observe que **[!UICONTROL Pesquisar Promover]** A palavra-chave também está visível nas Propriedades desse ativo.
