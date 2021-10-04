---
title: Compartilhar pastas
seo-title: Share folders
description: A Brand Portal não é compatível com a assimilação de ativos, portanto, os ativos devem ser publicados na Brand Portal a partir de uma instância do autor do Experience Manager Assets pré-configurada. Os ativos publicados não estão acessíveis a usuários não administradores do Brand Portal, a menos que sejam configurados ao configurar a replicação com a instância do Experience Manager e precisem ser compartilhados com eles.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 1%

---

# Compartilhar pastas no Brand Portal {#share-folders}

Os ativos precisam ser publicados no Brand Portal a partir de uma instância de autor de Experience Manager pré-configurada, pois o Brand Portal não oferece suporte à assimilação de ativos.

## Fluxo de trabalho de compartilhamento de pastas no Brand Portal {#folder-sharing-workflow-in-brand-portal}

A seguir, descreve o fluxo de trabalho de compartilhamento de pastas e o acesso do usuário:

* Por padrão, todas as pastas publicadas do Experience Manager Assets para o Brand Portal estão visíveis apenas para o Administrador do Brand Portal, a menos que sejam marcadas como públicas ao configurar a replicação.
* O Administrador usa o console **[!UICONTROL Propriedades da pasta]** para compartilhar uma pasta com usuários ou grupos seletivos. Somente os usuários ou grupos com os quais a pasta é compartilhada podem visualizá-la depois de fazerem logon no Brand Portal. A pasta não está visível para outros usuários.
* O Administrador também pode optar por tornar uma pasta pública por meio da caixa de seleção **[!UICONTROL Public Folder]** no console **[!UICONTROL Folder Properties]**. Uma pasta pública está visível para todos os usuários.

* Independentemente das funções e privilégios de usuário, quando os usuários fazem logon no Brand Portal, eles verão todas as pastas públicas e as pastas compartilhadas diretamente com eles ou com um grupo ao qual pertencem. As pastas privadas ou as pastas compartilhadas com outros usuários não estão visíveis para todos os usuários.

### Compartilhar pastas com grupos de usuários no Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Os direitos de acesso nos ativos de uma pasta dependem dos direitos de acesso na pasta pai, independentemente das configurações das pastas filhas. Esse comportamento é regido por [ACLs](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) no AEM, pois as pastas secundárias herdam ACLs de suas pastas pai. Por exemplo, se uma pasta A contiver a pasta B que contém a pasta C, um grupo de usuários (ou usuários) com direitos de acesso na pasta A também terá os mesmos direitos de acesso na pasta B e na pasta C. A pasta B sendo a pasta filho de A herda as ACLs e a pasta C sendo a pasta filho de B herda as ACLs.

Da mesma forma, os grupos de usuários (ou usuários) com permissões para acessar somente a pasta B têm as mesmas permissões de acesso na pasta C, mas não na pasta A. Portanto, é recomendável que as organizações organizem seu conteúdo de modo que a maioria dos ativos expostos seja colocada na pasta filho e dos filhos para o acesso à pasta raiz possa ser restringida.

### Publicação de pasta pública {#public-folder-publish}

A menos que a opção **[!UICONTROL Publicação de pasta pública]** esteja selecionada durante a configuração da replicação do Brand Portal, usuários não administradores (como Editores e Visualizadores) não terão acesso a ativos publicados do AEM Assets para o Brand Portal.

![](assets/assetbpreplication.png)

Se a opção **[!UICONTROL Publicar pasta pública]** estiver desativada, os administradores precisarão compartilhar esses ativos especificamente com usuários não administradores usando o recurso de compartilhamento.

>[!NOTE]
>
>A opção para habilitar **[!UICONTROL Publicação de pasta pública]** está disponível AEM 6.3.2.1 em diante.

## Acesso a pastas compartilhadas {#access-to-shared-folders}

A matriz a seguir discute os direitos de acesso e os direitos para compartilhar/cancelar o compartilhamento de ativos para várias funções de usuário:

|  | Acesso a todas as pastas publicadas do AEM Assets para o Brand Portal | Acesso a pastas compartilhadas | Compartilhar/cancelar compartilhamento de direitos de pasta |
|---------------|-----------|-----------|------------|
| Administrador | Sim | Sim | Sim |
| Editor | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Sim, somente para as pastas compartilhadas com elas ou com o grupo ao qual elas pertencem |
| Visualizador | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |
| Usuário convidado | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |

>[!NOTE]
>
>Por padrão, a opção **[!UICONTROL Public Folder Publish]** é desativada ao configurar a replicação do Brand Portal com o AEM Author. Se a opção estiver ativada, as pastas publicadas no Brand Portal estarão acessíveis a todos os usuários (usuários não administradores também) por padrão.

### Acesso de usuário não administrador a pastas compartilhadas {#non-admin-user-access-to-shared-folders}

Usuários não administradores podem acessar somente as pastas compartilhadas com eles no Brand Portal. No entanto, a forma como essas pastas são exibidas no portal quando fazem logon depende das configurações de **[!UICONTROL Ativar hierarquia de pasta]** configuração.

**Se a configuração estiver desativada**

Usuários não administradores veem todas as pastas compartilhadas com eles na página de aterrissagem, ao fazer logon na Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Se a configuração estiver ativada**

Usuários não administradores veem a árvore de pastas (começando pela pasta raiz) e as pastas compartilhadas organizadas em suas respectivas pastas pai, ao fazer logon na Brand Portal.

Essas pastas pai são as pastas virtuais e nenhuma ação pode ser executada nelas. Você pode reconhecer essas pastas virtuais com um ícone de cadeado.

Nenhuma tarefa de ação é visível ao passar o mouse ou selecioná-la em **[!UICONTROL Exibição de cartão]**, ao contrário das pastas compartilhadas. **** O botão Visão geral é exibido ao selecionar uma pasta virtual na  **[!UICONTROL Exibição de]** coluna e Exibição  **[!UICONTROL de lista]**.

>[!NOTE]
>
>Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Compartilhar pastas {#how-to-share-folders}

Para compartilhar uma pasta com usuários no Brand Portal, siga estas etapas:

1. Clique no ícone de sobreposição à esquerda e escolha **[!UICONTROL Navegação]**.

   ![](assets/selectorrail.png)

1. No lado esquerdo, selecione **[!UICONTROL Arquivos]**.

   ![](assets/access_files.png)

1. Na interface do Brand Portal, selecione a pasta que deseja compartilhar.

   ![](assets/share-folders.png)

1. Na barra de ferramentas na parte superior, selecione **[!UICONTROL Compartilhar]**.

   ![](assets/share_icon.png)

   O console [!UICONTROL Propriedades da pasta] é exibido.

   ![](assets/folder_properties.png)

1. No console **[!UICONTROL Propriedades da pasta]**, especifique o título da pasta no campo **[!UICONTROL Título da pasta]** se não quiser que o nome padrão seja exibido aos usuários.
1. Na lista **[!UICONTROL Adicionar Usuário]**, selecione os usuários ou grupos com os quais deseja compartilhar a pasta e clique em **[!UICONTROL Adicionar]**.
Para compartilhar a pasta somente com usuários convidados e nenhum outro usuário, selecione **[!UICONTROL Usuários Anônimos]** na lista suspensa **[!UICONTROL Membros]**.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Para tornar a pasta disponível para todos os usuários, independentemente da associação e função do grupo, torne-a pública selecionando a caixa de seleção **[!UICONTROL Pasta pública]**.

1. Se necessário, clique em **[!UICONTROL Change Thumbnail]** para modificar a imagem em miniatura da pasta.
1. Clique em **[!UICONTROL Salvar]**.

1. Para acessar a pasta compartilhada, faça logon no Brand Portal com as credenciais do usuário com o qual você compartilhou a pasta. Revise a pasta compartilhada na interface.

## Cancelar compartilhamento de pastas {#unshare-the-folders}

Para cancelar o compartilhamento de uma pasta compartilhada anteriormente, siga estas etapas:

1. Na interface do Brand Portal, selecione a pasta que deseja cancelar o compartilhamento.

   ![](assets/share-folders-1.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Compartilhar]**.
1. No console **[!UICONTROL Propriedades da pasta]**, em **[!UICONTROL Membros]**, clique no símbolo **[!UICONTROL x]** ao lado de um usuário para removê-los da lista de usuários com os quais você compartilhou a pasta.

   ![](assets/folder_propertiesunshare.png)

1. Na caixa de mensagem de aviso, clique em **[!UICONTROL Confirm]** para confirmar o cancelamento do compartilhamento.
Clique em **[!UICONTROL Salvar]**.

1. Faça logon no Brand Portal com as credenciais do usuário removido da lista compartilhada. A pasta não está mais disponível na interface do Brand Portal para o usuário.
