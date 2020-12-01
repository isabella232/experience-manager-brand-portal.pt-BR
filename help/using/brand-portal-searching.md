---
title: Buscar ativos no Brand Portal
seo-title: Pesquisa de ativos e pesquisa salva no AEM Brand Portal
description: A capacidade de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o Omnisearch, e filtros de pesquisa ajudam a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
seo-description: A capacidade de pesquisa do Brand Portal permite que você pesquise rapidamente ativos relevantes usando o Omnisearch, e filtros de pesquisa ajudam a restringir ainda mais sua pesquisa. Salve suas pesquisas como coleções inteligentes para o futuro.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 7%

---


# Buscar ativos no Brand Portal {#search-assets-on-brand-portal}

O recurso de pesquisa do Brand Portal permite que você pesquise rapidamente os ativos relevantes usando o Omnisearch e a busca por facetas que usam filtros para ajudá-lo a restringir ainda mais sua pesquisa. Você também pode salvar suas pesquisas como coleções inteligentes para o futuro.

## Pesquisar ativos usando o Omnisearch {#search-assets-using-omnisearch}

Para pesquisar ativos no Brand Portal:

1. Na barra de ferramentas, clique no ícone **[!UICONTROL Pesquisar]** ou pressione a tecla &quot;**[!UICONTROL /]**&quot; para iniciar o Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Na caixa de pesquisa, digite uma palavra-chave para os ativos que deseja pesquisar.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >São necessários pelo menos 3 caracteres no Omnisearch para que sugestões de pesquisa sejam exibidas.

1. Selecione dentre as sugestões relacionadas que aparecem na lista suspensa para acessar rapidamente os ativos relevantes.

   ![](assets/assets-search-result.png)

   *Pesquisa de ativos usando o omnisearch*

Para saber mais sobre o comportamento da pesquisa com ativos marcados inteligentes, consulte [compreender os resultados e o comportamento da pesquisa](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html).

## Pesquisar usando aspectos no painel Filtros {#search-using-facets-in-filters-panel}

Os aspectos de pesquisa no painel Filtros adicionam granularidade à sua experiência de pesquisa e tornam a funcionalidade de pesquisa eficiente. Os aspectos de pesquisa usam várias dimensões (predicados) que permitem executar pesquisas complexas. É possível detalhar facilmente para o nível de detalhes desejado para uma pesquisa mais focada.

Por exemplo, se você estiver procurando uma imagem, poderá escolher se deseja um bitmap ou uma imagem vetorial. Você pode reduzir ainda mais o escopo da pesquisa especificando o tipo MIME para a imagem na faceta de pesquisa Tipo de arquivo. Da mesma forma, ao pesquisar documentos, você pode especificar o formato, por exemplo, PDF ou MS Word.<br />

![Painel filtros no painel Brand ](assets/file-type-search.png "PortalFilters no Brand Portal")

O painel **[!UICONTROL Filtros]** inclui algumas facetas padrão, como - **[!UICONTROL Navegador de caminhos]**, **[!UICONTROL Tipo de arquivo]**, **[!UICONTROL Tamanho do arquivo]**, **[!UICONTROL Estado]** e **[!UICONTROL Orientação]**. No entanto, você pode [adicionar aspectos de pesquisa personalizados](../using/brand-portal-search-facets.md) ou remover aspectos de pesquisa específicos do painel **[!UICONTROL Filtros]** adicionando ou removendo predicados no Formulário de pesquisa subjacente. Veja a lista dos [predicados de pesquisa disponíveis e utilizáveis no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Para aplicar filtros à sua pesquisa, use os [aspectos de pesquisa](../using/brand-portal-search-facets.md) disponíveis:

1. Clique no ícone de sobreposição e selecione **[!UICONTROL Filtro]**.

   ![](assets/selectorrail.png)

1. No painel **[!UICONTROL Filtros]** à esquerda, selecione as opções apropriadas para aplicar os filtros relevantes.
Por exemplo, use os seguintes filtros padrão:

   * **[!UICONTROL Navegador]** de caminho para pesquisar ativos em um diretório específico. O caminho de pesquisa padrão do predicado para Navegador de caminho é `/content/dam/mac/<tenant-id>/`, que pode ser configurado editando o formulário de pesquisa padrão.
   >[!NOTE]
   >
   >Para usuários não administradores, [!UICONTROL Navegador de caminhos] no painel [!UICONTROL Filtro] mostra somente a estrutura de conteúdo das pastas (e suas pastas ancestrais) compartilhadas com eles.\
   >Para administrar usuários, o Navegador de caminhos permite navegar até qualquer pasta no Portal de marcas.

   * **[!UICONTROL Tipo de]** arquivo para especificar o tipo (imagem, documento, multimídia, arquivo) do arquivo de ativo que você está procurando. Além disso, você pode restringir o escopo da pesquisa, por exemplo, especificar o tipo MIME (Tiff, Bitmap, Imagens GIMP) para imagem ou formato (PDF ou MS Word) para os documentos.
   * **[!UICONTROL Tamanho do arquivo]** para pesquisar ativos com base em seu tamanho. Você pode especificar os limites inferior e superior do intervalo de tamanho para restringir sua pesquisa e especificar a unidade de medida a ser pesquisada.
   * **[!UICONTROL Os]** Estatutos buscam ativos com base nos status dos ativos, como Aprovação (Aprovada, Alterações Solicitadas, Rejeitada, Pendente) e Expiração.
   * **[!UICONTROL Média]** para pesquisar ativos com base na classificação dos ativos.
   * **[!UICONTROL Orientação]** para procurar ativos com base na orientação (horizontal, vertical, quadrada) dos ativos.
   * **[!UICONTROL Estilo]** para procurar ativos com base no estilo (colorido, monocromático) dos ativos.
   * **[!UICONTROL Video]** Formatto para pesquisar ativos de vídeo com base em seu formato (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   Você pode usar [aspectos de pesquisa personalizados](../using/brand-portal-search-facets.md) no painel Filtros editando o Formulário de pesquisa subjacente.

   * **[!UICONTROL O]** Predicado de propriedade, se usado no formulário de pesquisa, permite pesquisar ativos que correspondem a uma propriedade de metadados para a qual o predicado está mapeado.\
      Por exemplo, se o Predicado de propriedade estiver mapeado para [!UICONTROL `jcr:content /metadata/dc:title`], você poderá pesquisar ativos com base em seu título.\
      O [!UICONTROL Predicado de propriedade] oferece suporte a pesquisas de texto para:

      **Frases parciais**
Para permitir a pesquisa do ativo usando frases parciais no predicado da propriedade, maque a caixa de seleção **[!UICONTROL Pesquisa parcial]** em Pesquisar formulário.\
      Isso permite pesquisar pelos ativos desejados mesmo que não especifique as palavras/frases exatas usadas nos metadados do ativo.\
      É possível:
      * Especifique uma palavra que ocorre em sua frase pesquisada na faceta no painel Filtros. Por exemplo, se você pesquisar pelo termo **climb** (e o Predicado de propriedade estiver mapeado para a propriedade [!UICONTROL `dc:title`]), todos os ativos com a palavra **climb** em sua frase de título serão retornados.
      * Especificar uma parte da palavra, que ocorre na frase pesquisada, juntamente com o caracter curinga (*) para preencher as lacunas.
Por exemplo, pesquisando por:
         * **climb*** retorna todos os ativos com palavras que começam com os caracteres &quot;escalar&quot; em suas frases de título.
         * ***** Inicia todos os ativos com palavras que terminam com caracteres que &quot;sobem&quot; em suas frases de título.
         * ***climb*** retorna todos os ativos com palavras que incluem os caracteres &quot;escalar&quot; em suas frases de título.

Para permitir pesquisas que não diferenciem maiúsculas de minúsculas no predicado de propriedade, ative a variável       **Texto sem distinção entre maiúsculas e**
minúsculasPara permitir pesquisas sem distinção entre maiúsculas e minúsculas no predicado de propriedade, ative a  **[!UICONTROL opção Ignorar]** caixa de seleção no Formulário de pesquisa. Por padrão, a pesquisa de texto no predicado de propriedade faz distinção entre maiúsculas e minúsculas.
   >[!NOTE]
   >
   >Ao marcar a caixa de seleção **[!UICONTROL Pesquisa parcial]**, **[!UICONTROL Ignorar caso]** é selecionado por padrão.

   ![](assets/wildcard-prop-1.png)

   Os resultados da pesquisa são exibidos de acordo com os filtros aplicados, juntamente com a contagem dos resultados da pesquisa.

   ![](assets/omnisearch-with-filters.png)

   Resultado da pesquisa do ativo com contagem de resultados da pesquisa.

1. Você pode navegar para um item facilmente a partir do resultado da pesquisa e retornar ao mesmo resultado da pesquisa usando o botão Voltar no seu navegador sem precisar executar novamente o query de pesquisa.

## Salvar suas pesquisas como coleção inteligente {#save-your-searches-as-smart-collection}

Você pode salvar as configurações de pesquisa como uma coleção inteligente para poder repetir rapidamente a mesma pesquisa sem precisar refazer as mesmas configurações posteriormente.

Para salvar as configurações de pesquisa como uma coleção inteligente:

1. Toque/ clique em **[!UICONTROL Salvar coleção inteligente]** e forneça um nome para a coleção inteligente.

   Para tornar a coleção inteligente acessível a todos os usuários, selecione **[!UICONTROL Public]**. Uma mensagem confirma que a coleção inteligente foi criada e adicionada à lista de suas pesquisas salvas.

   >[!NOTE]
   >
   >Os usuários não administradores podem ser restringidos de tornar públicas as coleções inteligentes, para evitar ter um grande número de coleções inteligentes públicas criadas por usuários não administradores no Portal de marcas da organização. As organizações podem desativar a configuração **[!UICONTROL Permitir a criação de coleções inteligentes públicas]** a partir das configurações **[!UICONTROL Geral]** disponíveis no painel de ferramentas administrativas.

   ![](assets/save_smartcollectionui.png)

1. Para salvar a coleção inteligente em um nome diferente e marcar ou desmarcar a caixa de seleção **[!UICONTROL Public]**, clique em **[!UICONTROL Editar coleção inteligente]**.

   ![](assets/edit_smartcollection.png)

1. Na caixa de diálogo **[!UICONTROL Editar coleção inteligente]**, selecione **[!UICONTROL Salvar como]** e insira um nome para a coleção inteligente. Clique em **[!UICONTROL Salvar]**.

   ![](assets/saveas_smartsearch.png)
