---
title: Usar o formulário de esquema de metadados
seo-title: Use the metadata schema form
description: Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o esquema específico. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 12%

---

# Usar o formulário de esquema de metadados {#use-the-metadata-schema-form}

Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para ativos que usam o esquema específico. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.

A variável **[!UICONTROL Propriedades]** A página de cada ativo inclui propriedades de metadados padrão, dependendo do tipo MIME do ativo. Os administradores podem usar o Editor de esquema de metadados para modificar esquemas existentes ou adicionar esquemas de metadados personalizados. O Experience Manager Assets Brand Portal fornece formulários padrão para ativos de vários tipos MIME. No entanto, também é possível adicionar formulários personalizados para esses ativos.

## Adicionar um formulário de esquema de metadados {#add-a-metadata-schema-form}

Para criar um novo formulário de esquema de metadados, faça o seguinte:

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Esquemas de metadados]**.

   ![](assets/navigation-panel.png)

1. No **[!UICONTROL Forms do esquema de metadados]** clique em **[!UICONTROL Criar]**.

   ![](assets/create-metadata-schema-form.png)

1. No **[!UICONTROL Criar formulário de esquema]** especifique o título do formulário Esquema e clique em **[!UICONTROL Criar]** para concluir o processo de criação do formulário.

   ![](assets/create-schema-form.png)

## Editar um formulário de esquema de metadados {#edit-a-metadata-schema-form}

Você pode editar um formulário de esquema de metadados recém-adicionado ou existente. O formulário de esquema de metadados contém conteúdo derivado de seu pai, incluindo guias e itens de formulário dentro de guias. Você pode mapear ou configurar esses itens de formulário para um campo em um nó de metadados.

Você pode adicionar novas guias ou itens de formulário ao formulário de esquema de metadados. As guias e os itens de formulário derivados (do pai) estão no estado bloqueado. Não é possível alterá-los no nível secundário.

Para editar um formulário de esquema de metadados, faça o seguinte:

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Esquemas de metadados]**.
1. No **[!UICONTROL Forms do esquema de metadados]** selecione um formulário de esquema para editar suas propriedades, por exemplo, **[!UICONTROL coleção]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Modelos não editados exibem um símbolo de bloqueio antes deles. Se você personalizar qualquer um dos modelos, o símbolo Bloquear antes que o modelo desapareça.

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Editar]**.

   A variável **[!UICONTROL Editor de esquema de metadados]** A página é aberta com o **[!UICONTROL Básico]** na guia à esquerda e na guia **[!UICONTROL Formulário de criação]** abram a guia à direita.

1. No **[!UICONTROL Editor de esquema de metadados]** personalize o **[!UICONTROL Propriedades]** página do ativo arrastando um ou mais componentes de uma lista de tipos de componentes na **[!UICONTROL Formulário de criação]** para a guia **[!UICONTROL Básico]** guia.

   ![](assets/metadata-schemaeditor-page.png)

1. Para configurar um componente, selecione-o e modifique suas propriedades na **[!UICONTROL Configurações]** guia.

### Componentes na guia Criar formulário {#components-in-the-build-form-tab}

A variável **[!UICONTROL Formulário de criação]** A guia lista itens que você pode usar no formulário do esquema. A variável **[!UICONTROL Configurações]** fornece os atributos de cada item selecionado na guia **[!UICONTROL Formulário de criação]** guia. A tabela a seguir lista os itens de formulário disponíveis no **[!UICONTROL Formulário de criação]** guia:

| Nome do componente | Descrição |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL Cabeçalho da seção]** | Adicione um cabeçalho de seção para obter uma lista de componentes comuns. |
| **[!UICONTROL Texto em linha única]** | Adicione uma propriedade de texto de linha única. Ele é armazenado como uma string. |
| **[!UICONTROL Texto de vários valores]** | Adicione uma propriedade de texto de vários valores. Ele é armazenado como uma matriz de sequência. |
| **[!UICONTROL Número]** | Adicione um componente de número. |
| **[!UICONTROL Data]** | Adicione um componente de data. |
| **[!UICONTROL Lista suspensa]** | Adicione uma lista suspensa. |
| **[!UICONTROL Tags padrão]** | Adicionar uma tag. **Nota:** Os administradores podem precisar alterar o valor do caminho, por exemplo, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`, se eles publicarem o formulário de esquema de metadados do Experience Manager Assets, em que o caminho não inclui informações do locatário, por exemplo, `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL Tags inteligentes]** | Tags detectadas automaticamente se você tiver comprado e configurado o complemento tags inteligentes da Experience Manager Assets. |
| **[!UICONTROL Campo oculto]** | Adicione um campo oculto. Ele é enviado como um parâmetro POST quando o ativo é salvo. |
| **[!UICONTROL Ativo referenciado por]** | Adicione este componente para visualizar a lista de ativos referenciados pelo ativo. |
| **[!UICONTROL Fazer referência ao ativo]** | Adicionar para exibir uma lista de ativos que fazem referência ao ativo. |
| **[!UICONTROL Classificação do ativo]** | Classificação média de um ativo adicionado do Experience Manager Assets antes de ele ser publicado no Brand Portal. |
| **[!UICONTROL Metadados do contexto]** | Adicione para controlar a exibição de outras guias de metadados na página Propriedades dos ativos. |

>[!NOTE]
>
>Não usar **[!UICONTROL Referências do produto]**, pois não é funcional.

#### Editar o componente de metadados {#edit-the-metadata-component}

Para editar as propriedades de um componente de metadados no formulário, clique no componente e edite suas propriedades na **[!UICONTROL Configurações]** guia.

* **[!UICONTROL Rótulo do campo]**: o nome da propriedade de metadados que é exibida na página Propriedades do ativo.

* **[!UICONTROL Mapear para a propriedade]**: o valor dessa propriedade fornece o caminho/nome relativo para o nó do ativo onde ele é salvo no repositório CRX. Ele começa com &quot;**./**&quot; porque indica que o caminho está no nó do ativo.

A seguir estão os valores válidos para essa propriedade:

-- `./jcr:content/metadata/dc:title`: armazena o valor no nó de metadados do ativo como a propriedade [!UICONTROL `dc:title`].

-- `./jcr:created`: exibe a propriedade jcr no nó do ativo. Se você configurar essas propriedades nas propriedades de exibição, recomendamos marcá-las como Desativar edição, pois elas estão protegidas. Caso contrário, o erro &quot;Os ativos falharam ao serem modificados&quot; ocorre ao salvar as propriedades do ativo.

* **[!UICONTROL Espaço reservado]**: use essa propriedade para fornecer ao usuário todas as informações relevantes sobre a propriedade de metadados.
* **[!UICONTROL Obrigatório]**: use essa propriedade para marcar uma propriedade de metadados como obrigatória na página Propriedades.
* **[!UICONTROL Desativar edição]**: use essa propriedade para tornar uma propriedade de metadados não editável na página Propriedades.
* **[!UICONTROL Mostrar Campo Vazio Em Somente Leitura]**: marque essa propriedade para exibir uma propriedade de metadados na página Propriedades, mesmo que ela não tenha valor. Por padrão, quando uma propriedade de metadados não tem valor, ela não é listada na página Propriedades.
* **[!UICONTROL Descrição]**: use essa propriedade para adicionar uma breve descrição do componente de metadados.
* **[!UICONTROL Ícone Excluir]**: Clique neste ícone para excluir um componente do formulário de esquema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos os campos de metadados são somente leitura no formulário do editor de metadados de um ativo. Como os metadados do ativo devem ser editados no Experience Manager Assets antes que um ativo seja publicado no Brand Portal.

#### Adicionar ou excluir uma guia no formulário de esquema {#add-or-delete-a-tab-in-the-schema-form}

O formulário de esquema padrão inclui a variável **[!UICONTROL Básico]** e **[!UICONTROL Avançado]** guias. O editor de esquema permite adicionar ou excluir uma guia.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para adicionar uma nova guia em um formulário de esquema, clique em **[!UICONTROL +]**. Por padrão, a nova guia tem o nome &quot;Sem nome-1&quot;. Você pode modificar o nome da variável **[!UICONTROL Configurações]** guia.

![](assets/add-tab-metadata-form.png)

* Para excluir uma guia, clique em **[!UICONTROL x]**. Clique em **[!UICONTROL Salvar]** para salvar as alterações.

## Aplicar um esquema de metadados a uma pasta {#apply-a-metadata-schema-to-a-folder}

O Brand Portal permite personalizar e controlar o esquema de metadados para que o **[!UICONTROL Propriedades]** de um ativo exibe somente as informações específicas que você escolhe revelar. Para controlar os metadados exibidos no **[!UICONTROL Propriedades]** remova os metadados necessários do formulário de esquema de metadados e aplique-os à pasta específica.

Para aplicar um formulário de esquema de metadados a uma pasta, faça o seguinte:

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Esquemas de metadados]**.

1. No **[!UICONTROL Forms do esquema de metadados]** selecione o formulário de esquema que deseja aplicar a um ativo, por exemplo, **[!UICONTROL vestuário]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Aplicar às pastas]**.

1. No **[!UICONTROL Selecionar pasta(s)]** navegue até a pasta à qual deseja aplicar a variável **[!UICONTROL vestuário]** esquema de metadados, por exemplo, **[!UICONTROL Luvas]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. Clique em **[!UICONTROL Aplicar]** para aplicar o formulário de esquema de metadados à pasta.

   Os metadados disponíveis no **[!UICONTROL vestuário]** o formulário de esquema de metadados é aplicado ao **[!UICONTROL Luvas]** e visível na **[!UICONTROL Propriedades]** página da pasta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se você aplicar um esquema que inclui esquemas aninhados a uma pasta contendo arquivos de vídeo, as propriedades de metadados dos arquivos de vídeo podem não ser renderizadas corretamente. Para garantir que as propriedades de metadados sejam renderizadas corretamente, remova os esquemas aninhados e aplique somente o esquema principal à pasta.

## Excluir um formulário de esquema de metadados {#delete-a-metadata-schema-form}

O Brand Portal permite excluir somente formulários de esquema personalizados. Isso não permite excluir os formulários/modelos de esquema padrão. No entanto, você pode excluir qualquer alteração personalizada nesses formulários.

Para excluir um formulário, selecione um formulário e clique no **[!UICONTROL Excluir]** ícone.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Após excluir as alterações personalizadas feitas em um formulário padrão, a variável **[!UICONTROL Bloquear]** O símbolo reaparece antes do nome do formulário na interface do Esquema de metadados para indicar que o formulário é revertido para seu estado padrão.

## Formulários de esquema para TIPOS MIME {#schema-forms-for-mime-types}

### Adição de novos formulários para tipos MIME {#adding-new-forms-for-mime-types}

Além dos formulários padrão, é possível adicionar formulários personalizados para ativos de vários tipos MIME ou criar um novo formulário em um tipo de formulário apropriado. Por exemplo, para adicionar um novo modelo para o subtipo **[!UICONTROL image/png]**, crie o formulário nos formulários &quot;image&quot;. O título do formulário de esquema é o nome do subtipo. Nesse caso, o título é &quot;png&quot;.

#### Uso de um modelo de esquema existente para vários tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Você pode usar um modelo existente para um tipo MIME diferente. Por exemplo, use o **image/jpeg** formulário para ativos do tipo MIME **image/png**.

Nesse caso, crie um novo nó em [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] no repositório CRX. Especifique um nome para o nó e defina as seguintes propriedades:

| **Nome** | **Tipo** | **Valor** |
|---|---|---|
| exposedmimetype | String | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmimetype**: Nome do formulário existente a ser mapeado
* **mimetypes**: lista de tipos MIME que usam o formulário definido no **exposedmimetype** atributo

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
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

Esta é uma lista de propriedades de metadados padrão:

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
