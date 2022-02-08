---
title: Buscar ativos no Brand Portal
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: O recurso de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o omnisearch, e os filtros de pesquisa ajudam a limitar ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: dc425522f134781b4420eb8643ee6ee65d98b6cc
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 7%

---

# Buscar ativos no Brand Portal {#search-assets-on-brand-portal}

O recurso de pesquisa do Brand Portal permite pesquisar rapidamente ativos relevantes usando o omnisearch e a pesquisa de faceta que usa filtros para ajudá-lo a restringir ainda mais sua pesquisa. Você pode pesquisar ativos em arquivos ou pastas e salvar seus resultados de pesquisa como coleções inteligentes. No entanto, não é possível pesquisar ativos de uma coleção usando pesquisa omnisearch ou facet.

## Pesquisar ativos usando o Omnisearch {#search-assets-using-omnisearch}

Para pesquisar ativos no Brand Portal:

1. Na barra de ferramentas, clique no botão **[!UICONTROL Pesquisar]** ou pressione o botão **[!UICONTROL /]**&quot; chave para iniciar o Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Na caixa de pesquisa, digite uma palavra-chave para os ativos que deseja pesquisar.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >São necessários pelo menos 3 caracteres no omnisearch para que sugestões de pesquisa sejam exibidas.

1. Selecione entre as sugestões relacionadas que aparecem na lista suspensa para acessar rapidamente os ativos relevantes.

   ![](assets/assets-search-result.png)

   *Pesquisa de ativos usando o omnisearch*

Para saber mais sobre o comportamento de pesquisa com ativos marcados inteligentes, consulte [entender os resultados e o comportamento da pesquisa](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## Pesquisar usando aspectos no painel Filtros {#search-using-facets-in-filters-panel}

Os aspectos de pesquisa no painel Filtros adicionam granularidade à sua experiência de pesquisa e tornam a funcionalidade de pesquisa eficiente. Os aspectos de pesquisa usam várias dimensões (predicados) que permitem executar pesquisas complexas. Você pode detalhar facilmente até o nível de detalhes desejado para uma pesquisa mais focada.

Por exemplo, se estiver procurando uma imagem, você pode escolher se deseja um bitmap ou uma imagem vetorial. Você pode reduzir ainda mais o escopo da pesquisa especificando o tipo MIME da imagem na faceta de pesquisa Tipo de arquivo . Da mesma forma, ao pesquisar documentos, é possível especificar o formato, por exemplo, PDF ou MS Word.

![Painel Filtros no Brand Portal](assets/file-type-search.png "Painel Filtros no Brand Portal")

O **[!UICONTROL Filtros]** O painel inclui algumas facetas padrão, como **[!UICONTROL Navegador de caminhos]**, **[!UICONTROL Tipo de arquivo]**, **[!UICONTROL Tamanho do arquivo]**, **[!UICONTROL Status]** e **[!UICONTROL Orientação]**. No entanto, é possível [adicionar aspectos de pesquisa personalizados](../using/brand-portal-search-facets.md) ou remover aspectos de pesquisa específicos da **[!UICONTROL Filtros]** adicionando ou removendo predicados no Formulário de pesquisa subjacente. Veja a lista de [predicados de pesquisa no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Para aplicar filtros à sua pesquisa, use o [aspectos de pesquisa](../using/brand-portal-search-facets.md):

1. Clique no ícone de sobreposição e selecione **[!UICONTROL Filtro]**.

   ![](assets/selectorrail.png)

1. No **[!UICONTROL Filtros]** à esquerda, selecione as opções apropriadas para aplicar os filtros relevantes.
Por exemplo, use os seguintes filtros padrão:

   * **[!UICONTROL Navegador de caminhos]** para pesquisar ativos em um diretório específico. O caminho de pesquisa padrão do predicado para Navegador de caminhos é `/content/dam/mac/<tenant-id>/`, que pode ser configurado ao editar o formulário de pesquisa padrão.
   >[!NOTE]
   >
   >Para usuários não administradores, [!UICONTROL Navegador de caminhos] em [!UICONTROL Filtro] mostra somente a estrutura de conteúdo das pastas (e suas pastas ancestrais) compartilhadas com elas.\
   >Para administradores de usuários, o Navegador de caminhos permite navegar para qualquer pasta no Brand Portal.

   * **[!UICONTROL Tipo de arquivo]** para especificar o tipo (imagem, documento, multimídia, arquivo) do arquivo de ativos que você está procurando. Além disso, você pode limitar o escopo de sua pesquisa, por exemplo, especificar o tipo MIME (Tiff, Bitmap, GIMP Images) para imagem ou formato (PDF ou MS Word) para os documentos.
   * **[!UICONTROL Tamanho do arquivo]** para procurar ativos com base em seu tamanho. Você pode especificar os limites inferior e superior para o intervalo de tamanho para restringir sua pesquisa e especificar a unidade de medida a ser pesquisada.
   * **[!UICONTROL Status]** para pesquisar ativos com base em status de ativos, como Aprovação (Aprovada, Alterações Solicitadas, Rejeitada, Pendente) e Expiração.
   * **[!UICONTROL Classificação média]** procurar ativos com base na classificação dos ativos.
   * **[!UICONTROL Orientação]** para pesquisar ativos com base na orientação (horizontal, vertical, quadrada) dos ativos.
   * **[!UICONTROL Estilo]** para pesquisar ativos com base no estilo (colorido, monocromático) dos ativos.
   * **[!UICONTROL Formato de vídeo]** para pesquisar ativos de vídeo com base em seu formato (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   Você pode usar [aspectos de pesquisa personalizada](../using/brand-portal-search-facets.md) no painel Filtros, editando o Formulário de pesquisa subjacente.

   * **[!UICONTROL Predicado de propriedade]** se usado no formulário de pesquisa, permite pesquisar ativos que correspondem a uma propriedade de metadados para a qual o predicado é mapeado.\
      Por exemplo, se o Predicado de propriedade estiver mapeado para [!UICONTROL `jcr:content /metadata/dc:title`], você pode pesquisar ativos com base em seu título.\
      O [!UICONTROL Predicado de propriedade] O suporta pesquisas de texto para:

      **Frases parciais**
Para permitir a pesquisa do ativo usando frases parciais no predicado da propriedade, maque a caixa de seleção **[!UICONTROL Pesquisa parcial]** em Pesquisar formulário.\
      Isso permite pesquisar pelos ativos desejados mesmo que não especifique as palavras/frases exatas usadas nos metadados do ativo.\
      É possível:
      * Especifique uma palavra que ocorre na frase pesquisada na faceta no painel Filtros . Por exemplo, se você pesquisar pelo termo **subida** (e o Predicado de propriedade é mapeado para [!UICONTROL `dc:title`] ), em seguida, todos os ativos com a palavra **subida** na frase de título são retornadas.
      * Especificar uma parte da palavra, que ocorre na frase pesquisada, juntamente com o caracter curinga (*) para preencher as lacunas.
Por exemplo, pesquisando por:
         * **subida*** retorna todos os ativos que têm palavras começando com os caracteres &quot;climb&quot; na frase de título.
         * ***subida** retorna todos os ativos com palavras que terminam com caracteres &quot;climb&quot; em sua frase de título.
         * ***subida*** retorna todos os ativos com palavras que incluem os caracteres &quot;climb&quot; na frase de título.

Para permitir a pesquisa que não diferencia maiúsculas de minúsculas no predicado da propriedade, habilite a variável       **Texto sem diferenciação entre maiúsculas e minúsculas**
Para permitir a pesquisa que não diferencia maiúsculas de minúsculas no predicado da propriedade, habilite a variável **[!UICONTROL Ignorar maiúsculas e minúsculas]** caixa de seleção em Formulário de pesquisa. Por padrão, a pesquisa de texto no predicado de propriedade diferencia maiúsculas de minúsculas.
   >[!NOTE]
   >
   >Ao selecionar **[!UICONTROL Pesquisa parcial]** caixa de seleção, **[!UICONTROL Ignorar maiúsculas e minúsculas]** é selecionada por padrão.

   ![](assets/wildcard-prop-1.png)

   Os resultados da pesquisa são exibidos de acordo com os filtros aplicados, juntamente com a contagem dos resultados da pesquisa.

   ![](assets/omnisearch-with-filters.png)

   Resultado da pesquisa do ativo com a contagem dos resultados da pesquisa.

1. Você pode navegar facilmente para um item a partir do resultado da pesquisa e retornar para o mesmo resultado usando o botão Voltar em seu navegador, sem precisar executar a consulta de pesquisa novamente.

## Salvar suas pesquisas como coleção inteligente {#save-your-searches-as-smart-collection}

Você pode salvar as configurações de pesquisa como uma coleção inteligente para poder repetir rapidamente a mesma pesquisa sem precisar refazer as mesmas configurações posteriormente. No entanto, não é possível aplicar filtros de pesquisa em uma coleção.

Para salvar as configurações de pesquisa como uma coleção inteligente:

1. Toque/clique **[!UICONTROL Salvar coleção inteligente]** e forneça um nome para a coleção inteligente.

   Para tornar a coleção inteligente acessível a todos os usuários, selecione **[!UICONTROL Público]**. Uma mensagem confirma que a coleção inteligente foi criada e adicionada à lista de suas pesquisas salvas.

   >[!NOTE]
   >
   >Usuários não administradores podem ser impedidos de tornar coleções inteligentes públicas, para evitar um grande número de coleções inteligentes públicas criadas por usuários não administradores no Brand Portal da organização. As organizações podem desativar o **[!UICONTROL Permitir a criação de coleções inteligentes públicas]** configuração de **[!UICONTROL Geral]** configurações disponíveis no painel Ferramentas administrativas.

   ![](assets/save_smartcollectionui.png)

1. Para salvar a coleção inteligente em um nome diferente, selecione ou desmarque a variável **[!UICONTROL Público]** caixa de seleção, clique em **[!UICONTROL Editar coleção inteligente]**.

   ![](assets/edit_smartcollection.png)

1. No **[!UICONTROL Editar coleção inteligente]** caixa de diálogo, selecione **[!UICONTROL Salvar como]** e insira um nome para a coleção inteligente. Clique em **[!UICONTROL Salvar]**.

   ![](assets/saveas_smartsearch.png)
