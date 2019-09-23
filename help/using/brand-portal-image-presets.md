---
title: Aplicar predefinições de imagens ou representações dinâmicas
seo-title: Aplicar predefinições de imagens ou representações dinâmicas
description: 'Como uma macro, uma predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos com um nome. As predefinições de imagens permitem que o AEM Assets Brand Portal forneça dinamicamente imagens de tamanhos, formatos e propriedades diferentes. '
seo-description: 'Como uma macro, uma predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos com um nome. As predefinições de imagens permitem que o AEM Assets Brand Portal forneça dinamicamente imagens de tamanhos, formatos e propriedades diferentes. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: referência
topic-tags: administração
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: c0169450c5cf1d8c99f8604df3bd2667445ff1ed

---


# Aplicar predefinições de imagens ou representações dinâmicas {#apply-image-presets-or-dynamic-renditions}

Como uma macro, uma predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos com um nome. As predefinições de imagens permitem que o AEM Assets Brand Portal forneça dinamicamente imagens de tamanhos, formatos e propriedades diferentes.

Uma predefinição de imagem é usada para gerar representações dinâmicas de imagens que podem ser visualizadas e baixadas. Ao visualizar imagens e suas representações, você pode escolher uma predefinição para reformatar imagens de acordo com as especificações definidas pelo administrador.

Para exibir representações dinâmicas de um ativo no Brand Portal, verifique se a execução tiff em pirâmide existe na instância do autor do AEM de onde você publica no Brand Portal. Quando você publica o ativo, sua execução PTIFF também é publicada no Brand Portal. Não há como gerar a execução PTIFF do Brand Portal.

>[!NOTE]
>
>Ao baixar imagens e suas representações, não há opção para escolher entre as predefinições existentes. Em vez disso, você pode especificar as propriedades de uma predefinição de imagem personalizada. Para obter mais informações, consulte [Aplicar predefinições de imagens ao baixar imagens](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Para obter mais informações sobre os parâmetros necessários ao criar predefinições de imagens, consulte [Gerenciamento de predefinições](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)de imagens.

## Criar uma predefinição de imagem {#create-an-image-preset}

Os administradores podem criar predefinições de imagens que aparecem como representações dinâmicas na página de detalhes do ativo. Você pode criar uma predefinição de imagem do zero ou salvar uma existente com um novo nome. Ao criar uma predefinição de imagem, escolha um tamanho para a entrega da imagem e os comandos de formatação. Quando uma imagem é entregue para exibição, sua aparência é otimizada de acordo com os comandos escolhidos.
Observe que somente os administradores podem criar predefinições de imagens no Brand Portal.

Observe que somente os administradores podem criar predefinições de imagens no Brand Portal.

>[!NOTE]
>
>As representações dinâmicas são criadas para os ativos para os quais o PTIFF está disponível. Portanto, se um ativo não tiver renderização de TIFF em pirâmide criada no AEM e publicada no Brand Portal, somente as renderizações do sistema poderão ser exportadas, mas as renderizações dinâmicas serão apresentadas como uma opção.
O modo Híbrido de mídia dinâmica deve estar habilitado no AEM (autor) para criar um tiff de pirâmide de um ativo. Quando esse ativo é publicado no Brand Portal, as predefinições de imagem são aplicadas e as representações dinâmicas são exibidas.

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

2. No painel de ferramentas administrativas, clique em Predefinições **[!UICONTROL de imagem]**.

   ![](assets/admin-tools-panel-4.png)

3. Na página de predefinições de imagens, clique em **[!UICONTROL Criar]**.

   ![](assets/image_preset_homepage.png)

4. Na página **[!UICONTROL Editar predefinição]** de imagem, digite valores nas guias **[!UICONTROL Básico]** e **[!UICONTROL Avançado]** , conforme apropriado, incluindo um nome. As opções são descritas nas opções [Predefinição de](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)imagem. As predefinições aparecem no painel esquerdo e podem ser usadas dinamicamente com outros ativos.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Você também pode usar a página **[!UICONTROL Editar predefinição]** de imagem para editar as propriedades de uma predefinição de imagem existente. Para editar uma predefinição de imagem, selecione-a na página de predefinições de imagem e clique em **[!UICONTROL Editar]**.

5. Clique em **[!UICONTROL Salvar]**. A predefinição de imagem é criada e exibida na página de predefinições de imagem.
6. Para excluir uma predefinição de imagem, selecione-a na página de predefinições de imagem e clique em **[!UICONTROL Excluir]**. Na página de confirmação, clique em **[!UICONTROL Excluir]** para confirmar a exclusão. A predefinição de imagem é removida da página de predefinições de imagem.

## Aplicar predefinições de imagens ao visualizar imagens {#apply-image-presets-when-previewing-images}

Ao visualizar imagens e suas representações, escolha entre as predefinições existentes para reformatar imagens de acordo com as especificações definidas pelo administrador.

1. Na interface do Brand Portal, clique em uma imagem para abri-la.
2. Clique no ícone de sobreposição à esquerda e escolha **[!UICONTROL Representações]**.

   ![](assets/image-preset-previewrenditions.png)

3. Na lista **[!UICONTROL Representações]** , selecione a representação dinâmica apropriada, por exemplo, **[!UICONTROL Miniatura]**. A imagem de visualização é renderizada com base na sua escolha da representação.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Aplicar predefinições de imagens ao baixar imagens {#apply-image-presets-when-downloading-images}

Ao baixar imagens e suas representações do Brand Portal, não é possível escolher entre as predefinições de imagens existentes. Entretanto, é possível personalizar as propriedades predefinidas da imagem com base nas quais deseja reformatar as imagens.

1. Na interface do Brand Portal, execute um dos procedimentos a seguir:

   * Passe o ponteiro do mouse sobre a imagem que deseja baixar. Nas miniaturas de ação rápida disponíveis, clique no ícone **[!UICONTROL Download]** .
   ![](assets/downloadsingleasset.png)

   * Selecione a imagem que deseja baixar. Na barra de ferramentas na parte superior, clique no ícone **[!UICONTROL Download]** .
   ![](assets/downloadassets.png)

2. Na caixa de diálogo **[!UICONTROL Download]** , selecione as opções necessárias, dependendo se você deseja baixar o ativo com ou sem suas representações.

   ![](assets/donload-assets-dialog.png)

3. Para baixar representações dinâmicas do ativo, selecione a opção Representações **[!UICONTROL dinâmicas]** .
4. Personalize as propriedades predefinidas da imagem com base nas quais você deseja reformatar dinamicamente a imagem e suas representações durante o download. Especifique o modificador de tamanho, formato, espaço de cor, resolução e imagem.

   ![](assets/dynamicrenditions.png)

5. Clique em **[!UICONTROL Download]**. As renderizações dinâmicas personalizadas são baixadas em um arquivo ZIP juntamente com a imagem e as renderizações que você escolheu baixar. No entanto, nenhum arquivo zip será criado se um único ativo for baixado, garantindo o download rápido.
