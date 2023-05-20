---
title: Compartilhar pastas
seo-title: Share folders
description: O Brand Portal não é compatível com a assimilação de ativos, portanto, os ativos devem ser publicados no Brand Portal a partir de uma instância pré-configurada do Experience Manager Assets Author. Os ativos publicados não podem ser acessados por usuários não administradores do Brand Portal, a menos que estejam configurados ao configurar a replicação com a instância do Experience Manager e precisem ser compartilhados com eles.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 2%

---

# Compartilhar pastas no Brand Portal {#share-folders}

Os ativos precisam ser publicados no Brand Portal a partir de uma instância pré-configurada do autor do Experience Manager, pois o Brand Portal não é compatível com a assimilação de ativos.

## Fluxo de trabalho de compartilhamento de pastas no Brand Portal {#folder-sharing-workflow-in-brand-portal}

A seguir, é descrito o fluxo de trabalho de compartilhamento de pastas e o acesso do usuário:

* Por padrão, todas as pastas publicadas do Experience Manager Assets para o Brand Portal ficam visíveis somente para o administrador do Brand Portal, a menos que marcadas como públicas durante a configuração da replicação.
* O administrador usa o **[!UICONTROL Propriedades da pasta]** para compartilhar uma pasta com usuários ou grupos seletivos. Somente os usuários ou grupos com os quais a pasta é compartilhada podem ver a pasta depois de fazerem logon no Brand Portal. A pasta não está visível para outros usuários.
* O administrador também pode optar por tornar uma pasta pública por meio da **[!UICONTROL Pasta pública]** caixa de seleção na **[!UICONTROL Propriedades da pasta]** console. Uma pasta pública fica visível para todos os usuários.

* Independentemente das funções e privilégios do usuário, quando os usuários fazem logon no Brand Portal, eles visualizam todas as pastas públicas e as pastas compartilhadas diretamente com eles ou com um grupo ao qual pertencem. As pastas privadas ou compartilhadas com outros usuários não estão visíveis para todos os usuários.

### Compartilhar pastas com grupos de usuários no Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Os direitos de acesso aos ativos de uma pasta dependem dos direitos de acesso em sua pasta principal, independentemente das configurações das pastas secundárias. Esse comportamento é regido pelo [ACLs](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html?lang=pt-BR) no AEM, as pastas secundárias herdam ACLs de suas pastas principais. Por exemplo, se uma pasta A contiver a pasta B, que contém a pasta C, um grupo de usuários (ou usuários) com direitos de acesso à pasta A também terá os mesmos direitos de acesso à pasta B e à pasta C. A pasta B, que é a pasta filho de A, herdará suas ACLs, e a pasta C, que é a pasta filho de B, herdará suas ACLs.

Da mesma forma, os grupos de usuários (ou usuários) que têm permissões para acessar somente a pasta B têm as mesmas permissões de acesso na pasta C, mas não na pasta A. É, portanto, recomendável que as organizações organizem seu conteúdo de modo que a maioria dos ativos expostos seja colocada na pasta filho e que o acesso das crianças à pasta raiz possa ser restrito.

### Publicação de pasta pública {#public-folder-publish}

A menos que a variável **[!UICONTROL Publicar pasta pública]** for selecionada durante a configuração da replicação do Brand Portal, os usuários não administradores (como Editores e Visualizadores) não terão acesso aos ativos publicados do AEM Assets para o Brand Portal.

![](assets/assetbpreplication.png)

Se a variável **[!UICONTROL Publicar pasta pública]** estiver desativada, os administradores precisarão compartilhar esses ativos especificamente com usuários não administradores que usam o recurso de compartilhamento.

>[!NOTE]
>
>A opção de habilitar **[!UICONTROL Publicar pasta pública]** O está disponível no AEM 6.3.2.1 em diante.

## Acesso a pastas compartilhadas {#access-to-shared-folders}

A matriz a seguir discute os direitos de acesso e os direitos de compartilhar/cancelar o compartilhamento de ativos para várias funções de usuário:

|  | Acesso a todas as pastas publicadas do AEM Assets para o Brand Portal | Acesso a pastas compartilhadas | Compartilhar/cancelar compartilhamento de direitos da pasta |
|---------------|-----------|-----------|------------|
| Administrador | Sim | Sim | Sim |
| Editor | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Sim, somente para as pastas compartilhadas com eles ou com o grupo ao qual pertencem |
| Visualizador | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |
| Usuário convidado | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |

>[!NOTE]
>
>Por padrão, a variável **[!UICONTROL Publicar pasta pública]** está desativada ao configurar a replicação do Brand Portal com o AEM Author. Se a opção estiver ativada, as pastas publicadas no Brand Portal serão acessíveis a todos os usuários (usuários não administradores também) por padrão.

### Acesso de usuário não administrador a pastas compartilhadas {#non-admin-user-access-to-shared-folders}

Usuários não administradores podem acessar somente as pastas compartilhadas com eles no Brand Portal. No entanto, a forma como essas pastas são exibidas no portal quando fazem logon depende das configurações de **[!UICONTROL Ativar hierarquia de pastas]** configuração.

**Se a configuração estiver desativada**

Usuários não administradores veem todas as pastas compartilhadas com eles na página de aterrissagem ao fazer logon na Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Se a configuração estiver ativada**

Os usuários não administradores veem a árvore de pastas (começando pela pasta raiz) e as pastas compartilhadas organizadas nas respectivas pastas principais, ao fazer logon na Brand Portal.

Essas pastas principais são as pastas virtuais e nenhuma ação pode ser executada nelas. Você pode reconhecer essas pastas virtuais com um ícone de cadeado.

Nenhuma tarefa de ação estará visível ao passar o mouse sobre elas ou selecioná-las **[!UICONTROL Exibição de cartão]**, ao contrário das pastas compartilhadas. **[!UICONTROL Visão geral]** é exibido ao selecionar uma pasta virtual no **[!UICONTROL Exibição de coluna]** e **[!UICONTROL Exibição de lista]**.

>[!NOTE]
>
>Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Compartilhar pastas {#how-to-share-folders}

Para compartilhar uma pasta com usuários no Brand Portal, siga estas etapas:

1. Clique no ícone de sobreposição à esquerda e escolha **[!UICONTROL Navegação]**.

   ![](assets/selectorrail.png)

1. No sideral à esquerda, selecione **[!UICONTROL Arquivos]**.

   ![](assets/access_files.png)

1. Na interface do Brand Portal, selecione a pasta que deseja compartilhar.

   ![](assets/share-folders.png)

1. Na barra de ferramentas na parte superior, selecione **[!UICONTROL Compartilhar]**.

   ![](assets/share_icon.png)

   A variável [!UICONTROL Propriedades da pasta] é exibido.

   ![](assets/folder_properties.png)

1. No **[!UICONTROL Propriedades da pasta]** console, especifique o título da pasta na caixa **[!UICONTROL Título da pasta]** se não quiser que o nome padrão seja exibido aos usuários.
1. No **[!UICONTROL Adicionar usuário]** selecione os usuários ou grupos com os quais deseja compartilhar a pasta e clique em **[!UICONTROL Adicionar]**.
Para compartilhar a pasta somente com usuários convidados e nenhum outro usuário, selecione **[!UICONTROL Usuários anônimos]** do **[!UICONTROL Membros]** lista suspensa.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Para disponibilizar a pasta para todos os usuários independentemente da associação e da função do grupo, torne-a pública selecionando o **[!UICONTROL Pasta pública]** caixa de seleção

1. Se necessário, clique em **[!UICONTROL Alterar miniatura]** para modificar a imagem em miniatura da pasta.
1. Clique em **[!UICONTROL Salvar]**.

1. Para acessar a pasta compartilhada, faça logon no Brand Portal com as credenciais do usuário com o qual você compartilhou a pasta. Revise a pasta compartilhada na interface.

## Cancelar compartilhamento de pastas {#unshare-the-folders}

Para cancelar o compartilhamento de uma pasta compartilhada anteriormente, siga estas etapas:

1. Na interface do Brand Portal, selecione a pasta que deseja cancelar o compartilhamento.

   ![](assets/share-folders-1.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Compartilhar]**.
1. No **[!UICONTROL Propriedades da pasta]** console, em **[!UICONTROL Membros]**, clique no link **[!UICONTROL x]** símbolo ao lado de um usuário para removê-lo da lista de usuários com os quais você compartilhou a pasta.

   ![](assets/folder_propertiesunshare.png)

1. Na caixa de mensagem de aviso, clique em **[!UICONTROL Confirmar o]** para confirmar o cancelamento de compartilhamento.
Clique em **[!UICONTROL Salvar]**.

1. Faça logon no Brand Portal com as credenciais do usuário que você removeu da lista compartilhada. A pasta não está mais disponível na interface do Brand Portal para o usuário.
