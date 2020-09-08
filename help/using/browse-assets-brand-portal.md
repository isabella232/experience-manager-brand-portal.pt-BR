---
title: Procurar ativos no Brand Portal
seo-title: Procurar ativos no Brand Portal
description: Navegue pelos ativos, navegue pelas hierarquias de ativos e pesquise os ativos, usando diferentes opções de visualização e elementos de interface no Brand Portal.
seo-description: Navegue pelos ativos, navegue pelas hierarquias de ativos e pesquise os ativos, usando diferentes opções de visualização e elementos de interface no Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: ca60fe1b76c6e99d835457627fcc4bf402b6bd87
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 4%

---


# Browse assets on Brand Portal {#browsing-assets-on-brand-portal}

O Portal de marcas da AEM Assets oferece vários recursos e elementos de interface do usuário que facilitam a navegação pelos recursos, a passagem de hierarquias de ativos e a pesquisa de ativos ao mesmo tempo que usam opções de visualização diferentes.

AEM logotipo na barra de ferramentas AEM na parte superior facilita que os usuários administradores acessem o painel de ferramentas administrativas.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

Seletor de painéis no canto superior esquerdo do Brand Portal suspenso para expor as opções de navegação nas hierarquias de ativos, dinamizar sua pesquisa e exibir os recursos.

![](assets/siderail-1.png)

Você pode visualização, navegar e selecionar ativos usando qualquer uma das visualizações disponíveis (Cartão, Coluna e Lista) no seletor de visualizações na parte superior direita do Brand Portal.

![](assets/viewselector.png)

## Visualização e seleção de recursos {#viewing-and-selecting-resources}

Exibir, navegar e selecionar cada uma são conceitualmente iguais em todas as visualizações, mas têm pequenas variações de manuseio, dependendo da visualização que você está usando.

Você pode visualização, navegar e selecionar (para mais ações) seus recursos com qualquer uma das visualizações disponíveis:

* Exibição de coluna
* Exibição de cartão
* Exibição de lista  

### Exibição de cartão

![](assets/card-view.png)

A Exibição de cartão exibe cartões de informações para cada item no nível atual. Esses cartões fornecem os seguintes detalhes:

* Uma representação visual do ativo/pasta.
* Tipo
* Título
* Nome
* Data e hora em que o ativo foi publicado no Brand Portal a partir da AEM
* Tamanho
* Dimensões

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Visualização de cartão para usuários não administradores

Cartões de pastas, na Visualização de cartão, exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas que estão acessando, em relação à hierarquia pai.
As informações de hierarquia de pastas são particularmente úteis na diferenciação de pastas com nomes semelhantes a outras pastas compartilhadas de uma hierarquia de pastas diferente. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, ativos/pastas com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para se ajustarem aos tamanhos dos cartões. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o mouse sobre o caminho truncado.

![](assets/folder-hierarchy1.png)

**Opção Visão geral para visualização propriedades de ativos**

A opção Visão geral está disponível para usuários não administradores (editores, visualizadores, usuários convidados) para visualização das Propriedades do ativo de ativos/pastas selecionados. A opção Visão geral está visível:

* na barra de ferramentas na parte superior da seleção de um ativo/pasta.
* na lista suspensa ao selecionar o Seletor de trilho.

Ao selecionar a opção **[!UICONTROL Visão geral]** enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação do ativo. Enquanto isso, na página de detalhes do ativo, selecionar a opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Configurações de visualização na visualização da placa

**[!UICONTROL A caixa de diálogo Configurações]** de visualização é aberta ao selecionar Configurações **[!UICONTROL de]** Visualização no seletor de visualizações. Ele permite redimensionar as miniaturas de ativos na visualização do cartão. Dessa forma, você pode personalizar sua visualização e controlar o número de miniaturas exibidas.

![](assets/cardviewsettings.png)

### Exibição de lista  

![](assets/list-view.png)

A visualização de lista exibe informações para cada recurso no nível atual. A visualização de listas fornece os seguintes detalhes:

* Imagem em miniatura de ativos
* Nome
* Título
* Localidade
* Tipo
* Dimension
* Tamanho
* Classificação
* Caminho da pasta mostrando a hierarquia<sup>do ativo*</sup>
* Data de publicação do ativo no Brand Portal

A coluna Caminho permite identificar facilmente o local do ativo na hierarquia de pastas. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Configurações de visualização na visualização da lista

A visualização de lista mostra o **[!UICONTROL Nome]** do ativo como a primeira coluna por padrão. Informações adicionais, como **[!UICONTROL Título]** do ativo, **[!UICONTROL Localidade]**, **[!UICONTROL Tipo]**, **[!UICONTROL Dimension]**, **[!UICONTROL Tamanho]******, Classificação, status de publicação também são mostradas. However, you can select the columns to be shown using **[!UICONTROL View Settings]**.

![](assets/list-view-setting.png)

### Exibição de coluna

![](assets/column-view.png)

Use a visualização de coluna para navegar em uma árvore de conteúdo por uma série de colunas em cascata. Essa visualização ajuda a visualizar e navegar pela hierarquia de ativos.

A seleção de um recurso na primeira coluna (na extremidade esquerda) exibe os recursos filhos na segunda coluna à direita. A seleção de um recurso na segunda coluna exibe recursos filhos na terceira coluna à direita e assim por diante.

Você pode navegar para cima e para baixo na árvore tocando ou clicando no nome do recurso ou na divisa à direita do nome do recurso.

* O nome do recurso e a divisa são destacados quando tocados ou clicados.
* Tocar ou clicar na miniatura seleciona o recurso.
* Quando selecionada, uma marca de seleção é sobreposta na miniatura e o nome do recurso é realçado.
* Os detalhes do recurso selecionado são mostrados na coluna final.

Quando um ativo é selecionado na visualização da coluna, a representação visual do ativo é exibida na coluna final junto com os seguintes detalhes:

* Título
* Nome
* Dimensões
* Data e hora em que o ativo foi publicado no Brand Portal a partir da AEM
* Tamanho
* Tipo
* Opção Mais Detalhes, para acessar a página de detalhes do ativo

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Árvore de conteúdo {#content-tree}

Além dessas visualizações, use a visualização em árvore para detalhar a hierarquia de ativos enquanto você visualização e seleciona os ativos ou pastas desejados.

Para abrir a visualização em árvore, toque/clique no seletor do painel na parte superior esquerda e selecione a árvore **** Conteúdo no menu.

![](assets/contenttree.png)

Na hierarquia de conteúdo, navegue até o ativo desejado.

![](assets/content-tree.png)

## Detalhes do ativo {#asset-details}

A página de detalhes do ativo permite que você visualização um ativo, baixe, compartilhe o link do ativo, mova-o para uma coleção ou visualização sua página de propriedades. Também permite navegar pela página de detalhes de outros ativos da mesma pasta sucessivamente.

![](assets/asset-detail.png)

Para visualização dos metadados do ativo ou visualização de suas várias representações, use o seletor de trilho na página de detalhes do ativo.

![](assets/asset-overview.png)

Você pode visualização todas as representações disponíveis do ativo na página de detalhes do ativo e selecionar uma representação para pré-visualização.

![](assets/renditions.png)

Para abrir a página de propriedades do ativo, use a opção **[!UICONTROL Propriedades (p)]** na barra superior.

![](assets/asset-properties.png)

Você também pode visualização uma lista de todos os seus ativos relacionados (ativos de origem ou derivados em AEM) na página de propriedades de um ativo, já que a relação de ativos também é publicada AEM para o Brand Portal.
