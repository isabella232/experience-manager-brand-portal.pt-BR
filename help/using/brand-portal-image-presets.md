---
title: Aplicar predefinições de imagens ou representações dinâmicas
seo-title: Aplicar predefinições de imagens ou representações dinâmicas
description: 'Como uma macro, uma predefinição de imagens é uma coleção predefinida de comandos de tamanho e formatação salvos com um nome. As predefinições de imagens permitem que o AEM Assets Brand Portal forneça dinamicamente imagens de tamanhos, formatos e propriedades diferentes. '
seo-description: 'Como uma macro, uma predefinição de imagens é uma coleção predefinida de comandos de tamanho e formatação salvos com um nome. As predefinições de imagens permitem que o AEM Assets Brand Portal forneça dinamicamente imagens de tamanhos, formatos e propriedades diferentes. '
uuid: a 3 c 8705 c -5 fbd -472 c -8 b 61-f 65 b 3 e 552 c 1 b
content-type: referência
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: a 512 dfa 0-fef 3f-a 3f-f-a 389-a 0 a 3 a 7415 bac
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Aplicar predefinições de imagens ou representações dinâmicas {#apply-image-presets-or-dynamic-renditions}

Como uma macro, uma predefinição de imagens é uma [!UICONTROL coleção] predefinida de comandos de tamanho e formatação salvos com um nome. As predefinições de imagens permitem [!DNL AEM] que os ativos [!DNL Brand Portal] forneçam dinamicamente imagens de tamanhos, formatos e propriedades diferentes.

Uma predefinição de imagens é usada para gerar representações dinâmicas de imagens que podem ser visualizadas e baixadas. Ao visualizar imagens e suas execuções, você pode escolher uma predefinição para reformatar imagens nas especificações definidas pelo Administrador.

Para exibir representações dinâmicas de um ativo em [!DNL Brand Portal], certifique-se de que sua execução PTIFF existe na instância [!DNL AEM] do autor de onde você publica [!DNL Brand Portal]. Ao publicar o ativo, sua execução PTIFF também é publicada [!DNL Brand Portal]. Não há forma de gerar a execução do PTIFF [!DNL Brand Portal].

>[!NOTE]
>
>Ao baixar imagens e suas execuções, não há opção para escolher uma das predefinições existentes. Em vez disso, é possível especificar as propriedades de uma predefinição de imagem personalizada. Para obter mais informações, consulte [Aplicar predefinições de imagens ao baixar imagens](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Para obter mais informações sobre os parâmetros necessários ao criar predefinições de imagens, consulte [Gerenciando predefinições]de imagens (https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM].

## Criar uma predefinição de imagens {#create-an-image-preset}

Os administradores podem criar predefinições de imagens que aparecem como representações dinâmicas na página de detalhes do ativo. É possível criar uma predefinição de imagem do zero ou salvar uma existente com um novo nome. Ao criar uma predefinição de imagens, escolha um tamanho para a entrega de imagens e os comandos de formatação. Quando uma imagem é entregue para exibição, sua aparência é otimizada de acordo com os comandos escolhidos.
Observe que somente administradores podem criar predefinições de imagens.[!DNL Brand Portal]

Observe que somente administradores podem criar predefinições de imagens.[!DNL Brand Portal]

>[!NOTE]
>
>As execuções dinâmicas são criadas para os ativos para os quais PTIFF está disponível. Assim, se um ativo não tiver a execução Pyramid TIFF criada [!DNL AEM] e publicada, [!DNL Brand Portal]somente as representações do sistema poderão ser exportadas, mas as representações dinâmicas serão apresentadas como uma opção.
O modo Dynamic Media híbrido deve ser ativado ( [!DNL AEM] autor) para criar pirâmide (ptiff) de um ativo. Quando um ativo é publicado, [!DNL Brand Portal]as predefinições de imagens são aplicadas e as representações dinâmicas são exibidas.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   !![](assets/[!DNL AEM]logo. png)

2. No painel de ferramentas administrativas, clique em Predefinições **de imagens**.

   ![](assets/admin-tools-panel-4.png)

3. Na página de predefinições de imagens, clique **em Criar**.

   ![](assets/image_preset_homepage.png)

4. Na página **Editar predefinição de imagem** , digite os valores nas guias **Básico** e **Avançado** conforme apropriado, incluindo um nome. As opções são descritas em Opções de predefinição [de imagens](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)[!DNL AEM]. As predefinições aparecem no painel esquerdo e podem ser usadas dinamicamente com outros ativos.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Você também pode usar a página **Editar predefinição de imagem** para editar as propriedades de uma predefinição de imagem existente. Para editar uma predefinição de imagens, selecione-a na página de predefinições de imagens e clique **em Editar**.

5. Clique em **Salvar**. A predefinição de imagens é criada e exibida na página de predefinições de imagens.
6. Para excluir uma predefinição de imagens, selecione-a na página predefinições de imagens e clique **em Excluir**. Na página de confirmação, clique **em Excluir** para confirmar a exclusão. A predefinição de imagens é removida da página predefinições de imagens.

## Aplicar predefinições de imagens ao visualizar imagens {#apply-image-presets-when-previewing-images}

Ao visualizar imagens e suas execuções, escolha uma das predefinições existentes para reformatar imagens nas especificações definidas pelo Administrador.

1. Na [!DNL Brand Portal] interface, clique em uma imagem para abri-la.
2. Clique no ícone de sobreposição à esquerda e escolha **Representações**.

   ![](assets/image-preset-previewrenditions.png)

3. Na lista **Representações** , selecione a execução dinâmica apropriada, por exemplo, **Miniatura**. A imagem de visualização é renderizada com base na sua escolha da execução.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Aplicar predefinições de imagens ao baixar imagens {#apply-image-presets-when-downloading-images}

Ao baixar imagens e suas execuções, [!DNL Brand Portal]não é possível escolher as predefinições de imagens existentes. No entanto, é possível personalizar propriedades predefinidas de imagens com base nas quais você deseja reformatar as imagens.

1. Na [!DNL Brand Portal] interface, execute um dos procedimentos a seguir:

   * Passe o ponteiro do mouse sobre a imagem que deseja baixar. Nas miniaturas de ação rápida disponíveis, clique no **ícone Download** .
   ![](assets/downloadsingleasset.png)

   * Selecione a imagem que deseja baixar. Na barra de ferramentas na parte superior, clique no **ícone Download** .
   ![](assets/downloadassets.png)

2. Na caixa de diálogo **Download** , selecione as opções necessárias, dependendo se você deseja baixar o ativo com ou sem suas execuções.

   ![](assets/donload-assets-dialog.png)

3. Para baixar representações dinâmicas do ativo, selecione a **opção Representações** dinâmicas.
4. Personalize as propriedades predefinidas de imagens com base nos quais você deseja reformatar dinamicamente a imagem e suas execuções durante o download. Especifique o tamanho, o formato, o espaço da cor, a resolução e modificador de imagem.

   ![](assets/dynamicrenditions.png)

5. Clique **em Download**. As representações dinâmicas personalizadas são baixadas em um arquivo ZIP junto com a imagem e as representações que você escolheu baixar. No entanto, nenhum arquivo zip é criado se um único ativo for baixado, o que garante o download rápido.
