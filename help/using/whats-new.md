---
title: Novidades do AEM Assets Brand Portal
seo-title: Novidades do AEM Assets Brand Portal
description: Dê uma olhada nos novos recursos e melhorias da versão 6.4.5.
seo-description: Dê uma olhada nos novos recursos e melhorias da versão 6.4.5.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
contentOwner: bdhar
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: referência
topic-tags: introdução
discoiquuid: provação32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: 94a3183f42e232f841a07644a89817591ca2d521

---


# Novidades do AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

O portal de marcas dos ativos Adobe Experience Manager (AEM) ajuda você a adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado. A Adobe está trabalhando para melhorar a experiência geral do Brand Portal. Veja os novos recursos e melhorias.

## O que mudou no ponto 6.4.5 {#what-changed-in-645}

O Brand Portal 6.4.5 é uma versão de recurso que tem como objetivo fornecer uma plataforma colaborativa para os usuários ativos do Brand Portal (agências/equipes externas) para fazer upload de ativos no Brand Portal e publicá-los nos ativos AEM sem precisar acessar o ambiente de criação do AEM. O recurso é nomeado como Fonte de **ativos no Portal** da marca. Este recurso melhora as experiências do cliente, fornecendo um mecanismo bidirecional para contribuir e compartilhar os ativos com outros usuários do Brand Portal distribuídos globalmente.

### Seleção de recursos no Brand Portal {#asset-sourcing-in-bp}

The Asset Sourcing feature allows AEM administrators to create new folders with an additional property named–**Asset Contribution**. A nova pasta criada é chamada como uma Contribuição *de* ativo, também conhecida como pasta *Contribuição* . Quando uma pasta de contribuição é criada no AEM, um fluxo de trabalho interno aciona duas subpastas na pasta de contribuição, a NOVA e a COMPARTILHADA.

O administrador do AEM define o requisito fazendo upload de um resumo sobre a pasta de contribuição, fazendo upload do ativo básico na pasta **SHARED** para referência, atribuindo usuários ativos do Brand Portal para acessar a pasta de contribuição e publicando a pasta de contribuição no Brand Portal. Assim que a pasta de contribuição for publicada, os usuários do Brand Portal que tiverem acesso à pasta de contribuição poderão fazer logon na instância do Brand Portal e começar a contribuir carregando conteúdo/ativos (arquivos ou pastas) na pasta **NEW** . Após carregar todo o conteúdo, os usuários do Brand Portal publicam manualmente a pasta de contribuição no AEM. Pode levar alguns minutos para importar e refletir o conteúdo/ativos publicados nos ativos AEM.

A funcionalidade existente permanece no lugar, os usuários do Brand Portal podem exibir, pesquisar e baixar ativos da pasta de contribuição, bem como de outras pastas permitidas. E os administradores podem compartilhar ainda mais a pasta de contribuição, modificar as propriedades e adicionar ativos às coleções. Consulte as notas [de versão mais recentes do Portal de](brand-portal-release-notes.md)marcas.

>[!NOTE]
>
>Os usuários do Brand Portal podem carregar conteúdo/ativos somente na pasta **NOVA** .

>[!NOTE]
>
>O limite máximo de upload para qualquer conta/locatário do Brand Portal é de **10** GB.



![](assets/asset-sourcing.png)

### Upload assets in Brand Portal {#upload-assets-in-bp}

Os usuários ativos do Brand Portal recebem notificação por pulso e por email sempre que uma pasta de contribuição é compartilhada com eles. Eles podem baixar o breve documento anexado à pasta de contribuição e baixar o conteúdo/ativos da linha de base da pasta **COMPARTILHADO** para entender o requisito.

The Brand Portal users having permission to access the contribution folder can upload assets only to the **NEW** folder. However, they can upload multiple assets or folders containing multiple assets.

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)

>[!NOTE]
>
>Brand Portal users do not have permission to delete an uploaded asset.

### Publish contribution folder to AEM Assets {#publish-assets-to-aem}

After uploading the assets in the NEW folder, Brand Portal user manually publishes the contribution folder to AEM. **** It may take few minutes to import and reflect the published content/assets in AEM Assets. The Brand Portal user and AEM administrator receive pulse/email notifications at the beginning and completion of the publishing event along with the job status (Queued/In-progress/Success). AEM and Brand Portal administrators can also view the job status from their respective interfaces.

![](assets/upload-asset5.png)

## What changed in 6.4.4 {#what-changed-in-644}

Brand Portal 6.4.4 release focuses on enhancements to text search and top customer requests. See latest Brand Portal Release Notes.[](brand-portal-release-notes.md)

### Search enhancements {#search-enhancements}

O Brand Portal 6.4.4 em diante oferece suporte à pesquisa de texto parcial no predicado de propriedade no painel de filtragem. To allow partial text search you need to enable Partial Search in Property Predicate in the search form.****

Leia para saber mais sobre pesquisa de texto parcial e pesquisa de curinga.

#### Pesquisa de frase parcial {#partial-phrase-search}

Agora você pode pesquisar ativos especificando apenas uma parte (ou seja, uma palavra ou duas) da frase pesquisada no painel de filtragem.

**Caso de usoA pesquisa de frases** parciais é útil quando você não tem certeza da combinação exata de palavras que ocorrem na frase pesquisada.

Por exemplo, se o formulário de pesquisa no Brand Portal usar o Predicado de propriedade para uma pesquisa parcial sobre o título dos ativos, a especificação do termo **campo** retornará todos os ativos com o campo de palavras em suas frases de título.

![](assets/partialphrasesearch.png)

#### Pesquisa curinga {#wildcard-search}

O Brand Portal permite o uso do asterisco (*) na consulta de pesquisa junto com uma parte da palavra na frase pesquisada.

**Caso** de uso Se você não tiver certeza das palavras exatas que ocorrem na frase pesquisada, poderá usar uma pesquisa curinga para preencher as lacunas na consulta de pesquisa.

Por exemplo, especificar **climb*** retorna todos os ativos com palavras que começam com os caracteres que **sobem** em suas frases de título se o formulário de pesquisa no Portal de marcas usar Predicado de propriedade para pesquisa parcial no título dos ativos.

![](assets/wildcard-prop.png)

Da mesma forma, especificando:

* ***climb** retorna todos os ativos que têm palavras que terminam com caracteres que **sobem** em suas frases de título.

* ***climb*** retorna todos os ativos com palavras que incluem os caracteres que **sobem** em suas frases de título.

>[!NOTE]
>
>Ao marcar a caixa de seleção Pesquisa **** parcial, **Ignorar caso** é selecionado por padrão.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## O que mudou no ponto 6.4.3 {#what-changed-in}

Brand Portal 6.4.3 release focuses on — providing organizations with an alternate alias in addition to their tenant ID in Brand Portal access URL, new folder hierarchy configuration, video support enhancements, scheduled publishing from AEM Author instance to Brand Portal, operational enhancements — and cateres to customer requests.

### Navegação de hierarquia de pastas para não administradores

Agora, os administradores podem configurar como as pastas são exibidas para usuários não administradores (editores, visualizadores e usuários convidados) no logon. [A configuração Ativar hierarquia](../using/brand-portal-general-configuration.md) de pastas é adicionada em Configurações **** gerais, no painel Ferramentas administrativas. Se a configuração for:

* **ativada**, a árvore de pastas que começa na pasta raiz está visível para usuários não administradores. Assim, concedendo a eles uma experiência de navegação semelhante aos administradores.
* **desativado**, somente as pastas compartilhadas são exibidas na página de aterrissagem.

![](assets/enable-folder-hierarchy.png)
**O caso de uso**

A funcionalidade [Ativar hierarquia](../using/brand-portal-general-configuration.md) de pastas (quando ativada) ajuda a diferenciar as pastas com os mesmos nomes compartilhados de diferentes hierarquias. Ao fazer logon, usuários não administradores agora veem as pastas pai virtual (e ancestral) das pastas compartilhadas.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

As pastas compartilhadas são organizadas nos respectivos diretórios em pastas virtuais. É possível reconhecer essas pastas virtuais com um ícone de cadeado.

Note that the default thumbnail of the virtual folders is the thumbnail image of the first shared folder.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Pesquisar em hierarquia ou caminho de pasta específicos

**O predicado Navegador** de caminho é introduzido no Formulário de pesquisa para permitir a pesquisa de ativos em um diretório específico. The default search path of search predicate for Path Browser is /content/dam/mac/&lt;tenant-id&gt;/, which can be configured by editing the default search form.**

* Admin users can use Path Browser to navigate to any folder directory on Brand Portal.
* Non-admin users can use Path Browser to navigate only to the folders (and navigate back to the parent folders) shared with them.
Por exemplo, */content/dam/mac/&lt;locatário-id&gt;/folderA/folderB/folderC* é compartilhado com um usuário não administrador. The user can search for assets within folderC using Path Browser. This user can also navigate to folderB and folderA (since they are ancestors of the folderC that is shared with the user).

![](assets/edit-search-form.png)

**The use case**

You can now restrict asset search within a specific folder you have browsed to, instead of beginning at the root folder.

Observe que a pesquisa nessas pastas retorna os resultados somente dos ativos que foram compartilhados com o usuário.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media video renditions support

Users whose AEM Author instance is on Dynamic Media hybrid mode can preview and download the dynamic media renditions, in addition to the original video files.

Para permitir a visualização e o download de execuções de mídia dinâmica em contas de locatário específicas, os administradores precisam especificar a Configuração **de Mídia** Dinâmica (URL do serviço de vídeo (URL do Gateway DM) e a ID de registro para buscar o vídeo dinâmico) na configuração de **Vídeo** no painel de ferramentas administrativas.

**Os vídeos de caso** de uso do Dynamic Media podem ser visualizados em:

* Asset details page
* Asset's card view
* Página de visualização do compartilhamento de links

As codificações de vídeo do Dynamic Media podem ser baixadas de:

* Portal de marcas
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

As organizações podem personalizar o URL do portal, tendo um prefixo alternativo no URL. Para obter um alias para o nome do locatário em seu URL de portal existente, as organizações precisam entrar em contato com o suporte da Adobe.

Observe que somente o prefixo do URL do Portal de Marcas pode ser personalizado e não o URL inteiro.\
Por exemplo, uma organização com o domínio existente **geomettrix.brand-portal.adobe.com** pode obter **geomettrixinc.brand-portal.adobe.com** criado mediante solicitação.

No entanto, a instância do autor de AEM pode ser [configurada](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) somente com o URL de ID do locatário e não com o URL de alias do locatário (alternativo).

**O caso** de uso As organizações podem atender às suas necessidades de marca ao personalizar o URL do portal, em vez de aderir ao URL fornecido pela Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Melhorias na experiência de download

A versão oferece uma experiência simplificada de download com um número reduzido de cliques e avisos, em:

* optar por baixar somente as representações (e não os ativos originais).
* baixar os ativos quando o acesso às representações originais estiver restrito.

## O que mudou no ponto 6.4.2 {#what-changed-in-1}

A versão do Brand Portal 6.4.2 traz uma variedade de recursos para atender às necessidades de distribuição de ativos das organizações e ajudá-las a atingir um grande número de usuários distribuídos globalmente por meio do acesso de convidado e da experiência ideal com downloads acelerados. O Brand Portal também oferece maior controle às organizações por meio de novas configurações para administradores, relatórios recém-adicionados e atende às solicitações dos clientes.

### Acesso de convidado

![](assets/bp-login-screen-1.png)

O portal da marca AEM permite que os convidados acessem o portal. A guest user doesn't require credentials to enter the portal and can access and download all the public folders and collections. Os usuários convidados podem adicionar ativos a seus lightbox (coleção privada) e baixar os mesmos. Eles também podem visualizar a pesquisa de tags inteligentes e os predicados de pesquisa definidos pelos administradores. A sessão de convidado não permite que os usuários criem coleções e pesquisas salvas ou as compartilhem mais, acessem configurações de pastas e coleções e compartilhem ativos como links.

Em uma organização, várias sessões de convidado simultâneas são permitidas, o que é limitado a 10% da cota total de usuários por organização.

Uma sessão de convidado permanece ativa por duas horas. Therefore, the state of the lightbox is also preserved until two hours from the session start time. After two hours, the guest session has to restart, so the lightbox state is lost.

### Downloads acelerados

Brand Portal users can leverage IBM Aspera Connect based fast downloads to get speeds up to 25x faster and enjoy a seamless download experience irrespective of their location across the globe. To download the assets faster from Brand Portal or the shared link, users need to select Enable Download Acceleration option in download dialog, provided download acceleration is enabled on their organization.****

![](assets/donload-assets-dialog-2.png)

To enable IBM Aspera based accelerated download for the organization, administrators Enable Download Acceleration option (which is disabled by default) from General Settings in the administrative tools panel. ****[](brand-portal-general-configuration.md#allow-download-acceleration) To know more about prerequisites and troubleshooting steps for downloading asset files faster from Brand Portal and shared links, refer Guide to accelerate downloads from Brand Portal.[](../using/accelerated-download.md#main-pars-header)

### User Logins Report

A new report, to track user logins, has been introduced. The User Logins report can be instrumental in enabling organizations to audit and keep a check on the delegated administrators and other users of Brand Portal.****

The report logs display names, email IDs, personas (admin, viewer, editor, guest), groups, last login, activity status, and login count of each user from Brand Portal 6.4.2 deployment until the time of report generation. Os administradores podem exportar o relatório como .csv. Juntamente com outros relatórios, o relatório Logons de usuário permite que as organizações monitorem mais detalhadamente as interações dos usuários com os recursos aprovados da marca, garantindo assim a conformidade com os escritórios de conformidade corporativos.

![](assets/user-logins-1.png)

### Acesso a representações originais

Os administradores podem restringir o acesso do usuário aos arquivos de imagem originais (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, imagem/photoshop, imagem/x-photoshop, psd, image/vnd.adobe.photoshop) e dá acesso a execuções de baixa resolução que eles baixam do Brand Portal ou link compartilhado. Esse acesso pode ser controlado no nível do grupo de usuários na guia Grupos da página Funções do usuário no painel Ferramentas administrativas.

![](assets/access-original-rend-1.png)

* Por padrão, todos os usuários podem baixar representações originais, já que o Acesso ao original está ativado para todos.
* Os administradores precisam desmarcar as respectivas caixas de seleção para impedir que um grupo de usuários acesse execuções originais.
* Se um usuário for membro de vários grupos, mas apenas um deles tiver restrições, as restrições se aplicam a esse usuário.
* As restrições não se aplicam aos administradores, mesmo sendo membros de grupos restritos.
* As permissões dos usuários que compartilham ativos como link se aplicam aos usuários que baixam ativos usando links compartilhados.

### Caminho da hierarquia de pastas nas exibições Cartão e Lista

Os cartões de pastas, na Visualização de cartão, agora exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas que estão acessando, em relação à hierarquia pai.

As informações de hierarquia de pastas são particularmente úteis na diferenciação de pastas com nomes semelhantes a outras pastas compartilhadas de uma hierarquia de pastas diferente. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, ativos/pastas com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para se ajustarem aos tamanhos dos cartões. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o mouse sobre o caminho truncado.

![](assets/folder-hierarchy1-1.png)

A Exibição de lista mostra a pasta Caminho dos ativos em uma coluna para todos os usuários do Brand Portal.

![](assets/list-view-1.png)

### Opção Visão geral para exibir as propriedades do ativo

O Brand Portal fornece a opção Visão geral para usuários não administradores (editores, visualizadores, usuários convidados) para exibir as Propriedades do ativo de ativos/pastas selecionadas. A opção Visão geral está visível:

1. Na barra de ferramentas na parte superior da seleção de um ativo/pasta.
2. Na lista suspensa ao selecionar o Seletor de painel.

Ao selecionar a opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação do ativo. Enquanto isso, na página de detalhes do ativo, selecionar a opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Novas configurações

Seis novas configurações são adicionadas aos administradores para ativar/desativar as seguintes funcionalidades em locatários específicos:

* Permitir acesso de convidado
* Permitir que os usuários solicitem acesso ao Brand Portal
* Allow administrators to delete assets from Brand Portal
* Permitir criação de coleções públicas
* Permitir a criação de coleções inteligentes públicas
* Allow Download Acceleration

As configurações acima estão disponíveis em Configurações gerais e de acesso no painel Ferramentas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### O Adobe.io hospeda a interface do usuário para configurar integrações do oAuth

A partir do Brand Portal 6.4.2, usa a interface Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para criar o aplicativo JWT, que permite a configuração de integrações de Auth para permitir a integração dos ativos AEM com o Brand Portal. Anteriormente, a interface para configurar integrações OAuth era hospedada em [https://marketing.adobe.com/developer/](https://marketing.adobe.com/developer/). Para saber mais sobre a integração dos ativos AEM com o Brand Portal para publicar ativos e coleções no Brand Portal, consulte [Configurar a integração dos ativos AEM com o Brand Portal](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## Aprimoramentos de pesquisa

Os administradores podem tornar os predicados de propriedade não sensíveis a maiúsculas e minúsculas usando o predicado de propriedade atualizado, que tem uma verificação para Ignorar maiúsculas e minúsculas. Essa opção está disponível para predicado de propriedade e predicado de propriedade de vários valores.\
No entanto, a pesquisa que não diferencia maiúsculas de minúsculas é comparativamente mais lenta do que a pesquisa padrão por predicado de propriedade. Se houver muitos predicados que não diferenciam maiúsculas de minúsculas no filtro de pesquisa, a pesquisa poderá diminuir. É, portanto, aconselhável utilizar judiciosamente a pesquisa que não diferencia maiúsculas de minúsculas.

## O que mudou na versão 6.4.1 {#what-changed-in-2}

O Brand Portal 6.4.1 é uma versão de atualização da plataforma que traz vários novos recursos e aprimoramentos vitais, como navegação, pesquisa e aprimoramentos de desempenho para oferecer experiências satisfatórias aos clientes.

### Aprimoramentos de navegação

* Novo painel Árvore de conteúdo para navegar rapidamente em uma hierarquia de ativos.

![](assets/contenttree-2.png)

* Introduzidos novos atalhos de teclado, por exemplo _(p)_ para navegação até a página de propriedades, _(e)_ para Editar e _(ctrl+c)_ para operações de cópia.
* Experiência de rolagem aprimorada e carregamento lento no cartão e exibição de lista para navegar em um grande número de ativos.
* Aprimoramento da exibição de cartão com suporte para placas de tamanho diferente com base na configuração de exibição.

![](assets/cardviewsettings-1.png)

* A exibição de cartão agora exibe o carimbo de data/hora ao passar o mouse acima do rótulo de data.

* Visualização aprimorada de Coluna com **mais detalhes** no instantâneo do ativo, que permite navegar até a página de detalhes de um ativo.

![](assets/columnmoredetail.png)

* A exibição de lista agora exibe os nomes de arquivo dos ativos na primeira coluna por padrão, além de informações sobre localidade, tipo de ativo, dimensões, tamanho, classificação e publicação. Novas configurações **de** exibição podem ser usadas para configurar a quantidade de detalhes a serem exibidos na exibição de Lista.

* Experiência de detalhes de ativos aprimorada com a capacidade de navegar para frente e para trás entre ativos usando novos botões de navegação e exibir a contagem de ativos.

![](assets/navbtn.png)

* Novo recurso para visualizar arquivos de áudio, carregados do AEM, na página de detalhes do ativo.
* Recurso Novos ativos relacionados fornecido nas propriedades do ativo. Os ativos relacionados a outros ativos de origem/derivados no AEM e publicados no Brand Portal agora têm seu relacionamento intacto no Brand Portal, com links para os ativos relacionados na página de propriedades.
* Uma nova configuração para impedir que usuários não administradores criem coleções públicas foi introduzida. As organizações podem trabalhar com a equipe de suporte da Adobe para configurar esse recurso em contas específicas.

### Aprimoramentos de pesquisa

* Recurso introduzido para voltar à mesma posição nos resultados da pesquisa, após navegar até um item de pesquisa, sem executar a consulta de pesquisa novamente.
* Nova contagem de resultados da pesquisa para exibir o número de resultados da pesquisa fornecidos.
* O Filtro de pesquisa do tipo de arquivo foi aprimorado com a capacidade de filtrar os resultados da pesquisa com base em tipos MIME refinados, como .jpg, .png e .psd, em comparação com as opções anteriores de Imagens, Documentos e Multimídia.
* Filtros de pesquisa aprimorados para coleções, com carimbos de data e hora precisos em vez da funcionalidade do controle deslizante de hora anterior.
* Novos filtros de tipo de acesso foram introduzidos para procurar as coleções que são públicas ou não.

![](assets/accesstypefilter.png)

### Otimizações de download

* Um único arquivo grande é baixado diretamente, sem a criação do arquivo zip, melhorando assim a velocidade e a throughput.
* O limite de download do Zip para o recurso de compartilhamento de links aumentou de 1 GB para 5 GB.

* Agora, os usuários podem optar por baixar apenas os arquivos personalizados e originais e impedir execuções prontas, enquanto baixam ativos do Brand Portal ou por meio do recurso de links compartilhados.

![](assets/excludeautorendition.png)

### Aprimoramentos de desempenho

* Melhoria de até 100% na velocidade de download dos ativos.
* Melhoria de até 40% na resposta de pesquisa para ativos.
* Melhoria de até 40% no desempenho da navegação.

**Observação**: As melhorias citadas são conforme os testes feitos no laboratório.

### Recursos aprimorados de relatórios

**Relatório** de compartilhamento de links introduzidoUm novo relatório, para fornecer informações sobre links compartilhados, foi introduzido. O relatório Compartilhamento de links lista todos os URLs, os ativos, compartilhados com usuários internos e externos em toda a organização no período especificado. Ele também informa quando o link foi compartilhado, por quem e quando expira.

![](assets/navigatereport.png)

**O ponto de entrada modificado para acessar o relatório** Uso de relatório agora é consolidado com outros relatórios e agora pode ser visualizado no console Relatórios de ativos. Para acessar o console Relatórios de ativos, navegue até **Criar/gerenciar relatórios** no painel de ferramentas administrativas.

![](assets/accessassetreport.png)

**A experiência do usuário aprimorada com a interface de relatórios** no Brand Portal tornou-se mais intuitiva e proporciona maior controle às organizações. Além de criar vários relatórios, os administradores agora podem revisitar os relatórios gerados e baixá-los ou excluí-los, pois esses relatórios são salvos no Brand Portal.

Cada relatório que está sendo criado pode ser personalizado adicionando ou removendo colunas padrão. Além disso, colunas personalizadas podem ser adicionadas aos relatórios Download, Expiração e Publicação para controlar seu grau de granularidade.

### Aprimoramento das ferramentas administrativas

Aprimorado o Seletor de propriedades nas ferramentas administrativas para Metadados, Pesquisa e Relatórios com recurso de avanço de tipo e navegação para simplificar a experiência administrativa.

### Outras melhorias

* Os ativos publicados no Brand Portal do AEM 6.3.2.1 e 6.4 agora podem ser disponibilizados publicamente para usuários gerais do Brand Portal, marcando a caixa de seleção Publicação de pasta pública na caixa de diálogo Replicação do Brand Portal do AEM Assets.

![](assets/public-folder-publish.png)

* Os administradores são notificados por meio de e-mails de solicitação de acesso, além das notificações na área de notificação do Portal da Marca, se alguém tiver solicitado acesso ao Portal da Marca.

## O que mudou no ponto 6.3.2 {#what-changed-in-3}

O Brand Portal 6.3.2 inclui funcionalidades novas e aprimoradas voltadas para as principais solicitações dos clientes e melhorias gerais de desempenho.

### Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Os usuários agora podem solicitar acesso ao Brand Portal usando o novo recurso de acesso****necessário disponível na tela de login do Brand Portal.

![](assets/bplogin_request_access.png)

Dependendo de os usuários terem uma Adobe ID ou precisarem criar uma Adobe ID, os usuários poderão seguir o fluxo de trabalho apropriado para enviar uma solicitação. Os administradores de produtos do Brand Portal recebem essas solicitações na área de notificação e concedem acesso por meio do Adobe Admin Console.

Para obter mais informações, consulte [Solicitar acesso ao Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Melhoria no relatório de ativos baixados {#enhancement-in-the-assets-downloaded-report}

O relatório de ativos baixados agora inclui a contagem de download de ativos por usuário dentro da data e do intervalo de tempo especificados. Os usuários podem baixar esse relatório no formato .csv e compilar dados como a contagem total de download de um ativo licenciado.

![](assets/reports_download_downloaded_by.png)

Para obter mais informações, consulte as Etapas 3 e 6 em [Criar e gerenciar relatórios](../using/brand-portal-reports.md#createandmanageadditionalreports)adicionais.

### Notificação de manutenção do Brand Portal {#brand-portal-maintenance-notification}

O Brand Portal agora exibe um banner de notificação alguns dias antes de uma atividade de manutenção futura. Uma notificação de amostra:

![](assets/bp_maintenance_notification-1.png)

Para obter mais informações, consulte Notificação [](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)de manutenção do Brand Portal.

### Aprimoramento de ativos licenciados compartilhados usando o recurso de compartilhamento de link {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Ao baixar ativos licenciados usando o recurso de compartilhamento de link, agora você é solicitado a concordar com o contrato de licença desses ativos.

![](assets/copyright_management.png)

Para obter mais informações, consulte Etapa 12 em [Compartilhar ativos como um link](../using/brand-portal-link-share.md#shareassetsasalink).

### Aprimoramento do seletor do usuário {#user-picker-enhancement}

O desempenho do seletor de usuários agora é aprimorado para atender às necessidades dos clientes com uma grande base de usuários.

### Alterações na marca da Experience Cloud {#experience-cloud-branding-changes}

O Portal de marcas agora está em conformidade com a nova marca da Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## O que mudou na versão 6.3.1 {#what-changed-in-4}

O Brand Portal 6.3.1 inclui funcionalidades novas e aprimoradas voltadas para alinhar o Brand Portal ao AEM.

### Interface do usuário atualizada {#upgraded-user-interface}

Para alinhar a experiência do usuário do Brand Portal com o AEM, a Adobe está migrando para a interface do usuário do Coral 3. Essa alteração melhora a utilização geral, incluindo navegação e aparência.

#### Experiência de navegação aprimorada {#enhanced-navigational-experience}

* Acesso rápido às ferramentas administrativas por meio do novo logotipo da Adobe:

![](assets/aemlogo-3.png)

* Navegação do produto por meio de uma sobreposição:

![](assets/overlay_navigation.png)

* Navegação rápida para pastas principais:

![](assets/navigationparentfolders.png)

* Pesquisa e navegação rápidas para o conteúdo e as ferramentas necessárias:

![](assets/omnisearchicon.png)

### Experiência de navegação aprimorada {#enhanced-browsing-experience}

* Nova exibição de coluna para navegar pelas pastas aninhadas:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* Na lista de ativos em uma pasta, o ativo mais recente carregado aparece na parte superior.

### Experiência de pesquisa aprimorada {#enhanced-search-experience}

* O novo recurso de pesquisa Omni facilita o acesso rápido a conteúdo, recursos ou tags relevantes por meio de sugestões automáticas à medida que você digita palavras-chave de pesquisa. A pesquisa Omni está disponível em todos os recursos de pesquisa.

![](assets/omnisearch_whatsnew.png)

* Você também pode adicionar filtros de pesquisa à pesquisa Omni para restringir ainda mais e acelerar sua pesquisa.

![](assets/omnisearch_withfilters.png)

* A nova pesquisa baseada na classificação de ativos permite que você pesquise ativos com classificações, se publicada nos ativos AEM.
* O novo recurso de pesquisa de vários valores aceita várias palavras-chave com o operador E para descobrir ativos mais rapidamente.
* O novo recurso de pesquisa otimizada permite melhorar a relevância da pesquisa para que ativos específicos apareçam na parte superior dos resultados da pesquisa.
* O novo recurso de pesquisa baseado em caminho permite que você forneça o caminho para uma pasta aninhada para poder pesquisar ativos nessa pasta.

#### Nova pesquisa baseada em tags inteligentes {#new-smart-tags-based-search}

Se imagens com tags inteligentes forem publicadas dos ativos AEM para o Portal de marcas, você poderá pesquisar por essas imagens no Portal de marcas usando os nomes de tags inteligentes como palavras-chave de pesquisa. Este recurso está disponível somente para arquivos.

### Experiência de download aprimorada {#enhanced-downloading-experience}

Após baixar uma pasta aninhada, é possível preservar a hierarquia da pasta original. Os ativos dentro de uma pasta aninhada podem ser baixados em uma única pasta em vez de pastas separadas.

### Desempenho aprimorado {#improved-performance}

Os aprimoramentos nos recursos de navegação, pesquisa e download melhoram significativamente o desempenho do Brand Portal.

### Novo gerenciamento de direitos digitais para ativos {#new-digital-rights-management-for-assets}

Os administradores podem definir a data e a hora de expiração dos ativos antes de compartilhá-los. Depois que um ativo expira, ele fica visível para visualizadores e editores, mas não é baixável. Quando um ativo expira, os administradores recebem uma notificação.

### Classificação de ativos aprimorada {#enhanced-asset-sorting}

A classificação de ativos em uma pasta na exibição de lista não está mais restrita ao número de ativos exibidos na primeira página. Todos os ativos em uma pasta são classificados, independentemente de todos estarem listados na primeira página.

### Relatório aprimorado {#reporting-capabilities}

Os administradores podem criar e gerenciar três tipos de relatórios: ativos baixados, expirados e publicados. A capacidade de configurar as colunas em um relatório e exportar os relatórios para o formato CSV também está disponível.

![](assets/newreport.png)

### Metadados adicionais {#additional-metadata}

O Brand Portal 6.3.1 apresenta metadados adicionais, que são iguais aos ativos AEM 6.3. Você pode usar o formulário do Editor de esquema para controlar os metadados que devem estar visíveis na página Propriedades dos ativos. Os metadados do ativo não estão visíveis para usuários de compartilhamento de link externo, que só podem visualizar e baixar ativos usando o URL de compartilhamento de link.

![](assets/additionsinmetadata.png)

### Recursos adicionais para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar as personalizações no wallpaper da tela de logon, os administradores podem visualizar as alterações.

![](assets/wallpaperpreview.png)

* Depois que um administrador adiciona novos usuários, eles não precisam aceitar convites para serem adicionados ao Brand Portal, eles são adicionados automaticamente.

### Novos recursos de publicação no AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* Os administradores do AEM podem publicar o esquema de metadados dos ativos AEM para o Brand Portal usando o AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponível no quarto trimestre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Os administradores do AEM podem publicar todas as tags dos ativos AEM para o Portal de marcas usando o AEM 6.2 SP1-CFP7 e o AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Em ativos AEM, você pode publicar ativos e coleções que tenham tags, incluindo tags inteligentes. Em seguida, você pode pesquisar por esses ativos ou coleções usando essas tags como palavras-chave de pesquisa no Brand Portal.

## Frequently asked questions {#frequently-asked-questions}

**Ques. Perderei o acesso a ativos, recursos ou configurações existentes que criei?**
**Ans.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não são afetados e seu conteúdo permanece intacto.

**Ques. Quando eu vou mudar para a nova versão do Brand Portal?**
**Ans.** O Brand Portal 6.4.4 foi lançado para produção em fevereiro de 2019. A próxima versão do Brand Portal deverá ser lançada no terceiro trimestre de 2019.

>[!NOTE]
>
>O cronograma de liberação é provisório e está sujeito a alterações. Entre em contato com seu Gerente de contas da Adobe ou com o Suporte ao cliente para obter o cronograma atualizado.

**Ques. Meus usuários serão afetados?**
**Ans.** Essa alteração ocorre exclusivamente no Brand Portal, portanto não há impacto para os usuários finais.

**Ques. Há alguma ação necessária da minha parte?**
**Ans.** Não há nenhuma ação necessária para o administrador. Após obter acesso ao novo Brand Portal, consulte a documentação para ver todos os sinos e assobios.

**Ques. Com quem eu entro em contato com as perguntas?**
**Ans.** Entre em contato com seu Gerente de conta da Adobe ou com o Suporte ao cliente.