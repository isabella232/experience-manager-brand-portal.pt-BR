---
title: Publicar predefinições, esquema e aspectos no Brand Portal
seo-title: Publicar predefinições, esquema e aspectos no Brand Portal
description: Saiba como publicar predefinições, schemas e aspectos no Brand Portal.
seo-description: Saiba como publicar predefinições, schemas e aspectos no Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 3%

---


# Publicar predefinições, esquema e aspectos no Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

O artigo se aprofunda em predefinições de imagens de publicação, schemas de metadados e aspectos de pesquisa personalizados da instância do autor de AEM para o Portal de marcas. O recurso de publicação permite que as organizações reutilizem predefinições de imagens, schemas de metadados e aspectos de pesquisa criados/modificados na instância do autor de AEM, reduzindo assim os esforços dos duplicados.

>[!NOTE]
>
>A capacidade de publicar predefinições de imagens, schema de metadados e aspectos de pesquisa da instância do autor de AEM para o Portal de marcas está disponível AEM 6.2 SP1-CFP7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1) em diante.

## Publicar predefinições de imagens no Brand Portal {#publish-image-presets-to-brand-portal}

As predefinições de imagens são um conjunto de comandos de dimensionamento e formatação aplicados à imagem no momento do delivery de imagem. As predefinições de imagens podem ser criadas e modificadas no Brand Portal. Como alternativa, se a instância do autor de AEM estiver sendo executada no modo de mídia dinâmica, os usuários poderão criar predefinições no autor de AEM e publicá-las no portal de marcas da AEM Assets e evitar a recriação das mesmas predefinições no Portal de marcas.\
Depois que a predefinição é criada, ela é listada como representação dinâmica no painel de representações detalhadas do ativo e na caixa de diálogo de download.

>[!NOTE]
>
>Se a instância do autor de AEM não estiver sendo executada no **[!UICONTROL Modo de Mídia Dinâmica]** (o cliente não comprou Mídia Dinâmica), a renderização **[!UICONTROL TIFF da pirâmide]** dos ativos não será criada no momento do upload. As predefinições de imagens ou representações dinâmicas funcionam em **[!UICONTROL TIFF de pirâmide]** de um ativo, portanto, se **[!UICONTROL TIFF de pirâmide]** não estiver disponível na instância do autor de AEM, ele também não estará disponível no Portal de marcas. Como resultado, nenhuma representação dinâmica está presente no painel de representações da página de detalhes do ativo e na caixa de diálogo de download.

Para publicar predefinições de imagens no Brand Portal:

1. Na instância do autor de AEM, toque/ clique no logotipo AEM para acessar o console de navegação global e toque/ clique no ícone Ferramentas e navegue até **[!UICONTROL Ativos > Predefinições de imagem]**.
1. Selecione a predefinição de imagem ou várias predefinições de imagem na lista de predefinições de imagem e clique/ toque em **[!UICONTROL Publicar no Portal de Marca]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando os usuários clicam em **[!UICONTROL Publicar no Brand Portal]**, as predefinições de imagem são enfileiradas para publicação. Os usuários são aconselhados a monitorar o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de uma predefinição de imagem no Portal de marcas:

1. Na instância do autor de AEM, toque/ clique no logotipo AEM para acessar o console de navegação global e toque/clique no ícone **[!UICONTROL Ferramentas]** e navegue até **[!UICONTROL Ativos > Predefinições de imagem]**.
1. Selecione uma predefinição de imagem e **[!UICONTROL Remover do Portal de Marcas]** nas opções disponíveis na parte superior.

## Publicar schema de metadados no Brand Portal {#publish-metadata-schema-to-brand-portal}

O schema de metadados descreve o layout e as propriedades que são exibidas na página de propriedades do ativo/ coleções.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se os usuários tiverem editado o schema padrão na instância do autor de AEM e estiverem dispostos a usar o mesmo schema como schema padrão no Portal de Marcas, eles poderão simplesmente publicar os formulários de schema de metadados no Portal de Marcas. Nesse cenário, o schema padrão no Brand Portal é substituído pelos schemas padrão publicados na instância do autor de AEM.

Se os usuários criarem um schema personalizado na instância do autor de AEM, poderão publicar o schema personalizado no Portal de marcas em vez de recriar o mesmo schema personalizado. Os usuários podem aplicar esse schema personalizado a qualquer pasta/coleção no Brand Portal.

>[!NOTE]
>
>Os schemas padrão não podem ser publicados no Brand Portal se estiverem bloqueados na instância AEM (ou seja, se não estiverem editados).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se uma pasta tiver um schema aplicado na instância do autor de AEM, o mesmo schema também deverá existir no Portal de marcas para manter a consistência na página de propriedades do ativo no AEM Author and Brand Portal.

Para publicar um schema de metadados da instância do autor de AEM no Portal de marcas:

1. Na instância do autor de AEM, toque/ clique no logotipo AEM para acessar o console de navegação global e toque/clique no ícone Ferramentas e navegue até **[!UICONTROL Ativos > Schemas de metadados]**.
1. Selecione um schema de metadados e **[!UICONTROL Publicar no Brand Portal]** nas opções disponíveis na parte superior.

>[!NOTE]
>
>Quando os usuários clicam em **[!UICONTROL Publicar no Brand Portal]**, os schemas de metadados são enfileirados para publicação. Os usuários são aconselhados a monitorar o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de um schema de metadados do Portal de marcas:

1. Na instância do autor de AEM, toque/ clique no logotipo AEM para acessar o console de navegação global e toque/clique no ícone Ferramentas e navegue até **[!UICONTROL Ativos > Schemas de metadados]**.
1. Selecione um schema de metadados e **[!UICONTROL Remover do Portal de Marcas]** nas opções disponíveis na parte superior.

## Publicar aspectos de pesquisa no Brand Portal {#publish-search-facets-to-brand-portal}

Os formulários de pesquisa fornecem a capacidade de [pesquisa facetada](../using/brand-portal-search-facets.md) aos usuários no Brand Portal. Os aspectos de pesquisa fornecem maior granularidade para pesquisas no Brand Portal. Todos os predicados [adicionados](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) no formulário de pesquisa estão disponíveis para os usuários como aspectos de pesquisa em filtros de pesquisa.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se você estiver disposto a usar o formulário de pesquisa personalizado **[!UICONTROL Painel de pesquisa do administrador de ativos]** da instância do autor de AEM, em vez de recriar o mesmo formulário no Portal de marcas, poderá publicar o formulário de pesquisa personalizado da instância do autor de AEM para o Portal de marcas.

>[!NOTE]
>
>O formulário de pesquisa bloqueado **[!UICONTROL Painel de pesquisa do administrador do Assets]** no AEM Assets não pode ser publicado no Portal da marca, a menos que seja editado. Depois de editado e publicado no Brand Portal, esse formulário de pesquisa substitui o formulário de pesquisa no Brand Portal.

Para publicar o aspecto de pesquisa editado da instância do autor de AEM no Portal de marcas:

1. Toque/clique no logotipo do AEM e acesse **[!UICONTROL Ferramentas > Geral > Pesquisar formulários]**.
1. Selecione o formulário de pesquisa editado e **[!UICONTROL Publicar no Brand Portal]**.

   >[!NOTE]
   >
   >Quando os usuários clicam em **[!UICONTROL Publicar no Brand Portal]**, os aspectos de pesquisa são enfileirados para publicação. Os usuários devem monitorar o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de formulários de pesquisa no Portal de marcas:

1. Na instância do autor de AEM, toque/ clique no logotipo AEM para acessar o console de navegação global e toque/clique no ícone Ferramentas e navegue até **[!UICONTROL Geral > Pesquisar Forms]**.
1. Selecione o formulário de pesquisa e selecione **[!UICONTROL Remover do Brand Portal]** a partir das opções disponíveis na parte superior.

>[!NOTE]
>
>A ação **[!UICONTROL Cancelar a publicação do Brand Portal]** deixa o formulário de pesquisa padrão no Brand Portal e não restaura para o último formulário de pesquisa usado antes da publicação.

### Limitações           {#limitations}

1. Poucos predicados de pesquisa não se aplicam a filtros de pesquisa no Portal de Marcas. Quando esses predicados de pesquisa são publicados como parte do formulário de pesquisa da instância do autor de AEM para o Portal de marcas, eles são filtrados. Os usuários, portanto, veem um número menor de predicados no formulário publicado no Brand Portal. Consulte [predicados de pesquisa aplicáveis a filtros no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Para [!UICONTROL Predicado de opções], se um usuário estiver usando qualquer caminho personalizado para ler opções na instância do autor de AEM, ele não funcionará no Portal de marcas. Esses caminhos e opções adicionais não são publicados no Brand Portal com o formulário de pesquisa. Nesse caso, os usuários podem selecionar a opção **[!UICONTROL Manual]** em **[!UICONTROL Adicionar opções]** em **[!UICONTROL Predicado de opções]** para adicionar essas opções manualmente no Brand Portal.

![](assets/options-predicate-manual.png)
