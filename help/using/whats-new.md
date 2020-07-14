---
title: Novidades do AEM Assets Brand Portal
seo-title: Novidades do AEM Assets Brand Portal
description: Dê uma olhada nos novos recursos e melhorias da versão 6.4.6.
seo-description: Dê uma olhada nos novos recursos e melhorias da versão 6.4.6.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '4462'
ht-degree: 2%

---


# Novidades do AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

O Portal de marcas de ativos Adobe Experience Manager (AEM) ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros externos e usuários empresariais internos em dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado. A Adobe está trabalhando para melhorar a experiência geral do Brand Portal. Veja os novos recursos e melhorias.

## O que mudou no ponto 6.4.6 {#what-changed-in-646}

No Brand Portal 6.4.6, o canal de autorização entre o AEM Assets e o Brand Portal é alterado. O Brand Portal agora é compatível com o serviço em nuvem AEM Assets, AEM Assets 6.3 e posteriores. No AEM Assets 6.3 e superior, o Brand Portal foi configurado anteriormente na interface clássica por meio do gateway OAuth herdado, que usa a troca de token JWT para obter um Token de acesso IMS para autorização. O AEM Assets agora está configurado com o Brand Portal por meio do Adobe Developer Console, que obtém um token IMS para autorização do locatário do Brand Portal.

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

As etapas para configurar AEM Assets com o Brand Portal são diferentes dependendo da versão do AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **Versão do AEM** | **Nova configuração** | **Configuração de atualização** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |

>[!NOTE]
>
>É recomendável atualizar sua instância do AEM para o service pack mais recente.

Consulte as notas [de versão mais recentes do Portal de](brand-portal-release-notes.md)marcas.

Consulte Perguntas frequentes sobre [o Brand Portal](brand-portal-faqs.md).

## O que mudou no ponto 6.4.5 {#what-changed-in-645}


O Brand Portal 6.4.5 é uma versão do recurso que tem como objetivo fornecer aos usuários do Brand Portal (agências/equipes externas) a capacidade de carregar conteúdo no Brand Portal e publicá-lo nos AEM Assets, sem precisar acessar o ambiente de criação. Esse recurso é chamado de Fonte de **[ativos no Portal](brand-portal-asset-sourcing.md)**de marcas e melhorará as experiências do cliente, fornecendo um mecanismo bidirecional para que os usuários contribuam e compartilhem ativos com outros usuários do Portal de marcas distribuído globalmente.

### Seleção de recursos no Brand Portal {#asset-sourcing-in-bp}

A Fonte de ativos permite que usuários do AEM (administradores/usuários não administradores) criem novas pastas com uma propriedade adicional de Contribuição **** de ativos, garantindo que a nova pasta criada seja aberta para envio de ativos por usuários do Brand Portal. Isso aciona automaticamente um fluxo de trabalho que cria duas subpastas adicionais, chamadas NOVO e COMPARTILHADO, na pasta recém-criada **Contribuição** .

O usuário do AEM define o requisito [fazendo upload de um resumo](brand-portal-configure-contribution-folder-properties.md) sobre os tipos de ativos que devem ser adicionados à pasta de contribuição, bem como [fazendo upload dos ativos](brand-portal-upload-baseline-assets.md)da linha de base, para a pasta **SHARED** , a fim de garantir que os usuários do BP tenham as informações de referência necessárias. O administrador pode conceder aos usuários ativos do Brand Portal acesso à pasta de contribuição antes de publicar a pasta recém-criada **Contribuição** no Brand Portal.


Quando o usuário terminar de adicionar conteúdo na pasta **NEW** , poderá publicar a pasta de contribuição de volta no ambiente do autor do AEM. Observe que pode levar alguns minutos para concluir a importação e refletir o conteúdo recém-publicado no AEM Assets.

Além disso, toda a funcionalidade existente permanece inalterada. Os usuários do Brand Portal podem visualização, pesquisar e baixar ativos da pasta de contribuição, bem como de outras pastas permitidas. E os administradores podem compartilhar ainda mais a pasta de contribuição, modificar as propriedades e adicionar ativos às coleções.

>[!NOTE]
>
>A Seleção de recursos no Brand Portal é compatível com o AEM 6.5.2.0 e superior.
>
>O recurso não é suportado nas versões anteriores - AEM 6.3 e AEM 6.4.

### Fazer upload de ativos para a pasta de contribuição {#upload-assets-in-bp}

Os usuários do Brand Portal com as permissões apropriadas podem [baixar os requisitos](brand-portal-download-asset-requirements.md) de ativos para entender a necessidade de contribuição e fazer upload de vários ativos ou pastas que contêm vários ativos para a pasta de contribuição. Entretanto, observe que os usuários do Brand Portal só podem carregar ativos na subpasta **NEW** . A pasta **SHARED** destina-se à distribuição de requisitos e ativos de linha de base. Consulte, [Fazer upload de ativos para a pasta de contribuição](brand-portal-upload-assets-to-contribution-folder.md)

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### Publicar pasta de contribuição em AEM Assets {#publish-assets-to-aem}

Quando o upload for concluído para a pasta **NOVA** , os usuários do Brand Portal poderão publicar a pasta de contribuição de volta no AEM. Pode levar alguns minutos para importar e refletir o conteúdo/ativos publicados no AEM Assets. Consulte, [Publicar pasta de contribuição para AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## O que mudou no ponto 6.4.4 {#what-changed-in-644}

A versão 6.4.4 do Brand Portal foca em melhorias na pesquisa de texto e nas principais solicitações do cliente. Consulte as notas [de versão mais recentes do Portal de](brand-portal-release-notes.md)marcas.

### Aprimoramentos de pesquisa {#search-enhancements}

O Brand Portal 6.4.4 em diante oferece suporte à pesquisa de texto parcial no predicado de propriedade no painel de filtragem. Para permitir a pesquisa de texto parcial, é necessário ativar a Pesquisa **** parcial no Predicado de propriedade no formulário de pesquisa.

Leia para saber mais sobre pesquisa de texto parcial e pesquisa de curinga.

#### Pesquisa de frase parcial {#partial-phrase-search}

Agora você pode pesquisar ativos especificando apenas uma parte (ou seja, uma palavra ou duas) da frase pesquisada no painel de filtragem.

**Caso de usoA pesquisa de frases** parciais é útil quando você não tem certeza da combinação exata de palavras que ocorrem na frase pesquisada.

Por exemplo, se o formulário de pesquisa no Brand Portal usar o Predicado de propriedade para uma pesquisa parcial sobre o título dos ativos, a especificação do termo **campo** retornará todos os ativos com o campo de palavras em suas frases de título.

![](assets/partialphrasesearch.png)

#### Pesquisa curinga {#wildcard-search}

O Brand Portal permite o uso do asterisco (*) no query de pesquisa junto com uma parte da palavra na frase pesquisada.

**Caso** de uso Se você não tiver certeza das palavras exatas que ocorrem na frase pesquisada, poderá usar uma pesquisa curinga para preencher as lacunas no query de pesquisa.

Por exemplo, especificar **climb*** retorna todos os ativos com palavras que começam com os caracteres que **sobem** em suas frases de título se o formulário de pesquisa no Portal de marcas usar Predicado de propriedade para pesquisa parcial no título dos ativos.

![](assets/wildcard-prop.png)

Da mesma forma, especificando:

* ***climb** retorna todos os ativos que têm palavras que terminam com caracteres que **sobem** em suas frases de título.

* ***climb*** retorna todos os ativos com palavras que incluem os caracteres que **sobem** em suas frases de título.

>[!NOTE]
>
>Ao marcar a caixa de seleção Pesquisa **** parcial, a opção **Ignorar caso** é selecionada por padrão.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## O que mudou no ponto 6.4.3 {#what-changed-in}

A versão 6.4.3 do Brand Portal foca em — fornecer às organizações um alias alternativo além da ID do locatário no URL de acesso do Brand Portal, nova configuração de hierarquia de pastas, aprimoramentos de suporte de vídeo, publicação agendada da instância do AEM Author para o Brand Portal, melhorias operacionais — e atende às solicitações do cliente.

### Navegação de hierarquia de pastas para não administradores

Agora, os administradores podem configurar como as pastas são exibidas para usuários não administradores (editores, visualizadores e usuários convidados) no logon. [A configuração Ativar hierarquia](../using/brand-portal-general-configuration.md) de pastas é adicionada em Configurações **** gerais, no painel Ferramentas administrativas. Se a configuração for:

* **ativada**, a árvore de pastas que começa na pasta raiz está visível para usuários não administradores. Assim, concedendo a eles uma experiência de navegação semelhante aos administradores.
* **desativado**, somente as pastas compartilhadas são exibidas na landing page.

![](assets/enable-folder-hierarchy.png)
**O caso de uso**

A funcionalidade [Ativar hierarquia](../using/brand-portal-general-configuration.md) de pastas (quando ativada) ajuda a diferenciar as pastas com os mesmos nomes compartilhados de diferentes hierarquias. Ao fazer logon, usuários não administradores agora veem as pastas pai virtual (e ancestral) das pastas compartilhadas.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

As pastas compartilhadas são organizadas nos respectivos diretórios em pastas virtuais. É possível reconhecer essas pastas virtuais com um ícone de cadeado.

Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Pesquisar em hierarquia ou caminho de pasta específicos

**O predicado Navegador** de caminho é introduzido no Formulário de pesquisa para permitir a pesquisa de ativos em um diretório específico. O caminho de pesquisa padrão do predicado de pesquisa para o Navegador de caminhos é `/content/dam/mac/<tenant-id>/`, que pode ser configurado pela edição do formulário de pesquisa padrão.

* Os usuários administradores podem usar o Navegador de caminhos para navegar até qualquer diretório de pastas no Brand Portal.
* Usuários não administradores podem usar o Navegador de caminhos para navegar somente para as pastas (e navegar de volta para as pastas pai) compartilhadas com eles.
Por exemplo, `/content/dam/mac/<tenant-id>/folderA/folderB/folderC` é compartilhado com um usuário não administrador. The user can search for assets within folderC using Path Browser. Esse usuário também pode navegar para folderB e folderA (já que eles são ancestrais da folderC que é compartilhada com o usuário).

![](assets/edit-search-form.png)

**O caso de uso**

Agora você pode restringir a pesquisa de ativos em uma pasta específica que você navegou, em vez de começar na pasta raiz.

Note that searching under these folders returns results only from the assets that have been shared with the user.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media video renditions support

Users whose AEM Author instance is on Dynamic Media hybrid mode can preview and download the dynamic media renditions, in addition to the original video files.

To allow preview and download of dynamic media renditions on specific tenant accounts, administrators need to specify **Dynamic Media Configuration** (video service URL (DM-Gateway URL) and registration ID to fetch the dynamic video) in **Video** configuration from admin tools panel.

**Os vídeos de caso** de uso do Dynamic Media podem ser visualizados em:

* Página de detalhes do ativo
* Asset&#39;s card view
* Página pré-visualização de compartilhamento de links

As codificações de vídeo Dynamic Media podem ser baixadas de:

* Brand Portal
* Link compartilhado

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publicação agendada para o Brand Portal

O fluxo de trabalho de publicação de ativos (e pastas) da instância do autor do [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) para o Brand Portal pode ser agendado para uma data e hora posteriores.

Da mesma forma, os recursos publicados podem ser removidos do portal em uma data posterior (hora), agendando o fluxo de trabalho Cancelar publicação do Brand Portal.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias de locatário configurável no URL

As organizações podem personalizar o URL do portal, tendo um prefixo alternativo no URL. To get an alias for tenant name in their existing portal URL, organizations need to contact Adobe support.

Observe que somente o prefixo do URL do Portal de Marcas pode ser personalizado e não o URL inteiro.\
Por exemplo, uma organização com o domínio existente **geomettrix.brand-portal.adobe.com** pode obter **geomettrixinc.brand-portal.adobe.com** criado mediante solicitação.

No entanto, a instância AEM Author só pode ser [configurada](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) com o URL de ID de locatário e não com o URL de alias de locatário (alternativo).

**O caso** de uso As organizações podem atender às suas necessidades de marca ao personalizar o URL do portal, em vez de aderir ao URL fornecido pela Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Melhorias na experiência de download

A versão do oferta simplificou a experiência de download com um número reduzido de cliques e avisos, em:

* optar por baixar somente as representações (e não os ativos originais).
* baixar os ativos quando o acesso às representações originais estiver restrito.

## O que mudou no ponto 6.4.2 {#what-changed-in-1}

A versão do Brand Portal 6.4.2 traz uma variedade de recursos para atender às necessidades de distribuição de ativos das organizações e ajudá-las a atingir um grande número de usuários distribuídos globalmente por meio do acesso de convidado e da experiência ideal com downloads acelerados. O Brand Portal também oferece maior controle às organizações por meio de novas configurações para administradores, relatórios recém-adicionados e atende às solicitações dos clientes.

### Acesso de convidado

![](assets/bp-login-screen-1.png)

O portal da marca AEM permite que os convidados acessem o portal. A guest user doesn&#39;t require credentials to enter the portal and can access and download all the public folders and collections. Guest users can add assets to their lightbox (private collection) and download the same. Eles também podem visualização previsões de pesquisa e pesquisa de tags inteligentes definidas pelos administradores. A sessão de convidado não permite que os usuários criem coleções e pesquisas salvas ou as compartilhem mais, acessem configurações de pastas e coleções e compartilhem ativos como links.

Em uma organização, várias sessões de convidado simultâneas são permitidas, o que é limitado a 10% da cota total de usuários por organização.

Uma sessão de convidado permanece ativa por duas horas. Portanto, o estado do lightbox também é preservado até duas horas a partir da hora do start da sessão. Depois de duas horas, a sessão de convidado tem que ser reiniciada, de modo que o estado do lightbox seja perdido.

### Downloads acelerados

Brand Portal users can leverage IBM Aspera Connect based fast downloads to get speeds up to 25x faster and enjoy a seamless download experience irrespective of their location across the globe. Para baixar os recursos mais rapidamente do Brand Portal ou do link compartilhado, os usuários precisam selecionar a opção **Ativar aceleração** do download na caixa de diálogo de download, desde que a aceleração do download esteja ativada em sua organização.

![](assets/donload-assets-dialog-2.png)

Para habilitar o download acelerado com base no IBM Aspera para a organização, os administradores **habilitam a opção de aceleração** de download (que está desabilitada por padrão) em Configurações [](brand-portal-general-configuration.md#allow-download-acceleration) gerais no painel de ferramentas administrativas. Para saber mais sobre pré-requisitos e etapas de solução de problemas para baixar arquivos de ativos mais rapidamente do Brand Portal e links compartilhados, consulte o [Guia para acelerar os downloads do Brand Portal](../using/accelerated-download.md#main-pars-header).

### Relatório de logons de usuário

A new report, to track user logins, has been introduced. O relatório Logons **de** usuário pode ser fundamental para permitir que as organizações auditem e verifiquem os administradores delegados e outros usuários do Brand Portal.

Os registros do relatório exibem nomes, IDs de e-mail, personas (administrador, visualizador, editor, convidado), grupos, último logon, status de atividade e contagem de logon de cada usuário da implantação do Brand Portal 6.4.2 até o momento da geração do relatório. Os administradores podem exportar o relatório como .csv. Juntamente com outros relatórios, o relatório Logons de usuário permite que as organizações monitorem mais detalhadamente as interações dos usuários com os recursos aprovados da marca, garantindo assim a conformidade com os escritórios de conformidade corporativos.

![](assets/user-logins-1.png)

### Acesso a representações originais

Os administradores podem restringir o acesso do usuário aos arquivos de imagem originais (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, imagem/photoshop, imagem/x-photoshop, psd, image/vnd.adobe.photoshop) e dá acesso a renderizações de baixa resolução que eles baixam do Brand Portal ou do link compartilhado. Esse acesso pode ser controlado no nível do grupo de usuários na guia Grupos da página Funções do usuário no painel Ferramentas administrativas.

![](assets/access-original-rend-1.png)

* Por padrão, todos os usuários podem baixar representações originais, já que o Acesso ao original está ativado para todos.
* Os administradores precisam desmarcar as respectivas caixas de seleção para impedir que um grupo de usuários acesse execuções originais.
* Se um usuário for membro de vários grupos, mas apenas um deles tiver restrições, as restrições se aplicam a esse usuário.
* As restrições não se aplicam aos administradores, mesmo sendo membros de grupos restritos.
* As permissões dos usuários que compartilham ativos como link se aplicam aos usuários que baixam ativos usando links compartilhados.

### Folder hierarchy path on Card and List views

Os cartões de pastas, na Visualização de cartão, agora exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas que estão acessando, em relação à hierarquia pai.

Folder hierarchy information is particularly helpful in differentiating the folders having names similar to other folders shared from a different folder hierarchy. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, ativos/pastas com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para se ajustarem aos tamanhos dos cartões. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o mouse sobre o caminho truncado.

![](assets/folder-hierarchy1-1.png)

A Visualização de Lista mostra a pasta Caminho dos ativos em uma coluna para todos os usuários do Brand Portal.

![](assets/list-view-1.png)

### Opção Visão geral para visualização propriedades de ativos

O Brand Portal fornece a opção Visão geral para usuários não administradores (editores, visualizadores, usuários convidados) para visualização das Propriedades do ativo de ativos/pastas selecionados. A opção Visão geral está visível:

1. Na barra de ferramentas na parte superior da seleção de um ativo/pasta.
2. Na lista suspensa ao selecionar o Seletor de painel.

Ao selecionar a opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação do ativo. Enquanto isso, na página de detalhes do ativo, selecionar a opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## New configurations

Seis novas configurações são adicionadas aos administradores para ativar/desativar as seguintes funcionalidades em locatários específicos:

* Permitir acesso de convidado
* Permitir que os usuários solicitem acesso ao Brand Portal
* Permitir que os administradores excluam ativos do Brand Portal
* Permitir criação de coleções públicas
* Permitir a criação de coleções inteligentes públicas
* Permitir aceleração de download

As configurações acima estão disponíveis em Configurações gerais e de acesso no painel Ferramentas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Interface do usuário de E/S da Adobe para configurar integrações do oAuth

A partir do Brand Portal 6.4.2, usa a interface Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para criar o aplicativo JWT, que permite a configuração de integrações de Auth para permitir a integração de AEM Assets com o Brand Portal. Anteriormente, a interface do usuário para configurar integrações OAuth era hospedada em `https://marketing.adobe.com/developer/`. To know more about integrating AEM Assets with Brand Portal for publishing assets and collections to Brand Portal refer [Configure AEM Assets integration with Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html).

## Search Enhancements

Administrators can make the property predicates non-case sensitive by using the updated property predicate, which has a check for Ignore Case. This option is available for property predicate and multi-value property predicate.\
However, the non-case sensitive search is comparatively slower than default search for property predicate. Se houver muitos predicados que não diferenciam maiúsculas de minúsculas no filtro de pesquisa, a pesquisa poderá diminuir. It is, therefore, advised to use the non-case sensitive search judiciously.

## What changed in 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 is a platform upgrade release which brings in several new features and vital enhancements such as browsing, searching, and performance enhancements to deliver fulfilling customer experiences.

### Browse Enhancements

* New Content Tree rail to quickly navigate an asset hierarchy.

![](assets/contenttree-2.png)

* Introduced new keyboard shortcuts, for example _(p)_ for navigation to properties page, _(e)_ for Edit, and _(ctrl+c)_ for copy operations.
* Improved scrolling, lazy loading experience in card and list view for browsing large number of assets.
* Visualização de placa aprimorada com suporte para placas de tamanho diferente com base na configuração de visualização.

![](assets/cardviewsettings-1.png)

* A visualização de cartão agora exibe o carimbo de data/hora ao passar o mouse sobre a etiqueta de data.

* visualização aprimorada de coluna com **mais detalhes** no instantâneo do ativo, que permite navegar até a página de detalhes de um ativo.

![](assets/columnmoredetail.png)

* A visualização de Lista agora exibe nomes de arquivos de ativos na primeira coluna por padrão, além de informações sobre localidade, tipo de ativo, dimensões, tamanho, classificação e publicação. Novas configurações **de** Visualização podem ser usadas para configurar a quantidade de detalhes a serem exibidos na visualização da Lista.

* Experiência de detalhes de ativos aprimorada com a capacidade de navegar para frente e para trás entre ativos usando novos botões de navegação e contagem de ativos de visualização.

![](assets/navbtn.png)

* Novo recurso para pré-visualização de arquivos de áudio, carregados do AEM, na página de detalhes do ativo.
* Recurso Novos ativos relacionados fornecido nas propriedades do ativo. Os ativos relacionados a outros ativos de origem/derivados no AEM e publicados no Brand Portal agora têm seu relacionamento intacto no Brand Portal, com links para os ativos relacionados na página de propriedades.
* Uma nova configuração para impedir que usuários não administradores criem coleções públicas foi introduzida. As organizações podem trabalhar com a equipe de suporte da Adobe para configurar esse recurso em contas específicas.

### Aprimoramentos de pesquisa

* Recurso introduzido para voltar à mesma posição nos resultados da pesquisa, após navegar até um item de pesquisa, sem executar o query de pesquisa novamente.
* Nova contagem de resultados da pesquisa para exibir o número de resultados da pesquisa fornecidos.
* Improved File Type Search Filter with the ability to filter search results based on fine-grained MIME types such as .jpg, .png, and .psd compared to earlier Images, Documents, Multimedia options.
* Enhanced search filters for collections, with accurate time stamps instead of previous time slider functionality.
* Novos filtros de tipo de acesso foram introduzidos para procurar as coleções que são públicas ou não.

![](assets/accesstypefilter.png)

### Download optimizations

* Um único arquivo grande é baixado diretamente, sem a criação do arquivo zip, melhorando assim a velocidade e a throughput.
* O limite de download do Zip para o recurso de compartilhamento de links aumentou de 1 GB para 5 GB.

* Users can now choose to download only the custom and original files, and prevent out-of-the-box renditions, while downloading assets from Brand Portal or through the shared links feature.

![](assets/excludeautorendition.png)

### Aprimoramentos de desempenho

* Melhoria de até 100% na velocidade de download dos ativos.
* Melhoria de até 40% na resposta de pesquisa para ativos.
* Up to 40% improvement in browsing performance.

**Observação**: As melhorias citadas são conforme os testes feitos no laboratório.

### Recursos aprimorados do relatórios

**Introduced Link Share Report**
A new report, to provide information about shared links, has been introduced. O relatório Compartilhamento de links lista todos os URLs, para os ativos, compartilhados com usuários internos e externos em toda a organização no período especificado. Ele também informa quando o link foi compartilhado, por quem e quando expira.

![](assets/navigatereport.png)

**O ponto de entrada modificado para acessar o relatório** Uso de relatório agora é consolidado com outros relatórios e agora pode ser visualizado no console Relatórios de ativos. Para acessar o console Relatórios de ativos, navegue até **Criar/gerenciar relatórios** no painel de ferramentas administrativas.

![](assets/accessassetreport.png)

**A experiência do usuário aprimorada com a interface do relatórios** no Brand Portal tornou-se mais intuitiva e proporciona maior controle às organizações. Além de criar vários relatórios, os administradores agora podem revisitar os relatórios gerados e baixá-los ou excluí-los, pois esses relatórios são salvos no Brand Portal.

Cada relatório que está sendo criado pode ser personalizado adicionando ou removendo colunas padrão. Além disso, colunas personalizadas podem ser adicionadas aos relatórios Download, Expiração e Publicação para controlar seu grau de granularidade.

### Aprimoramento das ferramentas administrativas

Aprimorado o Seletor de propriedades nas ferramentas administrativas para Metadados, Pesquisa e Relatórios com recurso de avanço de tipo e navegação para simplificar a experiência do administrador.

### Outras melhorias

* Os ativos publicados no Brand Portal do AEM 6.3.2.1 e 6.4 agora podem ser disponibilizados publicamente para usuários gerais do Brand Portal, marcando a caixa de seleção Publicação de pasta pública na caixa de diálogo Replicação do Portal de marca do AEM Assets.

![](assets/public-folder-publish.png)

* Os administradores são notificados por meio de e-mails de solicitação de acesso, além das notificações na área de notificação do Portal da Marca, se alguém tiver solicitado acesso ao Portal da Marca.

## O que mudou no ponto 6.3.2 {#what-changed-in-3}

O Brand Portal 6.3.2 inclui funcionalidades novas e aprimoradas voltadas para as principais solicitações dos clientes e melhorias gerais de desempenho.

### Request access to Brand Portal {#request-access-to-brand-portal}

Users can now request access to Brand Portal using the new **need access** capability available on the login screen of Brand Portal.

![](assets/bplogin_request_access.png)

Depending on whether users have an Adobe ID or need to create an Adobe ID, users can follow the appropriate workflow to submit a request. Os administradores de produtos do Brand Portal recebem essas solicitações na área de notificação e concedem acesso por meio da Adobe Admin Console.

Para obter mais informações, consulte [Solicitar acesso ao Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Melhoria no relatório de ativos baixados {#enhancement-in-the-assets-downloaded-report}

The assets downloaded report now includes the asset download count per user within the specified date and time range. Users can download this report in .csv format and compile data such as the total download count for a licensed asset.

![](assets/reports_download_downloaded_by.png)

For more information, see Steps 3 and 6 in [Create and manage additional reports](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Brand Portal maintenance notification {#brand-portal-maintenance-notification}

Brand Portal now displays a notification banner a few days before an upcoming maintenance activity. Uma notificação de amostra:

![](assets/bp_maintenance_notification-1.png)

Para obter mais informações, consulte Notificação [](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)de manutenção do Brand Portal.

### Aprimoramento de ativos licenciados compartilhados usando o recurso de compartilhamento de link {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

While downloading licensed assets using the link share feature, you are now prompted to agree to the license agreement for those assets.

![](assets/copyright_management.png)

Para obter mais informações, consulte Etapa 12 em [Compartilhar ativos como um link](../using/brand-portal-link-share.md#shareassetsasalink).

### User picker enhancement {#user-picker-enhancement}

O desempenho do seletor de usuários agora é aprimorado para atender às necessidades dos clientes com uma grande base de usuários.

### Alterações na marca da Experience Cloud {#experience-cloud-branding-changes}

O Portal de marcas agora está em conformidade com a nova marca da Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## O que mudou na versão 6.3.1 {#what-changed-in-4}

Brand Portal 6.3.1 includes new and enhanced functionality oriented toward aligning Brand Portal with AEM.

### Interface do usuário atualizada {#upgraded-user-interface}

Para alinhar a experiência do usuário do Brand Portal com o AEM, a Adobe está migrando para a interface do usuário do Coral 3. Essa alteração melhora a utilização geral, incluindo navegação e aparência.

#### Enhanced navigational experience {#enhanced-navigational-experience}

* Quick access to administrative tools through the new Adobe logo:

![](assets/aemlogo-3.png)

* Product navigation through an overlay:

![](assets/overlay_navigation.png)

* Quick navigation to parent folders:

![](assets/navigationparentfolders.png)

* Quick search and navigation to the required content and tools:

![](assets/omnisearchicon.png)

### Enhanced browsing experience {#enhanced-browsing-experience}

* New column view to browse through nested folders:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* In the list of assets in a folder, the latest asset uploaded appears at the top.

### Enhanced search experience {#enhanced-search-experience}

* The new Omni search feature facilitates quick access to relevant content, capability, or tags through automatic suggestions as you type search keywords. A pesquisa Omni está disponível em todos os recursos de pesquisa.

![](assets/omnisearch_whatsnew.png)

* You can also add search filters to Omni search to further narrow down and quicken your search.

![](assets/omnisearch_withfilters.png)

* A nova pesquisa baseada na classificação de ativos permite que você pesquise ativos com classificações, se publicada por AEM Assets.
* The new multi-value search feature accepts multiple keywords with the AND operator to discover assets faster.
* The new search boost capability lets you improve the search relevance so that specific assets appear at the top of the search results.
* The new path-based search feature lets you provide the path to a nested folder to be able to search assets in that folder.

#### New smart tags-based search {#new-smart-tags-based-search}

If images with smart tags are published from AEM Assets to Brand Portal, you can search for these images in Brand Portal using the smart tag names as search keywords. This feature is available only for files.

### Enhanced downloading experience {#enhanced-downloading-experience}

After downloading a nested folder, you can preserve the original folder hierarchy. Os ativos dentro de uma pasta aninhada podem ser baixados em uma única pasta, em vez de pastas separadas.

### Improved performance {#improved-performance}

Enhancements in the browse, search, and download capabilities significantly improve Brand Portal performance.

### New digital rights management for assets {#new-digital-rights-management-for-assets}

Administrators can set the expiry date and time for assets before sharing them. Depois que um ativo expira, ele fica visível para visualizadores e editores, mas não é baixável. When an asset expires, administrators receive a notification.

### Enhanced asset sorting {#enhanced-asset-sorting}

Asset sorting in a folder in list view is no longer restricted to the number of assets being displayed on the first page. All assets in a folder are sorted, irrespective of whether all are listed on the first page.

### Enhanced reporting {#reporting-capabilities}

Administrators can create and manage three types of reports—assets downloaded, expired, and published. The ability to configure the columns in a report, and export the reports to CSV format is also available.

![](assets/newreport.png)

### Metadados adicionais {#additional-metadata}

O Brand Portal 6.3.1 apresenta metadados adicionais, que estão ao mesmo nível da AEM Assets 6.3. Você pode usar o formulário Editor de Schemas para controlar os metadados que devem estar visíveis na página Propriedades de ativos. Asset metadata is not visible to external link share users, who can only preview and download assets using the link share URL.

![](assets/additionsinmetadata.png)

### Recursos adicionais para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar as personalizações no wallpaper da tela de login, os administradores podem pré-visualização as alterações.

![](assets/wallpaperpreview.png)

* Depois que um administrador adiciona novos usuários, eles não precisam aceitar convites para serem adicionados ao Brand Portal, eles são adicionados automaticamente.

### Novos recursos de publicação no AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* Os administradores do AEM podem publicar schemas de metadados do AEM Assets para o Brand Portal usando o AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponível no quarto trimestre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Os administradores do AEM podem publicar todas as tags do AEM Assets para o Brand Portal usando o AEM 6.2 SP1-CFP7 e o AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Em AEM Assets, você pode publicar ativos e coleções que tenham tags, incluindo tags inteligentes. Em seguida, você pode pesquisar por esses ativos ou coleções usando essas tags como palavras-chave de pesquisa no Brand Portal.