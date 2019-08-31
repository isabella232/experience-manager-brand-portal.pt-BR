---
title: Navegação de ativos no Brand Portal
seo-title: Procurar ativos no Brand Portal
description: Navegue pelos ativos, navegue por hierarquias de ativos e pesquise ativos, usando opções de exibição e elementos de interface de usuário diferentes no Portal da marca.
seo-description: Navegue pelos ativos, navegue por hierarquias de ativos e pesquise ativos, usando opções de exibição e elementos de interface de usuário diferentes no Portal da marca.
uuid: 178 ce 217-0050-4922-a 204-f 4539 d 46 f 539
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
topic-tags: introdução
discoiquuid: a 70 ce 694-81 d 1-4829-9 e 61-b 6412 e 013 e 5 c
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Navegação de ativos no Brand Portal {#browsing-assets-on-brand-portal}

O AEM Assets Brand Portal oferece vários recursos e elementos da interface do usuário que facilitam a navegação pelos recursos, a tendência das hierarquias de ativos e a pesquisa de ativos enquanto usam diferentes opções de visualização.

O logotipo do AEM na barra de ferramentas do AEM na parte superior facilita os usuários administradores de acessar o painel de ferramentas administrativas.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

O seletor de painel no canto superior esquerdo do Portal da marca para expor as opções para navegar em hierarquias de ativos, simplificar a pesquisa e os recursos de exibição.

![](assets/siderail-1.png)

É possível exibir, navegar e selecionar ativos usando qualquer uma das exibições disponíveis (Cartão, Coluna e Lista) no seletor de visualização no canto superior direito do Portal da marca.

![](assets/viewselector.png)

## Visualização e seleção de recursos {#viewing-and-selecting-resources}

Visualizar, navegar e selecionar cada um são conceitualmente iguais em todas as exibições, mas têm pequenas variações de manuseio, dependendo da exibição usada.

Você pode visualizar, navegar e selecionar (para uma futura ação) seus recursos com qualquer uma das exibições disponíveis:

* Visualização de coluna
* Exibição de cartão
* Exibição de lista

### Exibição de cartão

![](assets/card-view.png)

A Exibição de cartão exibe cartões de informações para cada item no nível atual. Esses cartões fornecem os seguintes detalhes:

* Uma representação visual do ativo/pasta.
* Tipo
* Título
* Nome
* Data e hora em que o ativo foi publicado no Portal da marca a partir do AEM
* Tamanho
* Dimensões

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Exibição de cartão para usuários não administradores

Cartões de pastas, na Exibição de cartão, exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas, estão acessando, em relação à hierarquia pai.
As informações de hierarquia de pastas são especialmente úteis na diferenciação das pastas com nomes semelhantes a outras pastas compartilhadas a partir de uma hierarquia de pasta diferente. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, os ativos /folders com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para ajustar os tamanhos do cartão. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o mouse sobre o caminho truncado.

![](assets/folder-hierarchy1.png)

**Opção Visão geral para exibir propriedades de ativos**

A opção Visão geral está disponível para usuários não administradores (Editores, Visualizadores, Usuários convidados) para exibir Propriedades de ativos de pastas/ativos selecionados. A opção Visão geral está visível:

* na barra de ferramentas na parte superior ao selecionar um ativo/pasta.
* no menu suspenso ao selecionar o Seletor de painéis.

Ao selecionar [!UICONTROL a] opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação de ativos. Enquanto a página de detalhes do ativo selecionando a opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Exibir configurações na exibição de cartão

[!UICONTROL Caixa de diálogo Configurações] de exibição é aberta ao selecionar **[!UICONTROL Configurações de exibição]** no seletor de visualização. Ele permite redimensionar as miniaturas de ativos na exibição de Cartão. Dessa forma, você pode personalizar a exibição e controlar o número de miniaturas exibidas.

![](assets/cardviewsettings.png)

### Exibição de lista

![](assets/list-view.png)

A exibição de lista exibe informações para cada recurso no nível atual. A exibição de lista fornece os seguintes detalhes:

* Imagem em miniatura dos ativos
* Nome
* Título
* Localidade
* Tipo
* Dimensão
* Tamanho
* Classificação
* Caminho da pasta que mostra a hierarquia do ativo<sup>*</sup>
* Data de publicação do ativo no Brand Portal

* A coluna Caminho permite identificar facilmente o local do ativo na hierarquia de pastas. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Exibir configurações na exibição de lista

A exibição de Lista mostra [!UICONTROL o Nome] do ativo como a primeira coluna por padrão. Informações adicionais, como [!UICONTROL Título do ativo], [!UICONTROL Localidade], [!UICONTROL Tipo], [!UICONTROL Dimensões], [!UICONTROL Tamanho], [!UICONTROL Classificação], status de publicação também são mostradas. However, you can select the columns to be shown using [!UICONTROL View Settings].

![](assets/list-view-setting.png)

### Visualização de coluna

![](assets/column-view.png)

Use a exibição de coluna para navegar em uma árvore de conteúdo por uma série de colunas em cascata. Essa exibição ajuda a visualizar e navegar pela hierarquia do ativo.

Selecionar um recurso na primeira coluna (mais à esquerda) exibe os recursos filho na segunda coluna à direita. Selecionar um recurso na segunda coluna exibe os recursos filho na terceira coluna à direita, e assim por diante.

É possível navegar para cima e para baixo na árvore tocando ou clicando no nome do recurso ou na divisa à direita do nome do recurso.

* O nome do recurso e a divisa são destacados quando tocados ou clicados.
* Tocar ou clicar na miniatura seleciona o recurso.
* Quando selecionada, uma marca de seleção é sobreposta à miniatura e o nome do recurso é destacado.
* Os detalhes do recurso selecionado são mostrados na coluna final.

Quando um ativo é selecionado na exibição de coluna, a representação visual do ativo é exibida na coluna final, juntamente com os seguintes detalhes:

* Título
* Nome
* Dimensões
* Data e hora em que o ativo foi publicado no Portal da marca a partir do AEM
* Tamanho
* Tipo
* Mais detalhes, para ir na página de detalhes do ativo

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

<h4>Deselecting All</h4>
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

Além dessas exibições, use a exibição em árvore para detalhar a hierarquia do ativo enquanto você visualiza e seleciona os ativos ou pastas desejados.

Para abrir a exibição em árvore, toque/clique no seletor do painel no canto superior esquerdo e selecione a **[!UICONTROL árvore]** Conteúdo no menu.

![](assets/contenttree.png)

Na hierarquia do conteúdo, navegue até o ativo desejado.

![](assets/content-tree.png)

## Detalhes do ativo {#asset-details}

A página de detalhes do ativo permite exibir um ativo, baixar, compartilhar o link do ativo, movê-lo para uma coleção ou visualizar sua página de propriedades. Também permite que você navegue pela página de detalhes de outros ativos da mesma pasta em sucessão.

![](assets/asset-detail.png)

Para exibir os metadados do ativo ou exibir várias execuções, use o seletor do painel na página de detalhes do ativo.

![](assets/asset-overview.png)

Você pode exibir todas as representações disponíveis do ativo na página de detalhes do ativo e selecionar uma execução para visualizá-la.

![](assets/renditions.png)

Para abrir a página Propriedades do ativo, use **[!UICONTROL a opção Propriedades (p)]** na barra superior.

![](assets/asset-properties.png)

Você também pode exibir uma lista de todos os ativos relacionados (fonte ou ativos derivados no AEM) na página de propriedades de um ativo, já que a relação de ativo também é publicada do AEM para o Portal de marcas.
