---
title: Publicar predefinições, esquemas e facetas no Brand Portal
seo-title: Publicar predefinições, esquemas e facetas no Brand Portal
description: Saiba como publicar predefinições, esquemas e facetas no Brand Portal.
seo-description: Saiba como publicar predefinições, esquemas e facetas no Brand Portal.
uuid: c 836 d 9 bb -074 a -4113-9 c 91-b 2 bf 7658 b 88 d
topic-tags: publicação
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
discoiquuid: bc 305 abc -9373-4 d 33-9179-0 a 5 f 3904 b 352
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publicar predefinições, esquemas e facetas no Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

O artigo vai para a publicação de predefinições de imagens, esquemas de metadados e aspectos de pesquisa personalizados da instância de autor de AEM para o Portal da marca. A capacidade de publicação permite que as organizações reutilizem as predefinições de imagens, esquemas de metadados e aspectos de pesquisa criados/modificados na instância do autor de AEM, reduzindo assim os esforços duplicados.

>[!NOTE]
>
>A capacidade de publicar predefinições de imagens, esquema de metadados e aspectos de pesquisa da instância de autor de AEM para o Brand Portal está disponível AEM 6.2 SP 1-CFP 7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1) em diante.

## Publicar predefinições de imagens no Brand Portal {#publish-image-presets-to-brand-portal}

As predefinições de imagens são um conjunto de comandos de dimensionamento e formatação aplicados à imagem no momento da entrega de imagens. As predefinições de imagens podem ser criadas e modificadas no Brand Portal. Como alternativa, se a instância do autor de AEM estiver em execução no modo de mídia dinâmica, os usuários poderão criar predefinições no AEM Author e publicá-las no Portal da marca do AEM Assets e evitar recriar as mesmas predefinições no Brand Portal.\
Uma vez que a predefinição é criada, ela é listada como representação dinâmica no painel de representações de detalhes do ativo e no diálogo de download.

>[!NOTE]
>
>Se a instância do Autor de AEM não estiver sendo executada no [!UICONTROL modo] Dynamic Media (o cliente não comprou Dynamic Media), a [!UICONTROL execução TIFF] Pirâmide dos ativos não será criada no momento do upload. As predefinições de imagens ou as representações dinâmicas funcionam no [!UICONTROL TIFF] Pirâmico de um ativo. Portanto, se [!UICONTROL o TIFF] Pirâmide não estiver disponível na instância do Autor de AEM, ele também não estará disponível no Brand Portal. Como resultado, nenhuma representação dinâmica está presente no painel de representações da página de detalhes do ativo e no diálogo de download.

Para publicar predefinições de imagens no Brand Portal:

1. Na instância Autor de AEM, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos]** &gt; Predefinições **[!UICONTROL de imagens]**.
2. Selecione a predefinição de imagens ou várias predefinições de imagens na lista de predefinições de imagens e clique/toque **[!UICONTROL em Publicar no portal da marca]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando os usuários clicam **[!UICONTROL em Publicar no portal]** da marca, as predefinições de imagens são colocadas em fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de uma predefinição de imagens no Brand Portal:

1. Na instância Autor de AEM, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone **[!UICONTROL Ferramentas]** e navegue até **[!UICONTROL Ativos &gt; Predefinições de imagens]**.
2. Selecione uma predefinição de imagens e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

## Publicar esquema de metadados no Brand Portal {#publish-metadata-schema-to-brand-portal}

O esquema de metadados descreve o layout e as propriedades exibidas na página de propriedades de ativos/coleções.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se os usuários editarem o esquema padrão na instância Autor de AEM e estiverem dispostos a usar o mesmo esquema do esquema padrão no Brand Portal, poderão simplesmente publicar os formulários de esquema de metadados no Portal da marca. Nesse cenário, o esquema padrão no Brand Portal é substituído pelos esquemas padrão publicados a partir da instância do Autor de AEM.

Se os usuários criaram um esquema personalizado na instância Autor de AEM, poderão publicar o esquema personalizado no Brand Portal em vez de recriar o mesmo esquema personalizado lá. Os usuários podem aplicar esse esquema personalizado a qualquer pasta/coleção no Brand Portal.

>[!NOTE]
>
>Os esquemas padrão não podem ser publicados no Brand Portal se estiverem bloqueados na instância do AEM (ou seja, não são editados).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se uma pasta tiver um esquema aplicado à instância do Autor de AEM, o mesmo esquema deverá existir no Portal da marca para manter a consistência na página de propriedades do ativo no Autor de AEM e no Portal de marcas.

Para publicar um esquema de metadados da instância de autor de AEM no Portal da marca:

1. Na instância Autor de AEM, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos &gt; Esquemas de metadados]**.
2. Selecione um esquema de metadados e selecione **[!UICONTROL Publicar no portal da marca]** com as opções disponíveis na parte superior.

>[!NOTE]
>
>Quando os usuários clicam **[!UICONTROL em Publicar no Brand Portal]**, os esquemas de metadados são colocados na fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de um esquema de metadados do Brand Portal:

1. Na instância Autor de AEM, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos &gt; Esquemas de metadados]**.
2. Selecione um esquema de metadados e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

## Publicar aspectos de pesquisa no Brand Portal {#publish-search-facets-to-brand-portal}

Os formulários de pesquisa fornecem a capacidade de [pesquisa por facetas](../using/brand-portal-search-facets.md) para usuários no Portal da marca. Os aspectos de pesquisa fornecem uma maior granularidade para pesquisas no Portal da marca. Todos [os predicados adicionados](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) no formulário de pesquisa estão disponíveis para usuários como aspectos de pesquisa em filtros de pesquisa.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se você estiver disposto a usar o Painel de pesquisa de administração **[!UICONTROL de ativos de pesquisa personalizada]** da instância do autor de AEM, em vez de recriar o mesmo formulário no Portal de marca, poderá publicar o formulário de pesquisa personalizado da instância de autor de AEM no Portal da marca.

>[!NOTE]
>
>O painel de pesquisa de administração de **[!UICONTROL ativos de pesquisa bloqueada]** nos ativos AEM não pode ser publicado no Portal da marca a menos que seja editado. Depois de editado e publicado no Brand Portal, esse formulário de pesquisa substitui o formulário de pesquisa no Brand Portal.

Para publicar a faceta de pesquisa editada da instância de autor de AEM no Portal da marca:

1. Toque/clique no logotipo do AEM e vá até **[!UICONTROL Ferramentas]** &gt; **[!UICONTROL Geral]** &gt; **[!UICONTROL Pesquisar formulários]**.
2. Selecione o formulário de pesquisa editado e selecione **[!UICONTROL Publicar no portal da marca]**.

   >[!NOTE]
   >
   >Quando os usuários clicam **[!UICONTROL em Publicar no portal da marca]**, os aspectos de pesquisa são colocados na fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de formulários de pesquisa no Brand Portal:

1. Na instância Autor de AEM, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Geral &gt; Formulários de pesquisa]**.
2. Selecione o formulário de pesquisa e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

>[!NOTE]
>
>A **[!UICONTROL ação Cancelar publicação da marca do Brand Portal]** deixa o formulário de pesquisa padrão no Brand Portal e não restaura para o último formulário de pesquisa usado antes da publicação.

### Limitações {#limitations}

1. Alguns predicados de pesquisa não se aplicam a filtros de pesquisa no Portal da marca. Quando esses predicados de pesquisa são publicados como parte do formulário de pesquisa da instância de autor de AEM para o Brand Portal, são filtrados. Os usuários, portanto, veem menos números de previsão no formulário publicado no Portal da marca. Consulte [predicados de pesquisa aplicáveis a filtros no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. Para [!UICONTROL o Predicado de opções], se um usuário estiver usando qualquer caminho personalizado para ler opções na instância Autor de AEM, ele não funcionará no Portal da marca. Esses caminhos e opções adicionais não são publicados no Brand Portal com o formulário de pesquisa. Nesse caso, os usuários podem selecionar a opção **[!UICONTROL Manual]** em **[!UICONTROL Adicionar opções]** no **[!UICONTROL Predicado de opções]** para adicionar essas opções manualmente no Portal da marca.

![](assets/options-predicate-manual.png)
