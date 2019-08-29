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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Publicar predefinições, esquemas e facetas no Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

O artigo entra em predefinições de imagens de publicação, esquemas de metadados e aspectos de pesquisa personalizados a [!DNL AEM] partir da instância do Autor para [!DNL Brand Portal]. A capacidade de publicação permite que as organizações reutilizem as predefinições de imagens, esquemas de metadados e aspectos de pesquisa criados/modificados na [!DNL AEM] instância do Autor, reduzindo os esforços duplicados.

>[!NOTE]
>
>A capacidade de publicar predefinições de imagens, esquema de metadados e facetas de pesquisa da [!DNL AEM] instância Autor está [!DNL Brand Portal] disponível [!DNL AEM 6.2 SP1-CFP7] e [!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] em seguida.

## Publicar predefinições de imagens no Brand Portal {#publish-image-presets-to-brand-portal}

As predefinições de imagens são um conjunto de comandos de dimensionamento e formatação aplicados à imagem no momento da entrega de imagens. As predefinições de imagens podem ser criadas e modificadas em [!DNL Brand Portal]. Como alternativa, se [!DNL AEM] a instância do Autor estiver sendo executada no modo de mídia dinâmica, os usuários poderão criar predefinições no [!DNL AEM] autor e publicá-las [!DNL AEM Assets Brand Portal]e evitar recriar as mesmas predefinições em [!DNL Brand Portal].\
Uma vez que a predefinição é criada, ela é listada como representação dinâmica no painel de representações de detalhes do ativo e no diálogo de download.

>[!NOTE]
>
>Se [!DNL AEM] a instância do Autor não estiver sendo executada no [!DNL Dynamic Media] Modo (o cliente não comprou [!DNL Dynamic Media]), [!UICONTROL a execução TIFF] Piraxid dos ativos não será criada no momento do upload. As predefinições de imagens ou as representações dinâmicas funcionam em [!UICONTROL TIFF Pirâmico] de um ativo, portanto, se [!UICONTROL o TIFF] Pirâmide não estiver disponível na [!DNL AEM] instância do Autor, ele não estará disponível [!DNL Brand Portal] também. Como resultado, nenhuma representação dinâmica está presente no painel de representações da página de detalhes do ativo e no diálogo de download.

Para publicar predefinições de imagens em [!DNL Brand Portal]:

1. Na [!DNL AEM] instância Autor, toque/clique no [!DNL AEM] logotipo para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos]** &gt; Predefinições **[!UICONTROL de imagens]**.
2. Selecione a predefinição de imagens ou várias predefinições de imagens na lista de predefinições de imagens e clique/toque **[!UICONTROL em Publicar no portal da marca]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando os usuários clicam **[!UICONTROL em Publicar no portal]** da marca, as predefinições de imagens são colocadas em fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de uma predefinição de imagem:[!DNL Brand Portal]

1. Na [!DNL AEM] instância Autor, toque/clique no [!DNL AEM] logotipo para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos]** &gt; Predefinições **[!UICONTROL de imagens]**.
2. Selecione uma predefinição de imagens e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

## Publicar esquema de metadados no Brand Portal {#publish-metadata-schema-to-brand-portal}

O esquema de metadados descreve o layout e as propriedades exibidas na página de propriedades de ativos/coleções.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se os usuários editarem o esquema padrão na [!DNL AEM] instância do Autor e estiverem dispostos a usar o mesmo esquema do esquema padrão, poderão simplesmente [!DNL Brand Portal]publicar os formulários de esquema de metadados para [!DNL Brand Portal]. Nesse cenário, o esquema padrão é [!DNL Brand Portal] substituído pelos esquemas padrão publicados a partir da instância [!DNL AEM] do Autor.

Se os usuários criaram um esquema personalizado na [!DNL AEM] instância do Autor, poderão publicar o esquema personalizado em [!DNL Brand Portal] vez de recriar o mesmo esquema personalizado nele. Os usuários podem aplicar esse esquema personalizado a qualquer pasta/coleção no [!DNL Brand Portal].

>[!NOTE]
>
>Os esquemas padrão não podem ser publicados no [!DNL Brand Portal] caso de bloqueio na [!DNL AEM] instância (ou seja, não são editados).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se uma pasta tiver um esquema aplicado a [!DNL AEM] instância do Autor, o mesmo esquema também deverá existir [!DNL Brand Portal] para manter a consistência na página de propriedades do ativo no [!DNL AEM] Autor e [!DNL Brand portal].

Para publicar um esquema de metadados da [!DNL AEM] instância do Autor para [!DNL Brand Portal]:

1. Na [!DNL AEM] instância Autor, toque/clique no logotipo do AEM para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos]** &gt; **[!UICONTROL Esquemas de metadados]**.
2. Selecione um esquema de metadados e selecione **[!UICONTROL Publicar no portal da marca]** com as opções disponíveis na parte superior.

>[!NOTE]
>
>Quando os usuários clicam **[!UICONTROL em Publicar no Brand Portal]**, os esquemas de metadados são colocados na fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de um esquema de metadados:[!DNL Brand Portal]

1. Na [!DNL AEM] instância Autor, toque/clique no [!DNL AEM] logotipo para acessar o console de navegação global e tocar/clicar no ícone Ferramentas e navegue até **[!UICONTROL Ativos]** &gt; **[!UICONTROL Esquemas de metadados]**.
2. Selecione um esquema de metadados e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

## Publicar aspectos de pesquisa no Brand Portal {#publish-search-facets-to-brand-portal}

Os formulários de pesquisa fornecem a capacidade de [pesquisa por facetas](../using/brand-portal-search-facets.md) para os usuários. [!DNL Brand Portal] Os aspectos de pesquisa aprimoram a granularidade maior para pesquisas. [!DNL Brand Portal] Todos [os predicados adicionados](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) no formulário de pesquisa estão disponíveis para usuários como aspectos de pesquisa em filtros de pesquisa.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se você estiver disposto a usar o Painel de pesquisa do Administrador **[!UICONTROL de pesquisa personalizado de ativos]** da [!DNL AEM] instância do Autor, em vez de recriar o mesmo formulário, [!DNL Brand Portal] poderá publicar o formulário de pesquisa personalizado a partir [!DNL AEM] da instância do Autor para [!DNL Brand Portal].

>[!NOTE]
>
>O painel de pesquisa de administração de **[!UICONTROL ativos de pesquisa bloqueada]** nos ativos AEM não pode ser publicado [!DNL Brand Portal] a menos que seja editado. Depois de editado e publicado, [!DNL Brand Portal]esse formulário de pesquisa substitui o formulário de pesquisa em [!DNL Brand Portal].

Para publicar a faceta de pesquisa editada da [!DNL AEM] instância do Autor para [!DNL Brand Portal]:

1. Toque/clique no [!DNL AEM] logotipo e vá para **[!UICONTROL Ferramentas]** &gt; **[!UICONTROL Geral]** &gt; **[!UICONTROL Pesquisar formulários]**.
2. Selecione o formulário de pesquisa editado e selecione **[!UICONTROL Publicar no portal da marca]**.

   >[!NOTE]
   >
   >Quando os usuários clicam **[!UICONTROL em Publicar no portal da marca]**, os aspectos de pesquisa são colocados na fila para publicação. Recomenda-se que os usuários monitorem o log dos agentes de replicação para confirmar se a publicação foi bem-sucedida.

Para cancelar a publicação de formulários de pesquisa:[!DNL Brand Portal]

1. Na [!DNL AEM] instância Autor, toque/clique no [!DNL AEM] logotipo para acessar o console de navegação global e toque/clique no ícone Ferramentas e navegue até **[!UICONTROL Geral]** &gt; Formulários **[!UICONTROL de pesquisa]**.
2. Selecione o formulário de pesquisa e selecione **[!UICONTROL Remover do portal da marca]** das opções disponíveis na parte superior.

>[!NOTE]
>
>A **[!UICONTROL ação Cancelar publicação da marca do Brand Portal]** deixa o formulário de pesquisa padrão no Brand Portal e não restaura para o último formulário de pesquisa usado antes da publicação.

### Limitações {#limitations}

1. Alguns predicados de pesquisa não se aplicam a filtros de pesquisa no [!DNL Brand Portal]. Quando esses predicados de pesquisa são publicados como parte do formulário de pesquisa a partir da instância [!DNL AEM] do Autor para [!DNL Brand Portal], são filtrados. Os usuários, portanto, veem menos números de previsão no formulário publicado no [!DNL Brand Portal]. Consulte [predicados de pesquisa aplicáveis a filtros no Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. Para [!UICONTROL o predicado Opções] , se um usuário estiver usando qualquer caminho personalizado para ler opções na instância Autor de AEM, ele não funcionará no Portal da marca. Esses caminhos e opções adicionais não são publicados no Brand Portal com o formulário de pesquisa. Nesse caso, os usuários podem selecionar a opção **[!UICONTROL Manual]** em **[!UICONTROL Adicionar opções]** no **[!UICONTROL Predicado de opções]** para adicionar essas opções manualmente.[!DNL Brand Portal]

![](assets/options-predicate-manual.png)
