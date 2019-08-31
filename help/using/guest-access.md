---
title: Acesso de convidado ao Brand Portal
seo-title: Acesso de convidado ao Brand Portal
description: Permita o acesso a convidados e salve o esforço para integrar vários usuários que não precisam ser autenticados.
seo-description: Permita o acesso a convidados e salve o esforço para integrar vários usuários que não precisam ser autenticados.
uuid: edb 4378 d -1710-44 a 2-97 a 6-594 d 99 f 62 fff
contentOwner: mgulati
topic-tags: introdução
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: b 9 e 9 fe 7 b -0373-42 d 1-851 b -7 c 76 b 47657 c 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Acesso de convidado ao Brand Portal {#guest-access-to-brand-portal}

O portal da marca do AEM permite o acesso do convidado ao portal. Um usuário convidado não precisa de credenciais para entrar no portal e tem acesso aos ativos públicos (e coleções) do portal. Os usuários na sessão de convidados podem adicionar ativos ao lightbox (coleção privada) e baixar o mesmo até que sua sessão seja dura, ou seja, 2 horas a partir do início da sessão, a menos que o usuário do convidado escolha [[! Sessão final do UICONTROL]](#exit-guest-session).

A funcionalidade de acesso de convidado permite que as organizações compartilham [rapidamente os ativos](../using/brand-portal-sharing-folders.md#how-to-share-folders) aprovados com o público-alvo pretendido em escala sem precisar aceitá-los. A versão onwards .4.2 do Brand Portal está equipada para servir vários usuários convidados simultâneos, que são 10% da cota total de usuários por organização. Permitir o acesso a convidados economiza tempo para gerenciar as pontuações de usuários que precisam usar funcionalidades limitadas no Portal da marca.\
As organizações podem ativar (ou desativar) o acesso a convidados na conta do Brand Portal da organização usando **[!UICONTROL a opção Permitir acesso]** de convidado das **[!UICONTROL configurações de acesso]** no painel de ferramentas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Iniciar a sessão de convidados {#begin-guest-session}

Para inserir o Brand Portal anonimamente, selecione **[!UICONTROL Clique aqui]** correspondendo ao Acesso **[!UICONTROL de convidado?]** na tela de boas-vindas do Portal da marca. Os usuários não precisam buscar acesso e esperar que o administrador os autentice para conceder acesso ao uso do Portal da marca.

![](assets/bp-login-screen.png)

## Duração da sessão de convidado {#guest-session-duration}

Uma sessão de usuário de convidados permanece ativa por 2 horas. Isso significa que o estado do [!UICONTROL Lightbox] é preservado até 1 hora da hora de início da sessão e, após 2 horas, a sessão de convidado atual é reiniciada para que o estado do Lightbox seja perdido.\
Por exemplo, um usuário convidado faz logon no Brand Portal a 1500 horas e adiciona ativos ao Lightbox para download em 16:50 horas. Se o usuário não fizer download da [!UICONTROL coleta do Lightbox] (ou dos ativos) antes de 17:00 horas, o [!UICONTROL Lightbox] ficará vazio, pois o usuário terá que reiniciar a sessão no final de 1 hora (ou seja, 1700 horas).

## Sessões de convidados simultâneas permitidas {#concurrent-guest-sessions-allowed}

O número de sessões de convidados simultâneos é limitado a 10% da cota total de usuários por organização. Isso significa que para uma organização com cota de usuário de 200, os usuários convidados máximo de 20 pessoas podem trabalhar ao mesmo tempo. O acesso ao primeiro usuário é negado e pode acessar como convidado somente se a sessão de qualquer um dos 20 usuários convidados terminar.

## Interação de usuário com a Marca do Brand Portal {#guest-user-interaction-with-brand-portal}

### Navegação de UI de convidado

Ao entrar no Portal da marca como convidado, os usuários podem ver todos [os ativos e pastas compartilhados](../using/brand-portal-sharing-folders.md#sharefolders) publicamente ou com usuários convidados exclusivamente. Essa exibição é a exibição apenas do conteúdo, que exibe os ativos em um dos layouts de cartão, lista ou coluna.

![](assets/disabled-folder-hierarchy1.png)

No entanto, os usuários convidados veem a árvore de pastas (começando pela pasta raiz) e as pastas compartilhadas organizadas em suas respectivas pastas principais ao fazer logon no Brand Portal, se os administradores habilitarem [a configuração Ativar hierarquia](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) da pasta.

Essas pastas pai são pastas virtuais e nenhuma ação pode ser executada neles. Você pode reconhecer essas pastas virtuais com um ícone de cadeado.

Nenhuma tarefa de ação é visível ao passar o mouse ou selecioná-las na Exibição [!UICONTROL de cartão], ao contrário das pastas compartilhadas. [!UICONTROL O] botão Visão geral é mostrado na seleção de uma pasta virtual na Exibição [!UICONTROL de coluna] e na Exibição [!UICONTROL de lista].

>[!NOTE]
>
>Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL A opção Configurações] de exibição permite que os usuários convidados ajustem os tamanhos de cartão na [!UICONTROL Exibição] de cartão ou colunas a serem exibidas na [!UICONTROL Exibição de lista].

![](assets/nav-guest-user.png)

A árvore [!UICONTROL Conteúdo] permite mover a hierarquia de ativos.

![](assets/guest-login-ui.png)

O Brand Portal fornece [!UICONTROL a opção Visão geral] aos usuários convidados para visualizar [!UICONTROL Propriedades] de ativos de pastas/ativos selecionados. A opção [!UICONTROL Visão geral] está visível:

* Na barra de ferramentas na parte superior, selecione um ativo/pasta.
* No menu suspenso ao selecionar o Seletor de painéis.

Ao selecionar [!UICONTROL a] opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e a hora da criação de ativos. Enquanto a página de detalhes do ativo selecionando [!UICONTROL a] opção Visão geral permite que os usuários vejam metadados do ativo.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL A]** opção de navegação no painel esquerdo permite navegar de arquivos para coleções e de volta na sessão de convidado para que os usuários possam navegar pelos ativos em arquivos ou coleções.

**[!UICONTROL A opção Filtro]** permite que os usuários convidados filtrem arquivos de ativos e pastas usando a previsão de pesquisa configurada pelo administrador.

### Recursos do usuário convidado

Os usuários convidados podem acessar ativos públicos no Portal da marca e também têm poucas restrições como discutidas.

Os usuários convidados podem:

* acessar todas as pastas públicas e coleções destinadas a todos os usuários do Brand Portal.
* navegar pelos membros, página de detalhes e ter uma visão de ativo total dos membros de todas as pastas públicas e coleções.
* ativos de pesquisa em pastas públicas e coleções.
* adicionar ativos à coleção lightbox. Essas alterações na coleção persistem durante a sessão.
* baixar ativos diretamente ou por meio da coleção lightbox.

Os usuários convidados não podem:

* criar coleções e pesquisas salvas, ou compartilhá-las ainda mais.
* de acesso às configurações de pastas e coleções.
* compartilhar ativos como links.

### Baixar ativos em sessão de convidados

Os usuários convidados podem baixar diretamente ativos compartilhados de maneira pública ou exclusiva com usuários convidados no Brand Portal. Os usuários convidados também podem adicionar ativos ao [!UICONTROL Lightbox] (coleção pública) e baixar a [!UICONTROL coleção do Lightbox] antes de sua sessão expirar.

Para baixar ativos e coleções, use o ícone de download de:

* miniaturas de ação rápida, que aparecem ao passar o mouse sobre o ativo ou a coleção
* a barra de ferramentas na parte superior, que aparece na seleção do ativo ou da coleção

![](assets/download-on-guest.png)

Selecionar **[!UICONTROL Ativar aceleração de download]** na [!UICONTROL caixa de diálogo Download] permite [aprimorar o desempenho do download](../using/accelerated-download.md).

## Sessão de convidados de saída {#exit-guest-session}

Para sair de uma sessão de convidado, use **[!UICONTROL a Sessão]** final das opções disponíveis no cabeçalho. No entanto, se a guia do navegador usada para a sessão de convidado estiver inativa, a sessão expira automaticamente após duas horas de inatividade.

![](assets/end-guest-session.png)

## Monitoramento das atividades do usuário do convidado {#monitoring-guest-user-activities}

Os administradores podem monitorar a interação do usuário convidado com o Portal da marca. Os relatórios gerados no Brand Portal podem fornecer informações importantes sobre as atividades do usuário de convidados. Por exemplo, **[!UICONTROL o]** relatório de Download pode ser usado para rastrear a contagem de ativos baixados pelo usuário convidado. **[!UICONTROL O relatório de logons]** de usuário pode informar quando o usuário convidado faz logon pela última vez no portal e frequência de logons em uma duração especificada.
