---
title: Usar aspectos de pesquisa personalizados
seo-title: Usar aspectos de pesquisa personalizados
description: Os administradores podem adicionar a pesquisa à painel Filtros para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.
seo-description: Os administradores podem adicionar a pesquisa à painel Filtros para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: referência
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 19 faa 028-246 b -42 c 7-869 f -97 c 95 c 7 a 1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Usar aspectos de pesquisa personalizados {#use-custom-search-facets}

Os administradores podem adicionar a pesquisa à painel [!UICONTROL Filtros] para personalizar a pesquisa e tornar a funcionalidade de pesquisa versátil.

O Brand Portal oferece suporte à [pesquisa](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) fachada para pesquisas granulares de ativos de marca aprovados, o que é possível devido ao painel [**Filtros**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Os aspectos de pesquisa são disponibilizados no painel Filtros por meio do Formulário **[!UICONTROL Pesquisar]** nas ferramentas administrativas. Um formulário de pesquisa padrão chamado Trilho de pesquisa de ativos existe na página Pesquisar formulários nas ferramentas administrativas. No entanto, os administradores podem personalizar o painel Filtros padrão ao editar o Formulário de pesquisa padrão (Painel de pesquisa de ativos de ativos) ao adicionar, modificar ou remover previsões de pesquisa, tornando a funcionalidade de pesquisa versátil.

Você pode usar vários predicados de pesquisa para personalizar o **[!UICONTROL painel Filtros]** . Por exemplo, adicione o predicado da propriedade para pesquisar ativos que correspondam a uma única propriedade especificada neste predicado. Adicione o predicado de opções para pesquisar ativos que correspondam a um ou mais valores especificados para uma propriedade específica. Adicione o predicado de intervalo de datas para pesquisar ativos criados em um intervalo de datas especificado.

>[!NOTE]
>
>O AEM permite que as organizações [publiquem formulários de pesquisa personalizados de autor](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) de AEM para o Brand Portal, em vez de recriar o mesmo formulário no Brand Portal.

## Adicionar um predicado de pesquisa {#add-a-search-predicate}

Para adicionar um predicado de pesquisa ao painel **[!UICONTROL Filtros]** :

1. Para acessar as ferramentas administrativas, clique no logotipo do AEM na barra de ferramentas na parte superior.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique em **[!UICONTROL Pesquisar formulários]**.

   ![](assets/navigation-panel-1.png)

3. Na página **[!UICONTROL Pesquisar formulários]** , selecione **[!UICONTROL Painel de pesquisa de administração de ativos]**.

   ![](assets/search-forms-page.png)

4. Na barra de ferramentas que aparece na parte superior, clique **[!UICONTROL em Editar]** para abrir o formulário de pesquisa editar.

   ![](assets/edit-search-form-1.png)

5. Na página [!UICONTROL Editar formulário] de pesquisa, arraste um predicado da guia [!UICONTROL Selecionar predicado] para o painel principal. Por exemplo, arraste **[!UICONTROL o Predicado da propriedade]**.

   O campo **[!UICONTROL Propriedade]** aparece no painel principal e a guia **[!UICONTROL Configurações]** à direita exibe as propriedades da propriedade.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >O rótulo do cabeçalho na guia **[!UICONTROL Configurações]** identifica o tipo de predicado selecionado.

6. Na guia **[!UICONTROL Configurações]** , insira um rótulo, texto de espaço reservado e descrição para o predicado da propriedade.

   * Selecione **[!UICONTROL Pesquisa parcial]**, se desejar permitir a pesquisa parcial de frases (e pesquisa curinga) de ativos com base no valor da propriedade especificada. Por padrão, o predicado suporta a pesquisa de texto completo.
   * Selecione **[!UICONTROL Ignorar caso]** se desejar que a pesquisa do ativo com base no valor da propriedade não diferencie maiúsculas de minúsculas. Por padrão, a pesquisa por valores de propriedade no Filtro de pesquisa diferencia maiúsculas e minúsculas.
   >[!NOTE]
   >
   >Ao selecionar **[!UICONTROL a caixa de seleção Pesquisa]** parcial, [!UICONTROL Ignorar caso] está selecionado por padrão.

7. No campo [!UICONTROL Nome] da propriedade, abra o seletor de propriedades e selecione a propriedade com base na qual a pesquisa é realizada. Como alternativa, insira um nome para a propriedade. Por exemplo, insira [!UICONTROL `  jcr :content/metadata/dc:title`] ou [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

8. Clique **[!UICONTROL em Concluído]** para salvar as configurações.
9. Na interface do usuário [!UICONTROL Ativos] , clique no ícone de sobreposição e escolha **[!UICONTROL Filtro]** para navegar até o **[!UICONTROL painel Filtros]** . O predicado **[!UICONTROL Propriedade]** é adicionado ao painel.

   ![](assets/property-filter-panel.png)

10. Digite um título para que o ativo seja pesquisado na caixa de texto **[!UICONTROL Propriedade]** . Por exemplo, "Adobe". Quando você realiza uma pesquisa, os ativos com o título correspondente à "Adobe" são exibidos nos resultados da pesquisa.

## Lista de predicações de pesquisa {#list-of-search-predicates}

Assim como você adiciona um **[!UICONTROL predicado de Propriedade]** , é possível adicionar os seguintes predefinidos ao painel **[!UICONTROL Filtros]** :

| **Nome do predicado** | **Descrição** | **Propriedades** |
|-------|-------|----------|
| [!UICONTROL Navegador de caminhos] | Predicado de pesquisa para pesquisar ativos em um local específico. **Observação:***Para um usuário conectado, o navegador de caminho no Filtro mostra apenas a estrutura de conteúdo das pastas (e os ancestrais) compartilhados com o usuário.*<br> Os usuários administradores podem pesquisar ativos em qualquer pasta navegando até essa pasta usando o Navegador de caminho. <br> Considerando que os usuários não administradores podem pesquisar ativos em uma pasta (acessível a eles), navegando para essa pasta no Navegador de caminhos. | <ul><li>Rótulo do campo</li><li>Caminho</li><li>Descrição</li></ul> |
| [!UICONTROL Propriedade] | Pesquisar ativos com base em uma propriedade de metadados específica. **Observação:***Ao selecionar Pesquisa parcial, Ignorar letras maiúsculas e minúsculas é selecionado por padrão*. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da Propriedade</li><li>Pesquisa parcial</li><li>Ignorar diferença entre maiúsculas e minúsculas</li><li> Descrição</li></ul> |
| [!UICONTROL Propriedade de vários valores] | Semelhante ao predicado da propriedade, mas permite vários valores de entrada, separados por um delimitador (padrão é vírgula,[]) ativos correspondentes a qualquer um dos valores de entrada são retornados nos resultados. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da propriedade</li><li>Suporte do delimitador</li><li>Ignorar diferença entre maiúsculas e minúsculas</li><li>Descrição</li></ul> |
| [!UICONTROL Tags] | Predicado de pesquisa para pesquisar ativos com base em tags. É possível configurar a propriedade Caminho para preencher várias tags na lista de Tags. * Observação: Os administradores podem precisar alterar o valor do caminho, por exemplo, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]se publicarem o formulário de pesquisa do AEM, onde o caminho não inclui informações de locatário, por exemplo,[!UICONTROL `/etc/tags/<custom_tag_namespace>`] | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Caminho</li><li>Descrição</li></ul> |
| [!UICONTROL Caminho] | Predicado de pesquisa para pesquisar ativos em um local específico. | <ul><li>Rótulo do campo</li><li>Caminho</li><li>Descrição</li></ul> |  |
| [!UICONTROL Data relativa] | Predicado de pesquisa para pesquisar ativos com base na data relativa da criação. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Data relativa</li></ul> |
| [!UICONTROL Intervalo] | Predicado de pesquisa para pesquisar ativos que estão dentro de um intervalo específico de valores de propriedade. No painel Filtros, é possível especificar valores de propriedade mínimo e máximo para o intervalo. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Intervalo de datas] | Predicado de pesquisa para pesquisar ativos criados em um intervalo especificado para uma propriedade date. No painel Filtros, é possível especificar datas de início e fim. | <ul><li>Rótulo do campo</li><li>Espaço reservado</li><li>Nome da propriedade</li><li>Texto do intervalo (de)</li><li>Texto do intervalo (até)</li><li>Descrição</li></ul> |
| [!UICONTROL Data] | Predicado de pesquisa para uma pesquisa com base em controle deslizante de ativos com base em uma propriedade date. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Tamanho do arquivo] | Predicado de pesquisa para pesquisar ativos com base em seu tamanho. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Caminho</li><li>Descrição</li></ul> |
| [!UICONTROL Última modificação do ativo] | Predicado de pesquisa para pesquisar ativos com base na última data de modificação. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Status de aprovação] | Predicado de pesquisa para pesquisar ativos com base na propriedade de metadados de aprovação. O nome da propriedade padrão é **dam: status**. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Status da retirada] | Predicado de pesquisa para pesquisar ativos com base no status de check-out de um ativo quando ele foi publicado nos ativos AEM. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Retirado por] | Predicado de pesquisa para pesquisar ativos com base no usuário que retirou o ativo. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Status da expiração] | Predicado de pesquisa para pesquisar ativos com base no status de expiração. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |
| [!UICONTROL Membro da coleção] | Predicado de pesquisa para pesquisar ativos com base em se um ativo faz parte de uma coleção. | Descrição |
| [!UICONTROL Oculto] | Esse predicado não está visível explicitamente para os usuários finais e é usado para qualquer restrição oculta geralmente para restringir o tipo de resultados de pesquisa a **dam: Ativo**. | <ul><li>Rótulo do campo</li><li>Nome da propriedade</li><li>Descrição</li></ul> |

>[!NOTE]
>
>Não use **[!UICONTROL Predicado de opções]**, **[!UICONTROL Predicado de status de publicação]** e Predicado **[!UICONTROL de classificação]** como esses previstos não estão funcionais no Brand Portal.

## Excluir um predicado de pesquisa {#delete-a-search-predicate}

Para excluir um predicado de pesquisa, siga estas etapas:

1. Clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique em **[!UICONTROL Pesquisar formulários]**.

   ![](assets/navigation-panel-2.png)

3. Na página **[!UICONTROL Pesquisar formulários]** , selecione **[!UICONTROL Painel de pesquisa de administração de ativos]**.

   ![](assets/search-forms-page.png)

4. Na barra de ferramentas que aparece na parte superior, clique **[!UICONTROL em Editar]** para abrir o formulário de pesquisa editar.

   ![](assets/edit-search-form-2.png)

5. Na página [!UICONTROL Editar formulário] de pesquisa, no painel principal, selecione o predicado que deseja excluir. Por exemplo, selecione **[!UICONTROL Predicado de propriedade]**.

   A guia **[!UICONTROL Configurações]** à direita exibe campos do predicado de propriedade.

6. Para excluir o predicado da propriedade, clique no ícone bin. Na caixa de diálogo **[!UICONTROL Excluir campo]** , clique **[!UICONTROL em Excluir]** para confirmar a ação de exclusão.

   O campo **[!UICONTROL Predicado]** de propriedade é removido do painel principal, e a guia **[!UICONTROL Configurações]** fica vazia.

   ![](assets/search-form-delete-predicate.png)

7. Para salvar as alterações, clique **[!UICONTROL em Concluído]** na barra de ferramentas.
8. Na interface do usuário **[!UICONTROL Ativos]** , clique no ícone de sobreposição e escolha **[!UICONTROL Filtro]** para navegar até o **[!UICONTROL painel Filtros]** . O predicado **[!UICONTROL Propriedade]** é removido do painel.

   ![](assets/property-predicate-removed.png)
