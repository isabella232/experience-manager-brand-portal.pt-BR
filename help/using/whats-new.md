---
title: Novidades do AEM Assets Brand Portal
seo-title: Novidades do AEM Assets Brand Portal
description: Analise os novos recursos e melhorias para 6.4.4.
seo-description: Analise os novos recursos e melhorias para 6.4.4.
uuid: 2 c 59 d 738-9 b 53-4 f 25-a 205-13 bf 75 c 80 b 77
contentOwner: bdhar
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
topic-tags: introdução
discoiquuid: fec 32 ca 3-142 b -4 a 11-9 b 92-5113 fc 27277 a
translation-type: tm+mt
source-git-commit: cbb64eb8a79480a1ccedbe5131a38ddf6eaec88d

---


# Novidades do AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

O Adobe Experience Manager (AEM) Assets Brand Portal ajuda você a adquirir, controlar e distribuir com segurança ativos criativos aprovados a terceiros e usuários empresariais internos em todos os dispositivos. Isso ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o mercado de ativos e reduz o risco de acesso não autorizado e não autorizado. A Adobe está trabalhando para melhorar a experiência geral do Portal de marcas. Aqui está uma novidade nos novos recursos e aprimoramentos.

## O que mudou em 6.4.4 {#what-is-changing-in}

A versão do Brand Portal 6.4.4 foca em melhorias na pesquisa de texto e nas principais solicitações do cliente. Consulte Notas de versão do [Portal de marca mais recentes](brand-portal-release-notes.md).

### Aprimoramentos de pesquisa {#search-enhancements}

A marca do Brand Portal 6.4.4 é compatível com a pesquisa parcial de texto no predicado da propriedade no painel de filtragem. Para permitir a pesquisa parcial de texto, é necessário ativar **a Pesquisa parcial** no Predicado de propriedade no formulário de pesquisa.

Faça a leitura para saber mais sobre pesquisa de texto parcial e pesquisa curinga.

#### Pesquisa de frase parcial {#partial-phrase-search}

Agora é possível pesquisar ativos especificando apenas uma parte (ou seja, uma ou duas) da frase pesquisada no painel de filtragem.

**A pesquisa de frase de caso**
parcial é útil quando você não tem certeza da combinação exata de palavras que ocorrem na frase pesquisada.

Por exemplo, se o formulário de pesquisa no Brand Portal usar o Predicado de propriedade para a pesquisa parcial no título de ativos, a especificação do termo **camp** retorna todos os ativos com a palavra camp na frase de título.

![](assets/partialphrasesearch.png)

#### Pesquisa de curinga {#wildcard-search}

O Brand Portal permite usar o asterisco (*) na consulta de pesquisa junto com uma parte da palavra na frase pesquisada.

**Caso
de uso** caso não tenha certeza das palavras exatas que estão acontecendo na frase pesquisada, você pode usar uma pesquisa curinga para preencher as lacunas na consulta de pesquisa.

Por exemplo, especificar **escalada *** retorna todos os ativos que têm palavras que começam com os caracteres **escalada** na frase de título se o formulário de pesquisa no Brand Portal usa o Predicado de propriedade para pesquisa parcial no título de ativos.

![](assets/wildcard-prop.png)

Da mesma maneira, especificando:

* *** escalada** retorna todos os ativos que têm palavras que terminam com caracteres **escalada** na frase de título.

* *** escalada *** retorna todos os ativos que têm palavras que incluem os caracteres **escalada** na frase de título.

>[!NOTE]
>
>Ao selecionar **a caixa de seleção Pesquisa** parcial, **Ignorar caso** está selecionado por padrão.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## O que mudou em 6.4.3 {#what-changed-in}

A versão do Brand Portal 6.4.3 foca em— fornecer às organizações um alias alternativo além da ID do locatário no URL de acesso do Brand Portal, a configuração da nova hierarquia de pastas, as melhorias no suporte a vídeos, a publicação programada da instância do autor de AEM para o Brand Portal, as melhorias operacionais— e atender às solicitações do cliente.

### Navegação de hierarquia de pastas para não administradores

Os administradores agora podem configurar como as pastas são exibidas para usuários não administradores (Editores, Visualizadores e Usuários convidados) no logon. [A configuração Ativar hierarquia](../using/brand-portal-general-configuration.md) da pasta é adicionada em **Configurações** gerais, no painel Ferramentas administrativas. Se a configuração for:

* **ativada**, a árvore de pastas começando pela pasta raiz é visível para usuários não administradores. Assim, concede a eles uma experiência de navegação semelhante aos administradores.
* **desativadas**, somente as pastas compartilhadas são exibidas na página de aterrissagem.

![](assets/enable-folder-hierarchy.png)**O caso de uso**

A funcionalidade [Ativar hierarquia](../using/brand-portal-general-configuration.md) de pastas (quando ativada) ajuda a diferenciar as pastas com os mesmos nomes compartilhados de hierarquias diferentes. Ao fazer logon, os usuários não administradores agora veem as pastas pai pai (e ancestral) das pastas compartilhadas.![](assets/disabled-folder-hierarchy1-2.png)![](assets/enabled-hierarchy1-2.png)
 

As pastas compartilhadas são organizadas nos respectivos diretórios nas pastas virtuais. Você pode reconhecer essas pastas virtuais com um ícone de cadeado.

Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Pesquisar em hierarquia ou caminho de pasta específica

**O predicado do Navegador** de caminhos é introduzido no Formulário de pesquisa para permitir a pesquisa de ativos em um diretório específico. O caminho de pesquisa padrão do predicado de pesquisa para Navegador de caminhos é */content/dam/mac/ &lt; tenant-id &gt;/*, que pode ser configurado ao editar o formulário de pesquisa padrão.

* Os usuários administradores podem usar o Navegador de caminho para navegar até qualquer diretório de pastas no Brand Portal.
* Usuários não administradores podem usar o Navegador de caminho para navegar somente para as pastas (e navegar para as pastas pai) compartilhadas com eles.
Por exemplo, */content/dam/mac/ &lt; tenant-id &gt;/foldera/folderb/folderc* é compartilhado com um usuário não administrador. O usuário pode pesquisar ativos no folderc usando o Navegador de caminho. Esse usuário também pode navegar para folderb e foldera (já que são ancestrais do folderc que é compartilhado com o usuário).

![](assets/edit-search-form.png)

**O caso de uso**

Agora você pode restringir a pesquisa do ativo dentro de uma pasta específica ao qual você tenha navegado, em vez de começar na pasta raiz.

Observe que a pesquisa nessas pastas retorna resultados somente dos ativos que foram compartilhados com o usuário.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Suporte para representações de vídeo de Dynamic Media

Os usuários cuja instância de autor de AEM está no modo híbrido de mídia dinâmica podem visualizar e baixar as representações de mídia dinâmica, além dos arquivos de vídeo originais.

Para permitir a visualização e o download de representações de mídia dinâmica em contas de locatário específicas, os administradores precisam especificar **a Configuração de mídia dinâmica** (URL do serviço de vídeo (URL do gateway DM) e a ID de registro para buscar o vídeo dinâmico) na configuração **de Vídeo** no painel de ferramentas administrativas.

**O caso**
de uso de vídeos de Dynamic Media pode ser visualizado em:

* Página de detalhes do ativo
* Exibição de cartão do ativo
* Página de visualização de compartilhamento de link

Os códigos de vídeo de Dynamic Media podem ser baixados de:

* Portal de marcas
* Link compartilhado

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publicação programada para o Brand Portal

A instância do autor de ativos (e pastas) de publicação do fluxo de trabalho do [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) para o Brand Portal pode ser agendada para uma data posterior, hora.

Da mesma forma, os ativos publicados podem ser removidos do portal em uma data posterior (tempo), agendando o fluxo de trabalho Cancelar publicação do portal de marca.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias configuráveis do locatário no URL

As organizações podem obter o URL do portal personalizado com um prefixo alternativo no URL. Para obter um alias do nome do inquilino no URL do portal existente, as organizações precisam entrar em contato com o suporte da Adobe.

Observe que apenas o prefixo do URL do Brand Portal pode ser personalizado e não todo o URL.\
Por exemplo, uma organização com domínio existente **geomettrix.brand-portal.adobe.com** pode obter **geomettrixinc.brand-portal.adobe.com** criado mediante solicitação.

No entanto, a instância do Autor de AEM pode ser [configurada](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) somente com o URL da ID do inquilino e não com o URL do alias (alternativo).

**O caso
de uso** Organizações pode atender às suas necessidades de marca ao obter o URL do portal personalizado, em vez de manter o URL fornecido pela Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Aprimoramentos de experiência de download

A versão oferece uma experiência simplificada de download com um número reduzido de cliques e avisos, em:

* optar por baixar apenas as representações (e não os ativos originais).
* download dos ativos quando o acesso às representações originais é restrito.

## O que mudou em 6.4.2 {#what-changed-in-1}

A versão do Brand Portal 6.4.2 traz uma variedade de recursos para atender às necessidades de distribuição de ativos das organizações e ajuda a atingir um grande número de usuários distribuídos globalmente por meio de acesso a convidado e experiência ideal com downloads acelerados. O Brand Portal também oferece maior controle a organizações por meio de novas configurações para administradores, relatório recém-adicionado e caters para solicitações de clientes.

### Acesso de convidado

![](assets/bp-login-screen-1.png)

O portal da marca do AEM permite o acesso do convidado ao portal. Um usuário convidado não requer credenciais para entrar no portal e pode acessar e baixar todas as pastas públicas e coleções. Os usuários convidados podem adicionar ativos ao lightbox (coleção privada) e baixar os mesmos. Eles também podem exibir a pesquisa inteligente de tags e a pesquisa configurada por administradores. A sessão de convidados não permite que os usuários criem coleções e pesquisas salvas ou compartilhá-las ainda mais, acessar configurações de pastas e coleções e compartilhar ativos como links.

Em uma organização, várias sessões de convidados simultâneos são permitidas, que é limitada a 10% da cota total de usuários por organização.

Uma sessão de convidados permanece ativa por duas horas. Portanto, o estado do lightbox também é preservado até duas horas da hora de início da sessão. Após duas horas, a sessão de convidados é reiniciada, portanto o estado do lightbox é perdido.

### Downloads acelerados

Os usuários do Brand Portal podem aproveitar os downloads rápidos do IBM Aspera com base em downloads rápidos para acelerar até 25 vezes mais rápido e desfrutar de uma experiência de download contínua independentemente de sua localização em todo o mundo. Para baixar os ativos mais rapidamente do Portal da marca ou do link compartilhado, os usuários precisam selecionar **Ativar a aceleração** de download na caixa de diálogo de download, desde que a aceleração de download esteja ativada na organização.

![](assets/donload-assets-dialog-2.png)

Para ativar o download acelerado pela IBM para a organização, os administradores **ativam a opção Aceleração** de download (que é desativada por padrão) das Configurações [gerais](brand-portal-general-configuration.md#allow-download-acceleration) no painel de ferramentas administrativas. Para saber mais sobre pré-requisitos e etapas de solução de problemas para baixar arquivos de ativos mais rapidamente no Portal da marca e links compartilhados, consulte [Guia para acelerar os downloads do Brand Portal](../using/accelerated-download.md#main-pars-header).

### Relatório de logons de usuário

Foi introduzido um novo relatório para rastrear logons de usuário. O **relatório de logons** de usuário pode ser instrumentais para permitir que as organizações auditem e mantenham uma verificação dos administradores delegados e de outros usuários do Portal da marca.

O relatório registra nomes de exibição, IDs de email, personalizadas (administrador, visualizador, editor, convidado), grupos, último logon, status da atividade e contagem de login de cada usuário da implantação do Portal da marca 6.4.2 até a hora da geração do relatório. Os administradores podem exportar o relatório como. csv. Juntamente com outros relatórios, o relatório de Logons de usuário permite que as organizações monitorem mais detalhadamente as interações do usuário com os recursos de marca aprovados, garantindo dessa forma a conformidade com os escritórios de conformidade corporativa.

![](assets/user-logins-1.png)

### Acesso a representações originais

Os administradores podem restringir o acesso do usuário a arquivos de imagem originais (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-bitmap, x-portable-bitmap, x-portable-pixmap, x-xpixmap, x-xon, image/photom photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) e conceder acesso a representações de baixa resolução que baixam do Brand Portal ou link compartilhado. Esse acesso pode ser controlado no nível do grupo de usuários na guia Grupos da página Funções do usuário no painel de ferramentas administrativas.

![](assets/access-original-rend-1.png)

* Por padrão, todos os usuários podem baixar representações originais como o Acesso ao original está ativado para todos.
* Os administradores precisam cancelar a seleção das respectivas caixas de seleção para impedir que um grupo de usuários acesse representações originais.
* Se um usuário for membro de vários grupos, mas apenas um deles tiver restrições, as restrições se aplicarão a esse usuário.
* As restrições não se aplicam a administradores, embora sejam membros de grupos restritos.
* As permissões do usuário que compartilham ativos como link se aplicam aos usuários que baixam ativos usando links compartilhados.

### Caminho da hierarquia de pastas nas exibições de Cartão e Lista

Cartões de pastas, na Exibição de cartão, agora exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas, estão acessando, em relação à hierarquia pai.

As informações de hierarquia de pastas são especialmente úteis na diferenciação das pastas com nomes semelhantes a outras pastas compartilhadas a partir de uma hierarquia de pasta diferente. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, os ativos /folders com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para ajustar os tamanhos do cartão. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o mouse sobre o caminho truncado.

![](assets/folder-hierarchy1-1.png)

A Exibição de lista mostra o Caminho de pasta dos ativos em uma coluna para todos os usuários do Brand Portal.

![](assets/list-view-1.png)

### Opção Visão geral para exibir propriedades de ativos

O Brand Portal oferece a opção Visão geral para usuários não administradores (Editores, Visualizadores, Usuários convidados) para exibir Propriedades de ativos de pastas/ativos selecionados. A opção Visão geral está visível:

1. Na barra de ferramentas na parte superior, selecione um ativo/pasta.
2. No menu suspenso ao selecionar o Seletor de painéis.

Ao selecionar a opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação de ativos. Enquanto a página de detalhes do ativo selecionando a opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Novas configurações

Seis novas configurações são adicionadas para administradores ativarem/desativarem a seguinte funcionalidade em inquilinos específicos:

* Permitir acesso de convidado
* Permitir que os usuários solicitem acesso ao Brand Portal
* Permitir que os administradores excluam ativos do Brand Portal
* Permitir a criação de coleções públicas
* Permitir a criação de coleções inteligentes públicas
* Permitir aceleração de download

As configurações acima estão disponíveis em Acesso e configurações gerais no painel de ferramentas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe. io hosts UI para configurar integrações oauth

A versão brand .4.2 do Brand Portal usa a interface Adobe. io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para criar aplicativos JWT, que permitem a configuração de integrações oauth para permitir a integração do AEM Assets com o Brand Portal. Anteriormente, a interface do usuário para configurar as integrações oauth era hospedada em [https://marketing.adobe.com/developer/](https://marketing.adobe.com/developer/). Para saber mais sobre a integração de ativos AEM com o Brand Portal para publicar ativos e coleções no Brand Portal, consulte [Configurar a integração do AEM Assets com o Brand Portal](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## Aprimoramentos de pesquisa

Os administradores podem fazer com que a propriedade determine maiúsculas de minúsculas usando o predicado de propriedade atualizado, que tem uma verificação de Ignorar caso. Essa opção está disponível para predicado de propriedade e previsão de propriedade multivalor.\
No entanto, a pesquisa que não diferencia maiúsculas e minúsculas é comparada de forma comparativa à pesquisa padrão do predicado de propriedade. Se houver muitos predicados sem maiúsculas e minúsculas no filtro de pesquisa, a pesquisa pode desacelerar. Portanto, é recomendável usar a pesquisa sensível a maiúsculas e minúsculas de forma errada.

## O que mudou em 6.4.1 {#what-changed-in-2}

O Brand Portal 6.4.1 é uma versão de atualização da plataforma que traz vários recursos novos e aprimoramentos vitais, como navegação, pesquisa e desempenho de desempenho, para fornecer experiências de clientes com desempenhos.

### Aprimoramentos de navegação

* Novo trilho de árvore para navegar rapidamente em uma hierarquia de ativos.

![](assets/contenttree-2.png)

* Introduziu novos atalhos do teclado, por exemplo _(p)_ para navegação em página de propriedades, _(e)_ para Editar e _(ctrl + c)_ para operações de cópia.
* Melhoria na rolagem, na experiência de carregamento lento na exibição de cartão e em lista para navegar em um grande número de ativos.
* Exibição de cartão aprimorada com suporte para cartões de tamanho diferente com base na configuração de visualização.

![](assets/cardviewsettings-1.png)

* A exibição de cartão agora exibe carimbo de data/hora ao passar o mouse sobre o rótulo da data.

* Exibição de coluna aprimorada com **Mais detalhes** abaixo do instantâneo do ativo, que permite que você navegue até a página de detalhes de um ativo.

![](assets/columnmoredetail.png)

* A exibição de lista agora exibe os nomes de arquivo dos ativos na primeira coluna, por padrão, além de local, tipo de ativo, dimensões, tamanho, classificação e informações de publicação. As Novas **Configurações** de exibição podem ser usadas para configurar a quantidade de detalhes exibida na exibição de Lista.

* Experiência de detalhes do ativo aprimorada com capacidade de navegar entre os ativos usando novos botões de navegação e exibir a contagem de ativos.

![](assets/navbtn.png)

* Novo recurso para visualizar arquivos de áudio, carregados do AEM, na página de detalhes do ativo.
* Novo recurso Ativos relacionados fornecido nas propriedades do Ativo. Os ativos relacionados com outros ativos derivados/derivados no AEM e publicados no Brand Portal agora têm o relacionamento intacto no Portal da marca, com links para os ativos relacionados na página de propriedades.
* Foi introduzida uma nova configuração para restringir usuários não administradores de criar coleções públicas. As organizações podem trabalhar com a equipe de suporte da Adobe para configurar esse recurso em contas específicas.

### Aprimoramentos de pesquisa

* Recurso introduzido para retornar à mesma posição nos resultados da pesquisa, após a navegação até um item de pesquisa, sem executar a consulta de pesquisa novamente.
* Uma nova contagem de resultados de pesquisa para exibir o número de resultados da pesquisa foi fornecida.
* Filtro de pesquisa de tipo de arquivo aprimorado com a capacidade de filtrar os resultados da pesquisa com base em tipos MIME refinados, como.jpg. png e. psd comparados com imagens anteriores, Documentos, opções Multimídia.
* Filtros de pesquisa aprimorados para coleções, com carimbos de data e hora precisos em vez da funcionalidade deslizante de tempo anterior.
* Novos filtros de tipo de acesso foram introduzidos para pesquisar as coleções públicas ou não públicas.

![](assets/accesstypefilter.png)

### Otimizações de download

* Um único arquivo grande é baixado diretamente, sem a criação do arquivo zip, melhorando assim a velocidade e o resultado.
* O limite de download de zip para o recurso de compartilhamento de links aumentou para 5 GB, de 1 GB.

* Os usuários agora podem optar por baixar apenas os arquivos personalizados e originais, além de evitar representações prontas para uso, ao baixar ativos do Portal da marca ou pelo recurso de links compartilhados.

![](assets/excludeautorendition.png)

### Aprimoramentos de desempenho

* Melhoria de até 100% na velocidade de download dos ativos.
* Melhoria de até 40% na resposta de pesquisa para ativos.
* Melhoria de até 40% no desempenho de navegação.

**Observação**: Aprimoramentos citados são os testes realizados no laboratório.

### Recursos aprimorados de relatórios

**Relatório de compartilhamento de links apresentado** Um novo relatório, para fornecer informações sobre links compartilhados, foi introduzido. O relatório Compartilhamento de links lista todos os urls, os ativos, compartilhados com usuários internos e externos na organização no período especificado. Ele também informa quando o link foi compartilhado, por quem e quando expira.

![](assets/navigatereport.png)

**O ponto de entrada para acessar o relatório de Uso do relatório**
de uso agora é consolidado com outros relatórios e agora pode ser visualizado no console Relatórios de ativo. Para acessar o console Relatórios de ativos, navegue até **Criar/gerenciar relatórios** no painel de ferramentas administrativas.

![](assets/accessassetreport.png)

**A experiência do usuário aprimorada com relatórios de**
relatórios no Portal de marca se tornou mais intuitiva e imprime maior controle para organizações. Além de criar vários relatórios, os administradores agora podem revisitar os relatórios gerados e baixá-los ou excluí-los, já que esses relatórios são salvos no Portal da marca.

Cada relatório que está sendo criado pode ser personalizado adicionando ou removendo colunas padrão. Além disso, as colunas personalizadas podem ser adicionadas aos relatórios de Download, Expiração e Publicação para controlar o grau de granularidade.

### Ferramentas administrativas aprimoradas

O Seletor de propriedade aprimorado nas Ferramentas administrativas para metadados, pesquisa e relatórios com recursos de tipo e navegação para simplificar a experiência de administrador.

### Outras melhorias

* Os ativos publicados no Brand Portal a partir do AEM 6.3.2.1 e 6.4 agora podem ser tornados publicalmente disponíveis para usuários gerais do Brand Portal, marcando a caixa de seleção Publicação de pastas públicas na caixa de diálogo Replicação do Portal de marcas do AEM Assets.

![](assets/public-folder-publish.png)

* Os administradores são notificados por e-mails de solicitação de acesso, além das notificações na área de notificação do Brand Portal, se alguém solicitou acesso ao Portal da marca.

## O que mudou em 6.3.2 {#what-changed-in-3}

O Brand Portal 6.3.2 inclui uma funcionalidade nova e aprimorada voltada para as principais exigências do cliente e melhorias gerais de desempenho.

### Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Agora os usuários podem solicitar acesso ao Brand Portal usando o novo recurso**** de acesso disponível na tela de logon do Portal da marca.

![](assets/bplogin_request_access.png)

Se os usuários tiverem uma Adobe ID ou precisam criar uma Adobe ID, os usuários poderão seguir o fluxo de trabalho apropriado para enviar uma solicitação. Os administradores de produtos do Brand Portal recebem solicitações em sua área de notificação e concedem acesso por meio do Adobe Admin Console.

Para obter mais informações, consulte [Solicitar acesso ao Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Aprimoramento no relatório baixado de ativos {#enhancement-in-the-assets-downloaded-report}

O relatório baixado agora inclui a contagem de downloads de ativos por usuário dentro da data e do intervalo de tempo especificados. Os usuários podem baixar este relatório no formato. csv e compilar dados como a contagem total de download para um ativo licenciado.

![](assets/reports_download_downloaded_by.png)

Para obter mais informações, consulte Etapas 3 e 6 em [Criar e gerenciar relatórios adicionais](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Notificação de manutenção do Brand Portal {#brand-portal-maintenance-notification}

O Brand Portal agora exibe um banner de notificação alguns dias antes de uma atividade de manutenção futura. Uma notificação de amostra:

![](assets/bp_maintenance_notification-1.png)

Para obter mais informações, consulte [Notificação de manutenção do Brand Portal](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### Aprimoramento de ativos licenciados compartilhados usando o recurso compartilhar link {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Ao baixar ativos licenciados usando o recurso de compartilhamento de links, agora você é solicitado a concordar com o contrato de licença desses ativos.

![](assets/copyright_management.png)

Para obter mais informações, consulte a Etapa 12 em [Compartilhar ativos como um link](../using/brand-portal-link-share.md#shareassetsasalink).

### Melhoria no seletor de usuários {#user-picker-enhancement}

O desempenho do seletor de usuários agora é aprimorado para atender às necessidades dos clientes com uma grande base de usuários.

### Alterações de marca da Experience Cloud {#experience-cloud-branding-changes}

O Brand Portal agora está em conformidade com a nova marca da Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## O que mudou em 6.3.1 {#what-changed-in-4}

O Brand Portal 6.3.1 inclui uma funcionalidade nova e aprimorada voltada para o alinhamento do Portal da marca com o AEM.

### Interface atualizada do usuário {#upgraded-user-interface}

Para alinhar a experiência do usuário do Brand Portal com o AEM, a Adobe está migrando para a interface do usuário Coral 3. Essa alteração melhora a utilização geral, incluindo a navegação e a aparência.

#### Experiência de navegação aprimorada {#enhanced-navigational-experience}

* Acesso rápido a ferramentas administrativas por meio do novo logotipo da Adobe:

![](assets/aemlogo-3.png)

* Navegação do produto por meio de uma sobreposição:

![](assets/overlay_navigation.png)

* Navegação rápida para pastas pai:

![](assets/navigationparentfolders.png)

* Pesquisa e navegação rápidas para o conteúdo e as ferramentas necessários:

![](assets/omnisearchicon.png)

### Experiência de navegação aprimorada {#enhanced-browsing-experience}

* Nova exibição de coluna para navegar pelas pastas aninhadas:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* Na lista de ativos em uma pasta, o ativo mais recente carregado aparece na parte superior.

### Experiência de pesquisa aprimorada {#enhanced-search-experience}

* O novo recurso de pesquisa Omni facilita o acesso rápido a conteúdos, recursos ou tags relevantes por meio de sugestões automáticas à medida que você digita palavras-chave de pesquisa. A pesquisa Omni está disponível em todos os recursos de pesquisa.

![](assets/omnisearch_whatsnew.png)

* Você também pode adicionar filtros de pesquisa à pesquisa Omni para restringir ainda mais e acelerar sua pesquisa.

![](assets/omnisearch_withfilters.png)

* A nova pesquisa baseada em classificação do ativo permite pesquisar ativos com classificações, se publicados nos ativos AEM.
* O novo recurso de pesquisa de vários valores aceita várias palavras-chave com o operador E para descobrir ativos mais rapidamente.
* O novo recurso de reforço de pesquisa permite melhorar a relevância da pesquisa para que ativos específicos sejam exibidos na parte superior dos resultados da pesquisa.
* O novo recurso de pesquisa baseado em caminho permite que você forneça o caminho para uma pasta aninhada para poder pesquisar ativos nessa pasta.

#### Nova pesquisa baseada em tags inteligentes {#new-smart-tags-based-search}

Se as imagens com tags inteligentes forem publicadas do AEM Assets para o Brand Portal, você pode pesquisar essas imagens no Brand Portal usando os nomes das tags inteligentes como palavras-chave de pesquisa. Esse recurso está disponível apenas para arquivos.

### Experiência de download aprimorada {#enhanced-downloading-experience}

Após baixar uma pasta aninhada, é possível preservar a hierarquia original de pastas. Os ativos dentro de uma pasta aninhada podem ser baixados em uma única pasta em vez de pastas separadas.

### Desempenho aprimorado {#improved-performance}

Os aprimoramentos na navegação, pesquisa e recursos de download melhoram significativamente o desempenho do Brand Portal.

### Novo gerenciamento de direitos digitais para ativos {#new-digital-rights-management-for-assets}

Os administradores podem definir a data e a hora de expiração para os ativos antes de compartilhá-los. Depois que um ativo expira, ele fica visível para visualizadores e editores, mas não para download. Quando um ativo expira, os administradores recebem uma notificação.

### Classificação de ativos aprimorada {#enhanced-asset-sorting}

A classificação do ativo em uma pasta na exibição de lista não está mais limitada ao número de ativos que estão sendo exibidos na primeira página. Todos os ativos em uma pasta são classificados, independentemente de todos serem listados na primeira página.

### Relatórios aprimorados {#reporting-capabilities}

Os administradores podem criar e gerenciar três tipos de relatórios: os ativos baixados, expirados e publicados. A capacidade de configurar as colunas em um relatório e exportar os relatórios para o formato CSV também está disponível.

![](assets/newreport.png)

### Metadados adicionais {#additional-metadata}

O Brand Portal 6.3.1 introduz metadados adicionais, que são semelhantes ao AEM Assets 6.3. Você pode usar o formulário Editor de esquema para controlar os metadados que devem estar visíveis na página Propriedades dos ativos. Os metadados do ativo não estão visíveis para usuários de link externo, que podem apenas visualizar e baixar ativos usando o URL de compartilhamento de links.

![](assets/additionsinmetadata.png)

### Recursos adicionais para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar as personalizações no papel de parede de tela de logon, os administradores podem visualizar as alterações.

![](assets/wallpaperpreview.png)

* Depois que um administrador adiciona novos usuários, eles não precisam aceitar convites para serem adicionados ao Brand Portal, eles são adicionados automaticamente.

### Novos recursos de publicação no AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* Os administradores do AEM podem publicar esquemas de metadados do AEM Assets para o Brand Portal usando o AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponível em Q 4 2017.

![](assets/publish_metadataschemaaemassets.png)

* Os administradores do AEM podem publicar todas as tags do AEM Assets no Portal da marca usando o AEM 6.2 SP 1-CFP 7 e o AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* No AEM Assets, é possível publicar ativos e coleções com tags, incluindo tags inteligentes. Você pode pesquisar esses ativos ou coleções usando essas tags como palavras-chave de pesquisa no Brand Portal.

## Frequently asked questions {#frequently-asked-questions}

**Qus. Perderei o acesso a quaisquer ativos, recursos ou configurações existentes que criei?****Anos.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não serão afetados e seu conteúdo permanecerá intacto.

**Fragmentos. Quando estou indo para a nova versão do Brand Portal?****Anos.** O Brand Portal 6.4.4 foi lançado na produção em fevereiro de 2019. Espera-se que a versão do próximo Portal de marca seja lançada em Q 3 2019.

>[!NOTE]
>
>A programação de lançamento é tentativa e sujeita a alteração. Entre em contato com seu Gerente de conta da Adobe ou com o Suporte ao cliente para obter o agendamento atualizado da versão.

**Fragmentos. Meus usuários serão afetados?****Anos.** Essa alteração está no Portal da marca, portanto não há impacto sobre os usuários finais.

**Fragmentos. Há alguma ação necessária na minha parte?****Anos.** Não há nenhuma ação exigida pelo administrador. Depois de obter acesso ao novo Brand Portal, consulte a documentação para ver todos os bells e whistles.

**Fragmentos. Quem posso entrar em contato com perguntas?****Anos.** Entre em contato com seu Gerente de conta da Adobe ou com o Suporte ao cliente.
