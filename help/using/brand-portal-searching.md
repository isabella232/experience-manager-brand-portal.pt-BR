---
title: Pesquisar ativos no Brand Portal
seo-title: Pesquisa de ativos e pesquisa salva no Portal de marcas do AEM
description: O recurso de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o omnisearch, e os filtros de pesquisa ajudam você a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
seo-description: O recurso de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o omnisearch, e os filtros de pesquisa ajudam você a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
uuid: c 2955198-bdc 0-4853-a 13 a -661 e 6 a 9 ec 61 f
contentOwner: bdhar
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Pesquisar ativos no Brand Portal {#search-assets-on-brand-portal}

[!DNL Brand Portal] o recurso de pesquisa permite pesquisar rapidamente ativos relevantes usando o omnisearch e a pesquisa facetada que usa filtros para ajudar você a restringir ainda mais sua pesquisa. Você também pode salvar suas pesquisas como [!UICONTROL coleções inteligentes] para o futuro.

## Pesquisar ativos usando o Omnisearch {#search-assets-using-omnisearch}

Para pesquisar ativos em [!DNL Brand Portal]:

1. Na barra de ferramentas, clique no **ícone Pesquisar** ou pressione a tecla "**/**" para iniciar o Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. Na caixa de pesquisa, digite uma palavra-chave para os ativos que deseja pesquisar.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Pelo menos dois caracteres são necessários na omnisearch para que sugestões de pesquisa apareçam.

3. Selecione uma das sugestões relacionadas que aparecem na lista suspensa para acessar rapidamente os ativos relevantes.

   ![](assets/assets-search-result.png)

   Pesquisa de ativos usando o omnisearch

## Pesquisar usando facetas no painel Filtros {#search-using-facets-in-filters-panel}

As facetas de pesquisa no painel Filtros adicionam granularidade à experiência de pesquisa e tornam a funcionalidade de pesquisa eficiente. As facetas de pesquisa usam várias dimensões (previsões) que permitem executar pesquisas avançadas. Você pode detalhar facilmente o nível de detalhes desejado para uma pesquisa mais focada.

Por exemplo, se estiver procurando por uma imagem, você pode escolher se deseja um bitmap ou uma imagem vetorial. Você pode reduzir ainda mais o escopo da pesquisa especificando o tipo MIME para a imagem na faceta de pesquisa Tipo de arquivo. Da mesma forma, ao pesquisar documentos, você pode especificar o formato, por exemplo, formato PDF ou MS Word.

![Painel Filtros no [!DNL Brand Portal]](assets/file-type-search.png "painel Filtros em [! DNL Brand Portal]")

O painel Filtros inclui alguns aspectos padrão, como Navegador de caminho, Tipo de arquivo, Tamanho de arquivo, Status e Orientação. No entanto, você [pode adicionar aspectos](../using/brand-portal-search-facets.md) de pesquisa personalizados ou remover aspectos de pesquisa específicos do painel **Filtros** adicionando ou removendo previsões no Formulário de pesquisa subjacente. Consulte a lista de predicados [de pesquisa disponíveis e utilizáveis no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Para aplicar filtros à pesquisa, usando as facetas [de pesquisa disponíveis](../using/brand-portal-search-facets.md):

1. Clique no ícone de sobreposição e selecione **Filtro**.

   ![](assets/selectorrail.png)

2. No painel **Filtros** à esquerda, selecione as opções apropriadas para aplicar os filtros relevantes.
Por exemplo, use os seguintes filtros padrão:

   * **Navegador de caminhos** para pesquisar ativos em um diretório específico. O caminho de pesquisa padrão do predicado para Navegador de caminho é */content/dam/mac/ &lt; tenant-id &gt;/*, que pode ser configurado ao editar o formulário de pesquisa padrão.
   >[!NOTE]
   >
   >Para usuários não administradores, o Navegador de caminho no painel Filtro mostra apenas a estrutura de conteúdo das pastas (e as pastas ancestrais) compartilhadas com eles.\
   >Para usuários administradores, o Navegador de caminhos permite navegar para qualquer pasta no [!DNL Brand Portal].

   * **Tipo de arquivo** para especificar o tipo (imagem, documento, multimídia, arquivamento) do arquivo de ativos que você está procurando. Além disso, é possível restringir o escopo da pesquisa, por exemplo, especificar o tipo MIME (Tiff, Bitmap, GIMP Images) para a imagem ou o formato (PDF ou MS Word) dos documentos.
   * **Tamanho** do arquivo para pesquisar ativos com base em seu tamanho. Você pode especificar os limites inferiores e superiores para o intervalo de tamanho para restringir sua pesquisa e especificar a unidade de medida a ser pesquisada.
   * **Status** para pesquisar ativos com base em status de ativos, como Aprovação (Aprovado, Alterações solicitadas, Rejeitada, Pendente) e Expiração.
   * **Classificação** média para pesquisar ativos com base na classificação dos ativos.
   * **Orientação** para pesquisar ativos com base na orientação (horizontal, vertical, quadrado) dos ativos.
   * **Estilo** para pesquisar ativos com base no estilo (colorido, monocromático) dos ativos.
   * **Formato de vídeo** para pesquisar ativos de vídeo com base em seu formato (DVI, Flash, MPEG 4, MPEG, OGG Theora, quicktime, Windows Media, webm).
   Você pode usar [aspectos de pesquisa personalizados](../using/brand-portal-search-facets.md) no painel Filtros editando o Formulário de pesquisa subjacente.

   * **Predicado de propriedade** se usado no formulário de pesquisa permite pesquisar ativos que correspondam a uma propriedade de metadados para a qual o predicado é mapeado.\
      Por exemplo, se o Predicado de propriedade estiver mapeado para `jcr:content /metadata/dc:title`, você pode pesquisar ativos com base em seu título.\
      O Predicado de propriedade suporta pesquisas de texto por:

      **Frases parciais**
Para permitir a pesquisa do ativo usando frases parciais no predicado da propriedade, maque a caixa de seleção **Pesquisa parcial** em Pesquisar formulário.\
      Isso permite pesquisar pelos ativos desejados mesmo que não especifique as palavras/frases exatas usadas nos metadados do ativo.\
      Você pode:
* Especifique uma palavra que ocorre na sua frase pesquisada na faceta no painel Filtros. For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **climb** in their title phrase are returned.
* Especificar uma parte da palavra, que ocorre na frase pesquisada, juntamente com o caracter curinga (*) para preencher as lacunas.
Por exemplo, pesquisando por:
      **escalada *** retorna todos os ativos que têm palavras que começam com os caracteres "escalada" em sua frase de título.
      *** escalada** retorna todos os ativos que têm palavras terminando com caracteres "escalada" em sua frase de título.
      *** escalada *** retorna todos os ativos com palavras que incluem os caracteres "escalada" na frase de título.\
      **Texto
que não diferencia maiúsculas de minúsculas** Para permitir a pesquisa sem maiúsculas e minúsculas no predicado da propriedade, ative a **caixa de seleção Ignorar caso** no Formulário Pesquisar. Por padrão, a pesquisa de texto em predicado de propriedade diferencia maiúsculas e minúsculas.
   >[!NOTE]
   >
   >Ao selecionar **a caixa de seleção Pesquisa** parcial, **Ignorar caso** está selecionado por padrão.

   ![](assets/wildcard-prop-1.png)

   Os resultados da pesquisa são exibidos de acordo com os filtros aplicados, juntamente com a contagem de resultados da pesquisa.

   ![](assets/omnisearch-with-filters.png)

   Resultado da pesquisa do ativo com contagem de resultados de pesquisa

3. Você pode navegar facilmente para um item do resultado da pesquisa e retornar para o mesmo resultado de pesquisa usando o botão Voltar no navegador sem precisar executar novamente a consulta de pesquisa.

## Salvar suas pesquisas como uma coleção inteligente {#save-your-searches-as-smart-collection}

Você pode salvar as configurações de pesquisa como uma coleção inteligente para poder repetir rapidamente a mesma pesquisa sem precisar refazer as mesmas configurações posteriormente.

Para salvar as configurações de pesquisa como uma coleção inteligente:

1. Toque/clique **em Salvar coleção inteligente** e forneça um nome para a coleção inteligente.

   Para tornar a coleção inteligente acessível a todos os usuários, selecione **Público**. Uma mensagem confirma que a coleção inteligente foi criada e adicionada à lista de suas pesquisas salvas.

   >[!NOTE]
   >
   >Usuários não administradores podem ser limitados a tornar as [!UICONTROL coleções inteligentes] públicas, a fim de evitar ter um grande número de coleções inteligentes [!UICONTROL públicas] criadas por usuários não administradores na organização [!DNL Brand Portal]. As organizações podem desativar a configuração **de criação de[!UICONTROL coleções]inteligentes** públicas de configurações **Gerais** disponíveis no painel de ferramentas administrativas.

   ![](assets/save_smartcollectionui.png)

1. Para salvar a coleção inteligente com um nome diferente e selecionar ou desmarcar a caixa **de** seleção Público, clique **em Editar coleção inteligente**.

   ![](assets/edit_smartcollection.png)

1. Na caixa de diálogo **Editar coleção** inteligente, selecione **Salvar como** e insira um nome para a coleção inteligente. Clique em **Salvar**.

   ![](assets/saveas_smartsearch.png)
