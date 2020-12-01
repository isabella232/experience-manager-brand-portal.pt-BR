---
title: Usar o formulário de esquema de metadados
seo-title: Usar o formulário de esquema de metadados
description: Um schema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o schema em particular. O schema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
seo-description: Um schema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o schema em particular. O schema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1756'
ht-degree: 12%

---


# Usar o formulário de esquema de metadados {#use-the-metadata-schema-form}

Um schema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o schema em particular. O schema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.

A página **[!UICONTROL Propriedades]** para cada ativo inclui propriedades de metadados padrão dependendo do tipo MIME do ativo. Os administradores podem usar o Editor de Schemas de Metadados para modificar schemas existentes ou adicionar schemas de metadados personalizados. O Portal de marcas da AEM Assets fornece formulários padrão para ativos de vários tipos MIME. No entanto, também é possível adicionar formulários personalizados para esses ativos.

## Adicionar um formulário de schema de metadados {#add-a-metadata-schema-form}

Para criar um novo formulário de schema de metadados, faça o seguinte:

1. Na barra de ferramentas AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Schemas de metadados]**.

   ![](assets/navigation-panel.png)

1. Na página **[!UICONTROL Forms]** Schema de metadados, clique em **[!UICONTROL Criar]**.

   ![](assets/create-metadata-schema-form.png)

1. Na caixa de diálogo **[!UICONTROL Criar formulário de Schema]**, especifique o título do formulário de Schema e clique em **[!UICONTROL Criar]** para concluir o processo de criação do formulário.

   ![](assets/create-schema-form.png)

## Editar um formulário de schema de metadados {#edit-a-metadata-schema-form}

É possível editar um formulário de schema de metadados recém-adicionado ou existente. O formulário de schema de metadados contém conteúdo derivado de seu pai, incluindo guias e itens de formulário dentro de guias. É possível mapear ou configurar esses itens de formulário para um campo dentro de um nó de metadados.

É possível adicionar novas guias ou itens de formulário ao formulário de schema de metadados. As guias derivadas e os itens de formulário (do pai) estão no estado bloqueado. Não é possível alterá-los no nível da criança.

Para editar um formulário de schema de metadados, faça o seguinte:

1. Na barra de ferramentas AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Schemas de metadados]**.
1. Na página **[!UICONTROL Schema de metadados Forms]**, selecione um formulário de schema para editar suas propriedades, por exemplo, **[!UICONTROL collection]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Os modelos desatualizados exibem um símbolo de cadeado antes deles. Se você personalizar qualquer um dos modelos, o símbolo de Bloqueio antes do modelo desaparecerá.

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Editar]**.

   A página **[!UICONTROL Editor de Schemas de metadados]** é aberta com a guia **[!UICONTROL Básico]** aberta à esquerda e a guia **[!UICONTROL Criar formulário]** aberta à direita.

1. Na página **[!UICONTROL Editor de Schemas de metadados]**, personalize a página **[!UICONTROL Propriedades]** do ativo arrastando um ou mais componentes de uma lista de tipos de componentes na guia **[!UICONTROL Criar formulário]** para a guia **[!UICONTROL Básico]**.

   ![](assets/metadata-schemaeditor-page.png)

1. Para configurar um componente, selecione-o e modifique suas propriedades na guia **[!UICONTROL Configurações]**.

### Componentes na guia Criar formulário {#components-in-the-build-form-tab}

A guia **[!UICONTROL Criar formulário]** lista itens que você pode usar no formulário de schema. A guia **[!UICONTROL Configurações]** fornece os atributos de cada item selecionado na guia **[!UICONTROL Criar formulário]**. A tabela a seguir lista os itens de formulário disponíveis na guia **[!UICONTROL Criar formulário]**:

| Nome do componente | Descrição |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL Título da seção]** | Adicione um cabeçalho de seção para uma lista de componentes comuns. |
| **[!UICONTROL Texto em linha única]** | Adicione uma única propriedade de texto de linha. É armazenado como uma string. |
| **[!UICONTROL Multi-ValueText]** | Adicione uma propriedade de texto de vários valores. Ele é armazenado como uma matriz de string. |
| **[!UICONTROL Número]** | Adicione um componente de número. |
| **[!UICONTROL Data]** | Adicione um componente de data. |
| **[!UICONTROL Lista suspensa]** | Adicione uma lista suspensa. |
| **[!UICONTROL Tags padrão]** | Adicionar uma tag. **Observação:** os administradores podem precisar alterar o valor do caminho, por exemplo,  `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`se publicarem o formulário de schema de metadados do AEM, no qual o caminho não inclui informações de locatário, por exemplo,  `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL Tags inteligentes]** | Tags detectadas automaticamente se você adquiriu e configurou o complemento de tags inteligentes AEM. |
| **[!UICONTROL Campo oculto]** | Adicionar um campo oculto. Ele é enviado como um parâmetro POST quando o ativo é salvo. |
| **[!UICONTROL Ativo referenciado por]** | Adicione esse componente à lista de visualização de ativos referenciados pelo ativo. |
| **[!UICONTROL Fazer referência ao ativo]** | Adicionar para exibir uma lista de ativos que fazem referência ao ativo. |
| **[!UICONTROL Classificação do ativo]** | Classificação média de um ativo adicionado da AEM Assets antes de ser publicado no Brand Portal. |
| **[!UICONTROL Metadados do contexto]** | Adicione para controlar a exibição de outras guias de metadados na página Propriedades dos ativos. |

>[!NOTE]
>
>Não use **[!UICONTROL Referências de produto]**, pois não está funcionando.

#### Editar o componente de metadados {#edit-the-metadata-component}

Para editar as propriedades de um componente de metadados no formulário, clique no componente e edite suas propriedades na guia **[!UICONTROL Configurações]**.

* **[!UICONTROL Rótulo]** do campo: O nome da propriedade de metadados exibida na página Propriedades do ativo.

* **[!UICONTROL Mapear para propriedade]**: O valor dessa propriedade fornece o caminho/nome relativo para o nó do ativo no qual ele é salvo no repositório CRX. Ele start com &quot;**./**&quot; porque indica que o caminho está sob o nó do ativo.

Estes são os valores válidos para esta propriedade:

-- `./jcr:content/metadata/dc:title`: armazena o valor no nó de metadados do ativo como a propriedade [!UICONTROL `dc:title`].

-- `./jcr:created`: exibe a propriedade jcr no nó do ativo. Se você configurar essas propriedades nas propriedades de exibição, recomendamos marcá-las como Desativar edição, pois elas estão protegidas. Caso contrário, o erro &quot;Os ativos falharam ao serem modificados&quot; ocorre ao salvar as propriedades do ativo.

* **[!UICONTROL Espaço reservado]**: Use essa propriedade para fornecer ao usuário quaisquer informações relevantes sobre a propriedade de metadados.
* **[!UICONTROL Obrigatório]**: Use essa propriedade para marcar uma propriedade de metadados como obrigatória na página Propriedades.
* **[!UICONTROL Desabilitar edição]**: Use essa propriedade para tornar uma propriedade de metadados não editável na página Propriedades.
* **[!UICONTROL Mostrar campo vazio em somente]** leitura: Marque essa propriedade para exibir uma propriedade de metadados na página Propriedades mesmo se ela não tiver valor. Por padrão, quando uma propriedade de metadados não tem valor, ela não é listada na página Propriedades.
* **[!UICONTROL Descrição]**: Use essa propriedade para adicionar uma breve descrição para o componente de metadados.
* **[!UICONTROL Ícone]** Excluir: Clique nesse ícone para excluir um componente do formulário de schema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos os campos de metadados são somente leitura no formulário editor de metadados de um ativo. Como os metadados do ativo devem ser editados no AEM Assets antes que um ativo seja publicado no Brand Portal.

#### Adicionar ou excluir uma guia no formulário de schema {#add-or-delete-a-tab-in-the-schema-form}

O formulário de schema padrão inclui as guias **[!UICONTROL Basic]** e **[!UICONTROL Advanced]**. O editor de esquema permite adicionar ou excluir uma guia.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para adicionar uma nova guia em um formulário de schema, clique em **[!UICONTROL +]**. Por padrão, a nova guia tem o nome &quot;Sem nome-1&quot;. É possível modificar o nome na guia **[!UICONTROL Settings]**.

![](assets/add-tab-metadata-form.png)

* Para excluir uma guia, clique em **[!UICONTROL x]**. Clique em **[!UICONTROL Salvar]** para salvar as alterações.

## Aplicar um schema de metadados a uma pasta {#apply-a-metadata-schema-to-a-folder}

O Brand Portal permite que você personalize e controle o schema de metadados para que a página **[!UICONTROL Propriedades]** de um ativo exiba apenas as informações específicas que você escolher revelar. Para controlar os metadados exibidos na página **[!UICONTROL Propriedades]**, remova os metadados necessários do formulário de schema de metadados e aplique-os à pasta específica.

Para aplicar um formulário de schema de metadados a uma pasta, faça o seguinte:

1. Na barra de ferramentas AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Schemas de metadados]**.

1. Na página **[!UICONTROL Schema de metadados Forms]**, selecione o formulário de schema que deseja aplicar a um ativo, por exemplo, **[!UICONTROL roupas]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Aplicar às pastas]**.

1. Na página **[!UICONTROL Selecionar pasta(s)]**, navegue até a pasta à qual deseja aplicar o schema de metadados **[!UICONTROL roupas]**, por exemplo, **[!UICONTROL Luvas]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. Clique em **[!UICONTROL Aplicar]** para aplicar o formulário de schema de metadados à pasta.

   Os metadados disponíveis no formulário de schema de metadados **[!UICONTROL roupas]** são aplicados à pasta **[!UICONTROL Luvas]** e são visíveis na página **[!UICONTROL Propriedades]** da pasta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se você aplicar um schema que inclui schemas aninhados a uma pasta que contém arquivos de vídeo, as propriedades de metadados dos arquivos de vídeo poderão não ser renderizadas corretamente. Para garantir que as propriedades de metadados sejam renderizadas corretamente, remova os schemas aninhados e aplique somente o schema pai à pasta.

## Excluir um formulário de schema de metadados {#delete-a-metadata-schema-form}

O Brand Portal permite que você exclua apenas formulários de schemas personalizados. Isso não permite que você exclua os formulários/modelos de schema padrão. No entanto, é possível excluir quaisquer alterações personalizadas nesses formulários.

Para excluir um formulário, selecione-o e clique no ícone **[!UICONTROL Excluir]**.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Após excluir as alterações personalizadas feitas em um formulário padrão, o símbolo **[!UICONTROL Lock]** reaparece antes do nome do formulário na interface do Schema de Metadados para indicar que o formulário é revertido para seu estado padrão.

## Formulários de schema para TIPOS MIME {#schema-forms-for-mime-types}

### Adicionar novos formulários para tipos MIME {#adding-new-forms-for-mime-types}

Além dos formulários padrão, você pode adicionar formulários personalizados para ativos de vários tipos MIME ou criar um novo formulário em um tipo de formulário apropriado. Por exemplo, para adicionar um novo modelo para o subtipo **[!UICONTROL image/png]**, crie o formulário nos formulários &quot;image&quot;. O título do formulário de esquema é o nome do subtipo. Nesse caso, o título é &quot;png&quot;.

#### Uso de um modelo de schema existente para vários tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Você pode usar um modelo existente para um tipo MIME diferente. Por exemplo, use o formulário **image/jpeg** para ativos do tipo MIME **image/png**.

Nesse caso, crie um novo nó em [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] no repositório CRX. Especifique um nome para o nó e defina as seguintes propriedades:

| **Nome** | **Tipo** | **Valor** |
|---|---|---|
| exposedmimetype | Sequência de caracteres | image/jpeg |
| mimetypes | Sequência de caracteres[] | image/png |

* **exposedmimetype**: Nome do formulário existente a ser mapeado
* **mimetypes**: Lista de tipos MIME que usam o formulário definido em  **** exposedmimetypeattribute

O Brand Portal mapeia os seguintes tipos MIME e formulários de schema:

| **Formulário de schema** | **Tipos MIME** |
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

A seguir está uma lista das propriedades de metadados padrão:

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
