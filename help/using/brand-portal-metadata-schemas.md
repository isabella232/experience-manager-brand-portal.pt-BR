---
title: Usar o formulário de esquema de metadados
seo-title: Usar o formulário de esquema de metadados
description: Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para os ativos que usam o esquema específico. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
seo-description: Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para os ativos que usam o esquema específico. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.
uuid: 1 a 944 a 3 b -5152-425 f-b 1 ea-bfe 3331 de 928
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: administration
discoiquuid: 500 b 46 da-ef 67-46 a 0-a 069-192 f 4 b 1 a 0 eca
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Usar o formulário de esquema de metadados {#use-the-metadata-schema-form}

Um esquema de metadados descreve o layout da página Propriedades e as propriedades de metadados exibidas para os ativos que usam o esquema específico. O esquema aplicado a um ativo determina os campos de metadados que aparecem na página Propriedades.

A página **Propriedades** de cada ativo inclui propriedades de metadados padrão dependendo do tipo MIME do ativo. Os administradores podem usar o Editor de esquema de metadados para modificar esquemas existentes ou adicionar esquemas de metadados personalizados. [!DNL AEM] Os ativos [!DNL Brand Portal] fornecem formulários padrão para ativos de vários tipos MIME. No entanto, você também pode adicionar formulários personalizados para esses ativos.

## Adicionar um formulário de esquema de metadados {#add-a-metadata-schema-form}

Para criar um novo formulário de esquema de metadados, faça o seguinte:

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Esquemas de metadados**.

   ![](assets/navigation-panel.png)

3. Na página Formulários de esquema **de metadados,** clique **em Criar**.

   ![](assets/create-metadata-schema-form.png)

4. Na caixa **de diálogo Criar formulário** de esquema, especifique o título do formulário Esquema e clique **em Criar** para concluir o processo de criação do formulário.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

É possível editar um formulário de esquema de metadados recém-adicionado ou existente. O formulário de esquema de metadados contém conteúdo derivado de seu pai, incluindo guias e itens de formulário nas guias. É possível mapear ou configurar esses itens de formulário para um campo dentro de um nó de metadados.

É possível adicionar novas guias ou itens de formulário ao formulário de esquema de metadados. As guias derivadas e os itens de formulário (do pai) estão no estado bloqueado. Não é possível alterá-los no nível filho.

Para editar um formulário de esquema de metadados, faça o seguinte:

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Esquemas de metadados**.
3. Na página **Formulários** de esquema de metadados, selecione um formulário de esquema para editar suas propriedades, por exemplo **, coleção**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Modelos não editados exibem um **símbolo de cadeado** antes deles. Se você personalizar qualquer um dos modelos, **o** símbolo Bloquear antes do modelo desaparecer.

4. Na barra de ferramentas na parte superior, clique **em Editar**.

   A página do Editor **de metadados de** metadados é aberta com a guia **Básica** aberta à esquerda e a guia **Build Form** (Criar formulário) aberta à direita.

5. Na página **Editor** de metadados de metadados, personalize a **página Propriedades** do ativo, arrastando um ou mais componentes de uma lista de tipos de componentes na guia **Criar formulário** para a **guia Básica** .

   ![](assets/metadata-schemaeditor-page.png)

6. Para configurar um componente, selecione-o e modifique suas propriedades na guia **Configurações** .

### Componentes na guia Criar formulário {#components-in-the-build-form-tab}

A guia **Criar formulário** lista itens que podem ser usados no formulário de esquema. A guia **Configurações** fornece os atributos de cada item selecionado na guia **Criar formulário** . A tabela a seguir lista os itens de formulário disponíveis na guia **Build Form** :

| Nome do componente | Descrição |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Título da seção | Adicione um título de seção para uma lista de componentes comuns. |
| Texto em linha única | Adicione uma propriedade de texto de linha única. É armazenado como uma string. |
| Multi valuetext | Adicione uma propriedade de texto com vários valores. É armazenado como uma matriz de string. |
| Número | Adicione um componente de número. |
| Data | Adicionar um componente de data. |
| Lista suspensa | Adicione uma lista suspensa. |
| Tags padrão | Adicionar uma tag. **Observação:** Os administradores podem precisar alterar o valor do caminho, por exemplo, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`se publicarem o formulário de esquema de metadados de [!DNL AEM]onde o caminho não inclui informações de locatário, por exemplo,`/etc/tags/<custom_tag_namespace>` |
| Tags inteligentes | Tags automaticamente detectadas se você adquiriu e configurou o complemento [!DNL AEM] de tags inteligentes. |
| Campo oculto | Adicione um campo oculto. É enviado como um parâmetro POST quando o ativo é salvo. |
| Ativo referenciado por | Adicione este componente para exibir a lista de ativos referenciados pelo ativo. |
| Fazer referência ao ativo | Adicione a exibição de uma lista de ativos que fazem referência ao ativo. |
| Classificação do ativo | Classificação média de um ativo adicionado a [!DNL AEM] partir de Ativos antes da publicação [!DNL Brand Portal]. |
| Metadados do contexto | Adicione para controlar a exibição de outras guias de metadados na página Propriedades dos ativos. |

>[!NOTE]
>
>Não use **Referências do produto** como não está funcionando.

#### Editar o componente de metadados {#edit-the-metadata-component}

Para editar as propriedades de um componente de metadados no formulário, clique no componente e edite suas propriedades na guia **Configurações** .

* **Rótulo do campo**: O nome da propriedade de metadados exibida na página Propriedades do ativo.

* **Mapear para propriedade**: O valor dessa propriedade fornece o caminho/nome relativo para o nó do ativo onde ele é salvo no repositório CRX. Inicia com "**./**"porque indica que o caminho está abaixo do nó do ativo.

Estes são os valores válidos para esta propriedade:

— `./jcr:content/metadata/dc:title`: Armazena o valor no nó de metadados do ativo como a propriedade `dc:title`.

— `./jcr:created`: Exibe a propriedade jcr no nó do ativo. Se você configurar essas propriedades em propriedades de exibição, recomendamos marcá-las como Desativar edição, pois elas são protegidas. Caso contrário, o erro "Ativo (s) não modificado" ocorre ao salvar as propriedades do ativo.

* **Espaço reservado**: Use essa propriedade para fornecer ao usuário quaisquer informações relevantes relacionadas à propriedade de metadados.
* **Obrigatório**: Use essa propriedade para marcar uma propriedade de metadados como obrigatório na página Propriedades.
* **Desativar Editar**: Use essa propriedade para tornar uma propriedade de metadados não editável na página Propriedades.
* **Mostrar campo vazio em somente leitura**: Marque essa propriedade para exibir uma propriedade de metadados na página Propriedades mesmo que não tenha valor. Por padrão, quando uma propriedade de metadados não tem valor, ela não é listada na página Propriedades.
* **Descrição**: Use essa propriedade para adicionar uma breve descrição para o componente de metadados.
* **Excluir ícone: Clique nesse ícone para excluir um componente do formulário de esquema.**

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos os campos de metadados são somente leitura no modo de editor de metadados de um ativo. Como os metadados do ativo devem ser editados em [!DNL AEM] Ativos antes da publicação de um ativo.[!DNL Brand Portal]

#### Adicionar ou excluir uma guia no formulário de esquema {#add-or-delete-a-tab-in-the-schema-form}

O formulário de esquema padrão inclui as guias **Básico** e **Avançado** . O editor de esquema permite adicionar ou excluir uma guia.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para adicionar uma nova guia em um formulário de esquema, clique **em +**. Por padrão, a nova guia possui o nome "Não nomeado -1". Você pode modificar o nome na guia **Configurações** .

![](assets/add-tab-metadata-form.png)

* Para excluir uma guia, clique **em x**. Click **Save** to save the changes.

## Aplicar um esquema de metadados a uma pasta {#apply-a-metadata-schema-to-a-folder}

[!DNL Brand Portal] permite personalizar e controlar o esquema de metadados para que a página **Propriedades** de um ativo exiba apenas as informações específicas que você escolher revelar. Para controlar os metadados exibidos na página **Propriedades** , remova os metadados necessários do formulário de esquema de metadados e aplique-os à pasta específica.

Para aplicar um formulário de esquema de metadados a uma pasta, faça o seguinte:

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Esquemas de metadados**.

3. Na página **Formulários** de esquema de metadados, selecione o formulário de esquema a ser aplicado a um ativo, por exemplo **, roupas**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. Na barra de ferramentas na parte superior, clique **em Aplicar às pastas**.

5. Na página **Selecionar pasta (s)** , navegue até a pasta à qual você deseja aplicar o esquema de metadados **de roupas** , por exemplo **, Gloves**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. Clique **em Aplicar** para aplicar o formulário de esquema de metadados à pasta.

   Os metadados disponíveis no formulário de esquema de metadados **do vestuário** são aplicados à pasta **Gloves** e são visíveis na página **Propriedades** da pasta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se você aplicar um esquema que inclua esquemas aninhados para uma pasta que contenha arquivos de vídeo, as propriedades de metadados dos arquivos de vídeo poderão não renderizar corretamente. Para garantir que as propriedades de metadados sejam renderizadas corretamente, remova os esquemas aninhados e aplique somente o esquema pai à pasta.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

[!DNL Brand Portal] permite excluir apenas formulários de esquema personalizados. Isso não permite que você exclua os formulários/modelos de esquema padrão. No entanto, é possível excluir quaisquer alterações personalizadas nesses formulários.

Para excluir um formulário, selecione um formulário e clique no **ícone Excluir** .

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Depois de excluir as alterações personalizadas feitas em um formulário padrão, o **símbolo de cadeado** aparece novamente antes do nome do formulário na interface do Esquema de metadados para indicar que o formulário é revertido para o estado padrão.

## Formulários de esquema para tipos MIME {#schema-forms-for-mime-types}

### Adição de novos formulários para tipos MIME {#adding-new-forms-for-mime-types}

Além dos formulários padrão, você pode adicionar formulários personalizados para ativos de vários tipos MIME ou criar um novo formulário em um tipo de formulário apropriado. Por exemplo, para adicionar um novo modelo para o subtipo **image/png** , crie o formulário sob os formulários "image". O título do formulário de esquema é o nome do subtipo. Nesse caso, o título é "png".

#### Uso de um modelo de esquema existente para vários tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Você pode usar um modelo existente para um tipo MIME diferente. Por exemplo, use o formulário **image/jpeg** para ativos de **imagem/png** MIME.

Nesse caso, crie um novo nó no `/etc/dam/metadataeditor/mimetypemappings` repositório CRX. Especifique um nome para o nó e defina as seguintes propriedades:

| **Nome** | **Tipo** | **Valor** |
|---|---|---|
| exposedmimetype | Sequência de caracteres | image/jpeg |
| mimetypes | Sequência de caracteres[] | image/png |

* **exposedmimetype**: Nome do formulário existente a ser mapeado
* **mimetypes**: Lista de tipos MIME que usam o formulário definido no atributo **exposedmimetype**

[!DNL Brand Portal] mapeia os seguintes tipos MIME e esquemas de esquema:

| **Formulário de esquema** | **Tipos MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-imageset | Multipart/Related; type=application/x-ImageSet |
| application/x-spinset | Multipart/Related; type=application/x-SpinSet |
| application/x-mixedmediaset | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg 4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

A seguir está uma lista de propriedades de metadados padrão:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr: content/metadata/videocodec
* jcr: content/metadata/audiocodec
* jcr: content/metadata/dc: title
* jcr: content/metadata/dc: descrição
* jcr: content/metadata/xmpmm: Instanceid
* jcr: content/metadata/xmpmm: Documentid
* jcr: conteúdo/metadata/dam: sha 1
* jcr: conteúdo/metadata/dam: Solutioncontext
* jcr: content/metadata/videobitrate
* jcr: content/metadata/audiobitrate
* jcr: content/usages/usedby
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr: content/ontime
* jcr: content/offtime
* jcr:content/metadata/dam:size
* jcr: content/metadata/tiff: Imagewidth
* jcr: content/metadata/tiff: Imagelength