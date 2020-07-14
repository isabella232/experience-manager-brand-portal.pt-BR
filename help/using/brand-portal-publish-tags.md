---
title: Publicar marcações no Brand Portal
seo-title: Publicar marcações no Brand Portal
description: Saiba como publicar tags de AEM Assets para o Brand Portal.
seo-description: Saiba como publicar tags de AEM Assets para o Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# Publicar marcações no Brand Portal {#publish-tags-to-brand-portal}

Saiba como publicar tags de AEM Assets para o Brand Portal.

As tags são úteis na organização de ativos e aprimoram a capacidade de pesquisa de ativos aos quais estão associadas. As tags podem ser consideradas palavras-chave ou rótulos (metadados) anexados aos ativos e permitem que os ativos sejam encontrados rapidamente como resultado de uma pesquisa. Para saber como atribuir tags a ativos em AEM Assets, consulte [usar tags para organizar ativos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

As tags (associadas aos ativos e coleções no AEM) são publicadas automaticamente no Brand Portal quando os ativos (e coleções) com tags associadas são publicados no Brand Portal. As tags publicadas são úteis para permitir que as pesquisas localizem os ativos associados.

>[!NOTE]
>
>No entanto, é recomendável publicar tags exclusivamente no Brand Portal antes de publicar os ativos (e coleções) com os quais as tags estão associadas. Isso garante a publicação mais rápida dos ativos (e das coleções) no Brand Portal.

## Manage tags {#manage-tags}

Você pode usar as tags pré-existentes para anexar a um ativo ou criar novas tags no console Tags do AEM (**[!UICONTROL Ferramentas | Marcação | Tags]** AEM). Em ambos os cenários, você deve primeiro publicar as tags no Brand Portal e associá-las aos ativos apropriados.

Para criar tags no AEM, publicar as tags no Brand Portal e associar as tags aos ativos apropriados (ou coleções), siga estas etapas:

1. **Criar tags** Faça logon na instância AEM Author com privilégios administrativos e acesse o console de tags **[!UICONTROL do]** AEM a partir da navegação global:

   1. Selecionar **[!UICONTROL ferramentas]**

   1. Selecionar **[!UICONTROL Geral]**

   1. Selecionar **[!UICONTROL marcação]**

1. Selecione **[!UICONTROL Criar]** e selecione a opção **[!UICONTROL Criar tag]** .
1. Especificar:

   * **[!UICONTROL Título]**

      *(obrigatório)* Um título de exibição para a tag.
   * **[!UICONTROL Nome]**
      *(obrigatório)* Um nome para a tag. Se não for especificado, um nome de nó válido será criado a partir do Título. Consulte [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descrição**

      *(opcional)* Uma descrição da tag.
   * **Caminho da tag Caminho** JCR caminho da tag .

1. Selecione **[!UICONTROL Enviar]** para criar a tag .

   Depois de criar uma tag na instância do AEM, ela estará disponível para ser anexada a um ativo (usando a seção Propriedades ou a seção Gerenciar tags desse ativo).

1. **Publique a tag no Brand Portal**.

   Ir para o console **[!UICONTROL Tags]** do AEM ([!UICONTROL Ferramentas) | Marcação | Tags]de AEM), selecione a tag desejada e publique no Portal de marcas.

1. **Anexe a tag a um ativo (ou coleção)**.

   Selecione um ativo (ou coleção) e anexe a tag desejada usando a seção Propriedades ou a seção Gerenciar tags desse ativo. Para saber mais sobre como atribuir tags a ativos em AEM Assets, consulte [usar tags para organizar ativos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Publique ativos (ou coleções) no Brand Portal**.\
   Quando você publica um ativo (ou uma coleção) no Brand Portal, a tag anexada também está disponível no Brand Portal.

   Para ver a tag anexada no respectivo ativo (ou coleção) no Brand Portal, faça logon no Brand Portal e selecione o ativo, na seção Propriedades, você verá a tag anexada.

## Pesquisar Promover {#search-promote}

O Portal de marcas do AEM Assets permite que você faça com que ativos específicos sejam os principais resultados de pesquisas com base em uma tag de palavra-chave.

Para elevar um ativo para uma palavra-chave de pesquisa, siga estas etapas:

1. Abra a página **[!UICONTROL Propriedades]** de um ativo na instância do autor de AEM.
1. Vá para a guia **[!UICONTROL Avançado]** .
1. Na seção **[!UICONTROL Pesquisar promoção]** em **[!UICONTROL Elevar para palavras-chave]** de pesquisa, selecione **[!UICONTROL Adicionar]** para adicionar as palavras-chave ou tags de pesquisa.

   ![](assets/search-promote.png)

1. Salve as alterações.
1. Publicar o ativo no Brand Portal.
1. Faça logon no Brand Portal. Guia **[!UICONTROL Avançado]** de Visualização na seção **[!UICONTROL Propriedades]** do ativo.
Observe que a palavra-chave **[!UICONTROL Search Promote]** também está visível nas Propriedades desse ativo.
