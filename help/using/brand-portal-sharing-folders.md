---
title: Compartilhar pastas
seo-title: Compartilhar pastas
description: O Brand Portal não oferece suporte à ingestão de ativos, portanto, os ativos devem ser publicados no Brand Portal a partir de uma instância pré-configurada do autor de AEM. Os ativos publicados não estão acessíveis a usuários não administradores do Brand Portal, a menos que estejam configurados ao configurar a replicação com a instância do AEM e precisem ser compartilhados com eles.
seo-description: O Brand Portal não oferece suporte à ingestão de ativos, portanto, os ativos devem ser publicados no Brand Portal a partir de uma instância pré-configurada do autor de AEM. Os ativos publicados não estão acessíveis a usuários não administradores do Brand Portal, a menos que estejam configurados ao configurar a replicação com a instância do AEM e precisem ser compartilhados com eles.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: referência
topic-tags: compartilhamento
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Compartilhar pastas no Brand Portal {#share-folders}

Os ativos precisam ser publicados no Brand Portal a partir de uma instância pré-configurada do autor de AEM, já que o Brand Portal não oferece suporte à inclusão de ativos.

## Fluxo de trabalho de compartilhamento de pastas no Brand Portal {#folder-sharing-workflow-in-brand-portal}

A seguir, descreve o fluxo de trabalho de compartilhamento de pastas e o acesso do usuário:

* Por padrão, todas as pastas publicadas do AEM Assets para o Brand Portal estão visíveis somente para o Administrador do Brand Portal, a menos que sejam marcadas como públicas ao configurar a replicação.
* O Administrador usa o console Propriedades [!UICONTROL da] pasta para compartilhar uma pasta com usuários ou grupos seletivos. Somente os usuários ou grupos com os quais a pasta é compartilhada poderão ver a pasta depois que fizerem logon no Brand Portal. The folder is not visible to other users.
* The Administrator can also choose to make a folder public through the Public Folder check box in the Folder Properties console.  A public folder is visible to all the users.

* Irrespective of user roles and privileges, when users log in to Brand Portal, they see all the public folders, and the folders directly shared with them or with a group to which they belong. Private folders, or folders shared with other users, are not visible to all users.

### Share folders with user groups on Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Access rights on assets of a folder are dependant on the access rights on its parent folder, irrespective of the settings of children folders. This behavior is governed by ACLs in AEM, as children folders inherit ACLs from their parent folders. [](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) Por exemplo, se uma pasta A contiver a pasta B que contém a pasta C, um grupo de usuários (ou usuários) com direitos de acesso na pasta A também terão os mesmos direitos de acesso na pasta B e na pasta C. A pasta B sendo a pasta filho de A herda ACLs e a pasta C sendo a pasta filho de B herda ACLs.

Similarly, user groups (or users) having permissions to access only folder B have the same access permissions on folder C but not on folder A. It is, therefore, advised that the organizations arrange their content such that most exposed assets are placed in the children folder and from children to root folder access can be restricted.

### Public folder publish {#public-folder-publish}

Unless the Public Folder Publish option is selected while configuring Brand Portal replication, non-admin users (such as Editors and Viewers) do not have access to assets published from AEM Assets to Brand Portal.

![](assets/assetbpreplication.png)

If the Public Folder Publish option is disabled, administrators need to specifically share these assets with non-admin users using share capability.

>[!NOTE]
>
>The option to enable Public Folder Publish is available in AEM 6.3.2.1 onwards.

## Access to shared folders {#access-to-shared-folders}

The following matrix discusses the access rights and rights to share/ unshare assets for various user roles:

|  | Acesso a todas as pastas publicadas do AEM Assets ao Brand Portal | Access to shared folders | Compartilhar/descompartilhar direitos de pastas |
|---------------|-----------|-----------|------------|
| Administrador | Sim | Sim | Sim |
| Editor | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Sim, somente para as pastas compartilhadas com eles ou com o grupo ao qual pertencem |
| Visualizador | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |
| Usuário convidado | Não* | Sim, somente se compartilhado com eles ou com o grupo ao qual pertencem | Não |

**Por padrão, a opção Publicação[!UICONTROL de pasta]pública está desativada ao configurar a replicação do Brand Portal com o autor de AEM. Se a opção estiver ativada, as pastas publicadas no Brand Portal estarão acessíveis a todos os usuários (usuários não administradores também) por padrão.*

### Acesso de usuário não administrador a pastas compartilhadas {#non-admin-user-access-to-shared-folders}

Usuários não administradores podem acessar somente as pastas compartilhadas com eles no Brand Portal. No entanto, a forma como essas pastas são exibidas no portal quando fazem logon depende das configurações de [!UICONTROL Ativar hierarquia] de pastas.

**Se a configuração estiver desativada**

Os usuários não administradores veem todas as pastas compartilhadas com eles na página de aterrissagem, ao fazer logon no Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Se a configuração estiver ativada**

Os usuários não administradores veem a árvore de pastas (começando pela pasta raiz) e as pastas compartilhadas organizadas em suas respectivas pastas pai, ao fazer logon no Brand Portal.

Essas pastas pai são as pastas virtuais e nenhuma ação pode ser executada nelas. É possível reconhecer essas pastas virtuais com um ícone de cadeado.

Nenhuma tarefa de ação é visível ao passar o mouse ou selecioná-la na Exibição [!UICONTROL de]cartão, ao contrário das pastas compartilhadas. [!UICONTROL Overview button is shown on selecting a virtual folder in Column View and List View.]

>[!NOTE]
>
>Note that the default thumbnail of the virtual folders is the thumbnail image of the first shared folder.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Compartilhar pastas {#how-to-share-folders}

Para compartilhar uma pasta com usuários no Brand Portal, siga estas etapas:

1. Clique no ícone de sobreposição à esquerda e escolha **[!UICONTROL Navegação]**.

   ![](assets/selectorrail.png)

2. Do lado esquerdo, selecione **[!UICONTROL Arquivos]**.

   ![](assets/access_files.png)

3. Na interface do Brand Portal, selecione a pasta que deseja compartilhar.

   ![](assets/share-folders.png)

4. Na barra de ferramentas na parte superior, selecione **[!UICONTROL Compartilhar]**.

   ![](assets/share_icon.png)

   O console Propriedades [!UICONTROL da] pasta é exibido.

   ![](assets/folder_properties.png)

5. No console Propriedades [!UICONTROL da] pasta, especifique o título da pasta no campo Título [!UICONTROL da] pasta se não quiser que o nome padrão seja exibido aos usuários.
6. Na lista [!UICONTROL Adicionar usuário] , selecione os usuários ou grupos com os quais você deseja compartilhar a pasta e clique em **[!UICONTROL Adicionar]**.
Para compartilhar a pasta somente com usuários convidados e nenhum outro usuário, selecione Usuários **** anônimos na lista suspensa [!UICONTROL Membros] .

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Para disponibilizar a pasta para todos os usuários, independentemente da associação e função do grupo, torne-a pública marcando a caixa de seleção Pasta **[!UICONTROL pública]** .

7. Se necessário, clique em **[!UICONTROL Alterar miniatura]** para modificar a imagem em miniatura da pasta.
8. Clique em **[!UICONTROL Salvar]**.
9. Para acessar a pasta compartilhada, faça logon no Brand Portal com as credenciais do usuário com o qual você compartilhou a pasta. Revise a pasta compartilhada na interface.

## Descompartilhar pastas {#unshare-the-folders}

Para cancelar o compartilhamento de uma pasta compartilhada anteriormente, siga estas etapas:

1. Na interface do Brand Portal, selecione a pasta que deseja cancelar o compartilhamento.

   ![](assets/share-folders-1.png)

2. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Compartilhar]**.
3. No console Propriedades [!UICONTROL da] pasta, em [!UICONTROL Membros], clique no símbolo **[!UICONTROL x]** ao lado de um usuário para removê-los da lista de usuários com os quais você compartilhou a pasta.

   ![](assets/folder_propertiesunshare.png)

4. Na caixa de mensagem de aviso, clique em **[!UICONTROL Confirmar]** para confirmar o cancelamento do compartilhamento.
Clique em **[!UICONTROL Salvar]**.

5. Faça logon no Brand Portal com as credenciais do usuário que você removeu da lista compartilhada. A pasta não está mais disponível na interface do Brand Portal para o usuário.
