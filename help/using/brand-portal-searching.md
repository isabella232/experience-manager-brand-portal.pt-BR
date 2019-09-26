---
title: Pesquisar ativos no Brand Portal
seo-title: Pesquisa de ativos e pesquisa salva no AEM Brand Portal
description: A capacidade de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o Omnisearch, e os filtros de pesquisa ajudam a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
seo-description: A capacidade de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o Omnisearch, e os filtros de pesquisa ajudam a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: referência
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 201ca4c0df9016929d63b4f41f570903a59f7ebf

---


# Pesquisar ativos no Brand Portal {#search-assets-on-brand-portal}

A capacidade de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o Omnisearch e a pesquisa facetada que usa filtros para ajudar a restringir ainda mais sua pesquisa. Você também pode salvar suas pesquisas como coleções inteligentes para o futuro.

## Pesquisar ativos usando o Omnisearch {#search-assets-using-omnisearch}

Para pesquisar ativos no Brand Portal:

1. Na barra de ferramentas, clique no ícone **[!UICONTROL Pesquisar]** ou pressione a tecla "**[!UICONTROL /]**" para iniciar o Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Na caixa de pesquisa, digite uma palavra-chave para os ativos que deseja pesquisar.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >São necessários pelo menos 3 caracteres no Omnisearch para que sugestões de pesquisa sejam exibidas.

1. Selecione uma das sugestões relacionadas que aparecem na lista suspensa para acessar rapidamente os ativos relevantes.

   ![](assets/assets-search-result.png)

   *Pesquisa de ativos usando o omnisearch*

Para saber mais sobre o comportamento da pesquisa com ativos marcados inteligentes, consulte [entender os resultados e o comportamento](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)da pesquisa.

## Pesquisar usando aspectos no painel Filtros {#search-using-facets-in-filters-panel}

Os aspectos de pesquisa no painel Filtros adicionam granularidade à sua experiência de pesquisa e tornam a funcionalidade de pesquisa eficiente. Os aspectos de pesquisa usam várias dimensões (predicados) que permitem executar pesquisas complexas. É possível detalhar facilmente para o nível de detalhes desejado para uma pesquisa mais focada.

Por exemplo, se você estiver procurando uma imagem, poderá escolher se deseja um bitmap ou uma imagem vetorial. Você pode reduzir ainda mais o escopo da pesquisa especificando o tipo MIME da imagem na faceta de pesquisa Tipo de arquivo. Da mesma forma, ao pesquisar documentos, você pode especificar o formato, por exemplo, PDF ou MS Word.

![Filters panel in Brand Portal](assets/file-type-search.png "Filters panel in Brand Portal")

O painel [!UICONTROL Filtros] inclui algumas facetas padrão, como - Navegador [!UICONTROL de]caminho, Tipo de arquivo, Tamanho de arquivo, [!UICONTROL Status]e Orientação. However, you can [add custom search facets](../using/brand-portal-search-facets.md) or remove specific search facets from the [!UICONTROL Filters] panel by adding or removing predicates in the underlying Search Form. See the list of the available and usable search predicates on Brand Portal.[](../using/brand-portal-search-facets.md#list-of-search-predicates)

To apply filters to your search, using the available search facets:[](../using/brand-portal-search-facets.md)

1. Click the overlay icon and select **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

2. From the **[!UICONTROL Filters]** panel on the left, select the appropriate options to apply the relevant filters.
For example, use the following standard filters:

   * **[!UICONTROL Path Browser]** to search assets in a specific directory. O caminho de pesquisa padrão do predicado para o navegador de caminho é **[!UICONTROL /content/dam/mac/&lt;locatário-id&gt;/]**, que pode ser configurado editando o formulário de pesquisa padrão.
   >[!NOTE]
   >
   >To non-admin users, Path Browser in Filter panel shows only the content structure of the folders (and their ancestor folders) shared with them.\
   >To admin users, Path Browser allows navigating to any folder in Brand Portal.

   * **[!UICONTROL File Type to specify the type (image, document, multimedia, archive) of asset file you are looking for.]** Further, you can narrow down the scope of your search, for example, specify the MIME type (Tiff, Bitmap, GIMP Images) for image or format (PDF or MS Word) for the documents.
   * **[!UICONTROL File Size to search for assets based on their size.]** You can specify the lower and upper limits for the size range to narrow down your search and specify the unit of measure to search.
   * **[!UICONTROL Status]** para pesquisar ativos com base em status de ativos, como Aprovação (Aprovada, Alterações Solicitadas, Rejeitada, Pendente) e Expiração.
   * **[!UICONTROL Classificação]** média para procurar ativos com base na classificação dos ativos.
   * **[!UICONTROL Orientation to search for assets based on the orientation (horizontal, vertical, square) of the assets.]**
   * **[!UICONTROL Estilo]** para procurar ativos com base no estilo (colorido, monocromático) dos ativos.
   * **[!UICONTROL Formato]** de vídeo para pesquisar ativos de vídeo com base em seu formato (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   Você pode usar aspectos [de pesquisa](../using/brand-portal-search-facets.md) personalizados no painel Filtros editando o Formulário de pesquisa subjacente.

   * **[!UICONTROL O Predicado]** de propriedade, se usado no formulário de pesquisa, permite pesquisar ativos que correspondem a uma propriedade de metadados para a qual o predicado está mapeado.\
      Por exemplo, se o Predicado de propriedade estiver mapeado para [!UICONTROL `jcr:content /metadata/dc:title`], você poderá pesquisar ativos com base em seu título.\
      O Predicado de [!UICONTROL propriedades] oferece suporte a pesquisas de texto para:

      **Frases parciais**
Para permitir a pesquisa do ativo usando frases parciais no predicado da propriedade, maque a caixa de seleção **[!UICONTROL Pesquisa parcial]em Pesquisar formulário.**\
      Isso permite pesquisar pelos ativos desejados mesmo que não especifique as palavras/frases exatas usadas nos metadados do ativo.\
      You can:
* Specify a word occurring in your searched phrase in the facet in Filters panel. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* Especificar uma parte da palavra, que ocorre na frase pesquisada, juntamente com o caracter curinga (*) para preencher as lacunas.
Por exemplo, pesquisando por:
      **climb*** retorna todos os ativos com palavras que começam com os caracteres "escalar" em suas frases de título.
      ***climb** retorna todos os ativos que têm palavras que terminam com caracteres "escalam" em suas frases de título.
      ***climb*** retorna todos os ativos com palavras que incluem os caracteres "escalar" em suas frases de título.\
      **Texto** que não diferencia maiúsculas de minúsculas Para permitir uma pesquisa que não diferencia maiúsculas e minúsculas no predicado de propriedade, ative a caixa de seleção **[!UICONTROL Ignorar maiúsculas e minúsculas]** no Formulário de pesquisa. Por padrão, a pesquisa de texto no predicado de propriedade faz distinção entre maiúsculas e minúsculas.
   >[!NOTE]
   >
   >Ao marcar a caixa de seleção Pesquisa **** parcial, [!UICONTROL Ignorar caso] é selecionado por padrão.

   ![](assets/wildcard-prop-1.png)

   Os resultados da pesquisa são exibidos de acordo com os filtros aplicados, juntamente com a contagem dos resultados da pesquisa.

   ![](assets/omnisearch-with-filters.png)

   Resultado da pesquisa de ativos com contagem de resultados da pesquisa

3. Você pode navegar para um item facilmente a partir do resultado da pesquisa e retornar ao mesmo resultado da pesquisa usando o botão Voltar no seu navegador sem precisar executar novamente a consulta de pesquisa.

## Salvar suas pesquisas como coleção inteligente {#save-your-searches-as-smart-collection}

Você pode salvar as configurações de pesquisa como uma coleção inteligente para poder repetir rapidamente a mesma pesquisa sem precisar refazer as mesmas configurações posteriormente.

Para salvar as configurações de pesquisa como uma coleção inteligente:

1. Toque/ clique em **[!UICONTROL Salvar coleção]** inteligente e forneça um nome para a coleção inteligente.

   Para tornar a coleção inteligente acessível a todos os usuários, selecione **[!UICONTROL Público]**. Uma mensagem confirma que a coleção inteligente foi criada e adicionada à lista de suas pesquisas salvas.

   >[!NOTE]
   >
   >Os usuários não administradores podem ser restringidos de tornar públicas as coleções inteligentes, para evitar ter um grande número de coleções inteligentes públicas criadas por usuários não administradores no Portal de marcas da organização. As organizações podem desativar a configuração de criação **** Permitir coleções inteligentes públicas nas configurações **[!UICONTROL Gerais]** disponíveis no painel de ferramentas administrativas.

   ![](assets/save_smartcollectionui.png)

2. Para salvar a coleção inteligente em um nome diferente e marcar ou desmarcar a caixa de seleção **[!UICONTROL Público]** , clique em **[!UICONTROL Editar coleção]** inteligente.

   ![](assets/edit_smartcollection.png)

3. Na caixa de diálogo **[!UICONTROL Editar coleção]** inteligente, selecione **[!UICONTROL Salvar como]** e digite um nome para a coleção inteligente. Clique em **[!UICONTROL Salvar]**.

   ![](assets/saveas_smartsearch.png)
