---
title: Usar facetas de busca personalizada
seo-title: Usar facetas de busca personalizada
description: Os administradores podem adicionar predicados de pesquisa ao painel Filtros para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.
seo-description: Os administradores podem adicionar predicados de pesquisa ao painel Filtros para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Usar facetas de busca personalizada {#use-custom-search-facets}

Os administradores podem adicionar predicados de pesquisa ao painel [!UICONTROL Filtros] para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.

O Brand Portal oferece suporte à pesquisa [](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) facetada para pesquisas granulares de ativos de marca aprovados, o que é possível devido ao painel [****Filtros](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Os aspectos de pesquisa são disponibilizados no painel Filtros por meio do Formulário**[!UICONTROL  de]** pesquisa nas ferramentas administrativas. Um formulário de pesquisa padrão chamado Asset Admin Search Rail existe na página Formulários de pesquisa nas ferramentas administrativas. No entanto, os administradores podem personalizar o painel Filtros padrão editando o Formulário de pesquisa padrão (Painel de pesquisa do administrador do ativo) adicionando, modificando ou removendo predicados de pesquisa, tornando assim a funcionalidade de pesquisa versátil.

Você pode usar vários predicados de pesquisa para personalizar o painel **[!UICONTROL Filtros]**. Por exemplo, adicione o predicado de propriedade para procurar ativos que correspondam a uma única propriedade especificada neste predicado. Adicione o predicado de opções para procurar ativos que correspondam a um ou mais valores especificados para uma propriedade específica. Adicione o predicado de intervalo de datas para pesquisar ativos criados dentro de um intervalo de datas especificado.

>[!NOTE]
>
>O AEM permite que as organizações [publiquem os formulários de pesquisa personalizados do autor](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) do AEM para o Portal de marcas, em vez de recriar o mesmo formulário no Portal de marcas.

## Adicionar um predicado de pesquisa {#add-a-search-predicate}

Para adicionar um predicado de pesquisa ao painel **[!UICONTROL Filtros]**:

1. Para acessar as ferramentas administrativas, clique no logotipo do AEM na barra de ferramentas na parte superior.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Pesquisar formulários]**.

   ![](assets/navigation-panel-1.png)

1. Na página **[!UICONTROL Pesquisar formulários]**, selecione Painel**[!UICONTROL  de pesquisa do administrador de]**ativos.

   ![](assets/search-forms-page.png)

1. Na barra de ferramentas exibida na parte superior, clique em **[!UICONTROL Editar]**para abrir o formulário de pesquisa de edição.

   ![](assets/edit-search-form-1.png)

1. Na página [!UICONTROL Editar formulário] de pesquisa, arraste um predicado da guia [!UICONTROL Selecionar predicado] para o painel principal. Por exemplo, arraste o Predicado **[!UICONTROL de propriedade]**.

   O campo **[!UICONTROL Propriedade]**é exibido no painel principal e a guia**[!UICONTROL  Configurações]** à direita exibe os predicados de propriedade.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >O rótulo do cabeçalho na guia **[!UICONTROL Configurações]**identifica o tipo de predicado selecionado.

1. Na guia **[!UICONTROL Configurações]**, digite um rótulo, um texto de espaço reservado e uma descrição para o predicado de propriedade.

   * Selecione Pesquisa ****parcial se desejar permitir a pesquisa parcial de frases (e a pesquisa curinga) de ativos com base no valor da propriedade especificada. Por padrão, o predicado suporta a pesquisa de texto completo.
   * Selecione **[!UICONTROL Ignorar maiúsculas de minúsculas]**, se desejar que a pesquisa de ativos com base no valor da propriedade não diferencie maiúsculas de minúsculas. Por padrão, a pesquisa por valores de propriedade no Filtro de pesquisa faz distinção entre maiúsculas e minúsculas.
   >[!NOTE]
   >
   >Ao marcar a caixa de seleção Pesquisa ****parcial,**[!UICONTROL  Ignorar caso]** é selecionado por padrão.

1. No campo Nome **[!UICONTROL da]**propriedade, abra o seletor de propriedades e selecione a propriedade com base na qual a pesquisa é realizada. Como alternativa, insira um nome para a propriedade. Por exemplo, insira`  jcr :content/metadata/dc:title`ou`./jcr:content/metadata/dc:title`.

   ![](assets/title-prop.png)

1. Clique em **[!UICONTROL Concluído]**para salvar as configurações.
1. Na interface do usuário [!UICONTROL Assets] , clique no ícone de sobreposição e escolha **[!UICONTROL Filtro]**para navegar até o painel**[!UICONTROL  Filtros]** . O predicado **[!UICONTROL Propriedade]**é adicionado ao painel.

   ![](assets/property-filter-panel.png)

1. Insira um título para o ativo a ser pesquisado na caixa de texto **[!UICONTROL Propriedade]**. Por exemplo, &quot;Adobe&quot;. Quando você realiza uma pesquisa, os ativos com o título correspondente a &quot;Adobe&quot; são exibidos nos resultados da pesquisa.

## Lista de predicados de pesquisa {#list-of-search-predicates}

Semelhante à forma como você adiciona um predicado **[!UICONTROL Propriedade]**, você pode adicionar os seguintes predicados ao painel**[!UICONTROL  Filtros]** :

| **Nome do Predicado** | **Descrição** | **Propriedades** |
|-------|-------|----------|
| **[!UICONTROL Navegador de caminhos]** | Predicado de pesquisa para pesquisar ativos em um local específico. **** Observação: *Para um usuário conectado, o navegador de caminho no Filtro mostra somente a estrutura de conteúdo das pastas (e seus ancestrais) compartilhadas com o usuário.* <br> Os usuários administradores podem pesquisar ativos em qualquer pasta navegando até essa pasta usando o Navegador de caminhos. <br> Enquanto isso, usuários não administradores podem pesquisar ativos em uma pasta (acessível a eles) navegando até essa pasta no Navegador de caminhos. | <ul><li>Rótulo do campo</li><li>Caminho</li><li>Descrição</li></ul> |
| **[!UICONTROL Propriedade]** | Pesquisar ativos com base em uma propriedade de metadados específica. **** Observação: *Ao selecionar Pesquisa parcial, Ignorar caso é selecionado por padrão*. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da Propriedade</li><li>Pesquisa parcial</li><li>Ignorar diferença entre maiúsculas e minúsculas</li><li> Descrição</li></ul> |
| **[!UICONTROL Propriedade de vários valores]** | Semelhante ao predicado de propriedade, mas permite vários valores de entrada, separados por um delimitador (o padrão é COMMA[,]) ativos que correspondem a qualquer um dos valores de entrada são retornados nos resultados. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da propriedade</li><li>Suporte do delimitador</li><li>Ignorar diferença entre maiúsculas e minúsculas</li><li>Descrição</li></ul> |
| **[!UICONTROL Tags]** | Projete de pesquisa para pesquisar ativos com base em tags. Você pode configurar a propriedade Caminho para preencher várias tags na lista Tags. *Observação: Os administradores podem precisar alterar o valor do caminho, por exemplo, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]se publicarem o formulário de pesquisa no AEM, onde o caminho não inclui informações de locatário, por exemplo, [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Caminho</li><li>Descrição</li></ul> |
| **[!UICONTROL Caminho]** | Predicado de pesquisa para pesquisar ativos em um local específico. | <ul><li>Rótulo do campo</li><li>Caminho</li><li>Descrição</li></ul> |  |
| **[!UICONTROL Data relativa]** | O predicado de pesquisa para pesquisar ativos com base na data relativa de sua criação. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Data relativa</li></ul> |
| **[!UICONTROL Intervalo]** | O predicado de pesquisa para pesquisar ativos que estão dentro de um intervalo especificado de valores de propriedade. No painel Filtros, é possível especificar valores de propriedade mínimos e máximos para o intervalo. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Intervalo de datas]** | Projete de pesquisa para pesquisar ativos criados em um intervalo especificado para uma propriedade de data. No painel Filtros, é possível especificar as datas de início e término. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da propriedade</li><li>Texto do intervalo (de)</li><li>Texto do intervalo (até)</li><li>Descrição</li></ul> |
| **[!UICONTROL Data]** | Projete de pesquisa para uma pesquisa de ativos baseada em controle deslizante com base em uma propriedade de data. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Tamanho do arquivo]** | Predicado de pesquisa para pesquisar ativos com base em seu tamanho. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Caminho</li><li>Descrição</li></ul> |
| **[!UICONTROL Última modificação do ativo]** | Projete de pesquisa para pesquisar ativos com base na última data modificada. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Status de aprovação]** | Projete de pesquisa para pesquisar ativos com base na propriedade de metadados de aprovação. O nome da propriedade padrão é **dam:status**. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Status da retirada]** | O predicado de pesquisa para pesquisar ativos com base no status de check-out de um ativo quando ele foi publicado nos ativos AEM. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Retirado por]** | O predicado de pesquisa para pesquisar ativos com base no usuário que fez check-out do ativo. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Status da expiração]** | Projete de pesquisa para pesquisar ativos com base no status de expiração. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| **[!UICONTROL Membro da coleção]** | O predicado de pesquisa para pesquisar ativos com base no fato de um ativo fazer parte de uma coleção. | Descrição |
| **[!UICONTROL Oculto]** | Esse predicado não é explicitamente visível para os usuários finais e é usado para quaisquer restrições ocultas normalmente para restringir o tipo de resultados de pesquisa a **dam:Asset**. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |

>[!NOTE]
>
>Não use o Predicado **[!UICONTROL de]**opções, o Predicado**[!UICONTROL  de status de]**publicação e o Predicado **[!UICONTROL de]**classificação, pois esses predicados não estão funcionando no Portal de marcas.

## Excluir um predicado de pesquisa {#delete-a-search-predicate}

Para excluir um predicado de pesquisa, siga estas etapas:

1. Clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Pesquisar formulários]**.

   ![](assets/navigation-panel-2.png)

1. Na página **[!UICONTROL Pesquisar formulários]**, selecione Painel**[!UICONTROL  de pesquisa do administrador de]**ativos.

   ![](assets/search-forms-page.png)

1. Na barra de ferramentas exibida na parte superior, clique em **[!UICONTROL Editar]**para abrir o formulário de pesquisa de edição.

   ![](assets/edit-search-form-2.png)

1. Na página [!UICONTROL Editar formulário] de pesquisa, no painel principal, selecione o predicado que deseja excluir. Por exemplo, selecione Predicado **[!UICONTROL de propriedade]**.

   A guia **[!UICONTROL Configurações]**à direita exibe os campos de predicado de propriedade.

1. Para excluir o predicado de propriedade, clique no ícone bin. Na caixa de diálogo **[!UICONTROL Excluir campo]**, clique em**[!UICONTROL  Excluir]** para confirmar a ação de exclusão.

   O campo Predicado de **[!UICONTROL propriedade]**é removido do painel principal e a guia**[!UICONTROL  Configurações]** fica vazia.

   ![](assets/search-form-delete-predicate.png)

1. Para salvar as alterações, clique em **[!UICONTROL Concluído]**na barra de ferramentas.
1. Na interface do usuário **[!UICONTROL Assets]**, clique no ícone de sobreposição e escolha**[!UICONTROL  Filtro]** para navegar até o painel **[!UICONTROL Filtros]**. O predicado**[!UICONTROL  Propriedade]** é removido do painel.

   ![](assets/property-predicate-removed.png)
