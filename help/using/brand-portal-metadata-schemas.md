---
title: Usar o formulário de esquema de metadados
seo-title: Usar o formulário de esquema de metadados
description: Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o esquema específico. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: referência
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administração
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Use the metadata schema form {#use-the-metadata-schema-form}

A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.

The Properties page for each asset includes default metadata properties depending upon the MIME type of the asset. **** Administrators can use the Metadata Schema Editor to modify existing schemas or add custom metadata schemas. AEM Assets Brand Portal provides default forms for assets of various MIME types. However, you can also add custom forms for such assets.

## Add a metadata schema form {#add-a-metadata-schema-form}

To create a new metadata schema form, do the following:

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em Esquemas **[!UICONTROL de metadados]**.

   ![](assets/navigation-panel.png)

1. Na página Formulários **[!UICONTROL de esquema de]** metadados, clique em **[!UICONTROL Criar]**.

   ![](assets/create-metadata-schema-form.png)

1. Na caixa de diálogo **[!UICONTROL Criar formulário]** de esquema, especifique o título do formulário de esquema e clique em **[!UICONTROL Criar]** para concluir o processo de criação do formulário.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

É possível editar um formulário de esquema de metadados recém-adicionado ou existente. O formulário de esquema de metadados contém conteúdo derivado de seu pai, incluindo guias e itens de formulário dentro de guias. É possível mapear ou configurar esses itens de formulário para um campo dentro de um nó de metadados.

É possível adicionar novas guias ou itens de formulário ao formulário de esquema de metadados. As guias derivadas e os itens de formulário (do pai) estão no estado bloqueado. Não é possível alterá-los no nível da criança.

Para editar um formulário de esquema de metadados, faça o seguinte:

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em Esquemas **[!UICONTROL de metadados]**.
1. Na página Formulários **[!UICONTROL de esquema de]** metadados, selecione um formulário de esquema para editar suas propriedades, por exemplo, **[!UICONTROL coleção]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Os modelos desatualizados exibem um símbolo de cadeado antes deles. Se você personalizar qualquer um dos modelos, o símbolo de Bloqueio antes do modelo desaparecerá.

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Editar]**.

   A página Editor **[!UICONTROL de esquema de]** metadados é aberta com a guia **[!UICONTROL Básico]** aberta à esquerda e a guia **[!UICONTROL Criar formulário]** é aberta à direita.

1. Na página Editor **[!UICONTROL de esquema de]** metadados, personalize a página **[!UICONTROL Propriedades]** do ativo arrastando um ou mais componentes de uma lista de tipos de componentes na guia **[!UICONTROL Criar formulário]** para a guia **[!UICONTROL Básico]** .

   ![](assets/metadata-schemaeditor-page.png)

1. Para configurar um componente, selecione-o e modifique suas propriedades na guia **[!UICONTROL Configurações]** .

### Componentes na guia Criar formulário {#components-in-the-build-form-tab}

A guia **[!UICONTROL Criar formulário]** lista itens que podem ser usados no formulário de esquema. A guia **[!UICONTROL Configurações]** fornece os atributos de cada item selecionado na guia **[!UICONTROL Criar formulário]** . A tabela a seguir lista os itens de formulário disponíveis na guia **[!UICONTROL Criar formulário]** :

| Component Name | Descrição |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Título da seção] | Adicione um cabeçalho de seção para obter uma lista de componentes comuns. |
| [!UICONTROL Texto em linha única] | Adicione uma única propriedade de texto de linha. É armazenado como uma string. |
| [!UICONTROL Multi-ValueText] | Adicione uma propriedade de texto de vários valores. Ele é armazenado como uma matriz de string. |
| [!UICONTROL Número] | Add a number component. |
| [!UICONTROL Data] | Add a date component. |
| [!UICONTROL Lista suspensa] | Add a dropdown list. |
| [!UICONTROL Tags padrão] | Adicionar uma tag. **** Observação: Os administradores podem precisar alterar o valor do caminho, por exemplo, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`se publicarem o formulário de esquema de metadados do AEM, onde o caminho não inclui informações de locatário, por exemplo, `/etc/tags/<custom_tag_namespace>`. |
| [!UICONTROL Tags inteligentes] | Tags detectadas automaticamente se você adquiriu e configurou o complemento de tags inteligentes do AEM. |
| [!UICONTROL Campo oculto] | Add a hidden field. It is sent as a POST parameter when the asset is saved. |
| [!UICONTROL Ativo referenciado por] | Adicione este componente para exibir a lista de ativos referenciados pelo ativo. |
| [!UICONTROL Fazer referência ao ativo] | Add to display a list of assets that reference the asset. |
| [!UICONTROL Classificação do ativo] | Average rating of an asset added from AEM Assets before it is published to Brand Portal. |
| [!UICONTROL Metadados do contexto] | Adicione para controlar a exibição de outras guias de metadados na página Propriedades dos ativos. |

>[!NOTE]
>
>Do not use Product References, as it is not functional.****

#### Edit the metadata component {#edit-the-metadata-component}

Para editar as propriedades de um componente de metadados no formulário, clique no componente e edite suas propriedades na guia **[!UICONTROL Configurações]** .

* **[!UICONTROL Rótulo]** do campo: O nome da propriedade de metadados exibida na página Propriedades do ativo.

* **[!UICONTROL Mapear para propriedade]**: O valor dessa propriedade fornece o caminho/nome relativo para o nó do ativo no qual ele é salvo no repositório CRX. Começa com "**./**" porque indica que o caminho está sob o nó do ativo.

Estes são os valores válidos para esta propriedade:

— [!UICONTROL `./jcr:content/metadata/dc:title`]: Armazena o valor no nó de metadados do ativo como a propriedade [!UICONTROL `dc:title`].

— [!UICONTROL `./jcr:created`]: Exibe a propriedade jcr no nó do ativo. Se você configurar essas propriedades nas propriedades de exibição, recomendamos marcá-las como Desativar edição, pois elas estão protegidas. Caso contrário, o erro "O(s) ativo(s) falhou(m) em modificar" ocorre quando você salva as propriedades do ativo.

* **[!UICONTROL Espaço reservado]**: Use essa propriedade para fornecer ao usuário quaisquer informações relevantes sobre a propriedade de metadados.
* **[!UICONTROL Obrigatório]**: Use essa propriedade para marcar uma propriedade de metadados como obrigatória na página Propriedades.
* **[!UICONTROL Desativar edição]**: Use essa propriedade para tornar uma propriedade de metadados não editável na página Propriedades.
* **[!UICONTROL Mostrar campo vazio em somente]** leitura: Marque essa propriedade para exibir uma propriedade de metadados na página Propriedades mesmo se ela não tiver valor. Por padrão, quando uma propriedade de metadados não tem valor, ela não é listada na página Propriedades.
* **[!UICONTROL Descrição]**: Use essa propriedade para adicionar uma breve descrição para o componente de metadados.
* **[!UICONTROL Ícone]** Excluir: Clique nesse ícone para excluir um componente do formulário de esquema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos os campos de metadados são somente leitura no formulário editor de metadados de um ativo. Como os metadados do ativo devem ser editados nos ativos AEM antes que um ativo seja publicado no Brand Portal.

#### Adicionar ou excluir uma guia no formulário de esquema {#add-or-delete-a-tab-in-the-schema-form}

O formulário de esquema padrão inclui as guias **[!UICONTROL Básico]** e **[!UICONTROL Avançado]** . O editor de esquema permite adicionar ou excluir uma guia.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para adicionar uma nova guia em um formulário de esquema, clique em **[!UICONTROL +]**. Por padrão, a nova guia tem o nome "Sem nome-1". É possível modificar o nome na guia **[!UICONTROL Configurações]** .

![](assets/add-tab-metadata-form.png)

* Para excluir uma guia, clique em **[!UICONTROL x]**. Click **[!UICONTROL Save]** to save the changes.

## Aplicar um esquema de metadados a uma pasta {#apply-a-metadata-schema-to-a-folder}

Brand Portal allows you to customize and control the metadata schema so that the Properties page of an asset displays only the specific information you choose to reveal.  Para controlar os metadados exibidos na página [!UICONTROL Propriedades] , remova os metadados necessários do formulário de esquema de metadados e aplique-os à pasta específica.

Para aplicar um formulário de esquema de metadados a uma pasta, faça o seguinte:

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em Esquemas **[!UICONTROL de metadados]**.

1. Na página Formulários **[!UICONTROL de esquema de]** metadados, selecione o formulário de esquema que deseja aplicar a um ativo, por exemplo, [!UICONTROL roupas].

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Aplicar às pastas]**.

1. Na página **[!UICONTROL Selecionar pasta(s)]** , navegue até a pasta à qual deseja aplicar o esquema de metadados de **[!UICONTROL roupas]** , por exemplo, **[!UICONTROL Luvas]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. Clique em **[!UICONTROL Aplicar]** para aplicar o formulário de esquema de metadados à pasta.

   Os metadados disponíveis no formulário de esquema de metadados do **[!UICONTROL vestuário]** são aplicados à pasta **[!UICONTROL Luvas]** e são visíveis na página **[!UICONTROL Propriedades]** da pasta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se você aplicar um esquema que inclui esquemas aninhados a uma pasta que contém arquivos de vídeo, as propriedades de metadados dos arquivos de vídeo poderão não ser renderizadas corretamente. Para garantir que as propriedades de metadados sejam renderizadas corretamente, remova os esquemas aninhados e aplique somente o esquema pai à pasta.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

O Brand Portal permite que você exclua apenas formulários de esquema personalizados. Isso não permite excluir os formulários/modelos de esquema padrão. No entanto, é possível excluir quaisquer alterações personalizadas nesses formulários.

Para excluir um formulário, selecione-o e clique no ícone **[!UICONTROL Excluir]** .

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Após excluir as alterações personalizadas feitas em um formulário padrão, o símbolo **[!UICONTROL Bloquear]** será exibido novamente antes do nome do formulário na interface do Esquema de metadados para indicar que o formulário foi revertido para seu estado padrão.

## Formulários de esquema para TIPOS MIME {#schema-forms-for-mime-types}

### Adicionar novos formulários para tipos MIME {#adding-new-forms-for-mime-types}

Além dos formulários padrão, você pode adicionar formulários personalizados para ativos de vários tipos MIME ou criar um novo formulário em um tipo de formulário apropriado. Por exemplo, para adicionar um novo modelo para o subtipo **[!UICONTROL image/png]** , crie o formulário sob os formulários "image". O título do formulário de esquema é o nome do subtipo. Neste caso, o título é "png".

#### Uso de um modelo de esquema existente para vários tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Você pode usar um modelo existente para um tipo MIME diferente. Por exemplo, use o formulário **image/jpeg** para ativos do tipo MIME **image/png**.

Nesse caso, crie um novo nó [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] no repositório CRX. Especifique um nome para o nó e defina as seguintes propriedades:

| **Nome** | **Tipo** | **Valor** |
|---|---|---|
| exposedmimetype | Sequência de caracteres | image/jpeg |
| mimetypes | Sequência de caracteres[] | image/png |

* **exposedmimetype**: Nome do formulário existente a ser mapeado
* **mimetypes**: Lista de tipos MIME que usam o formulário definido no atributo **exposedmimetype**

O Brand Portal mapeia os seguintes tipos MIME e formulários de esquema:

| **Formulário de esquema** | **Tipos MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| vídeo/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

A seguir está uma lista de propriedades de metadados padrão:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
