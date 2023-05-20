---
title: Gerenciar usuários, grupos e cargos de usuários
seo-title: Manage users, groups, and user roles
description: Os administradores podem usar o Adobe Admin Console para criar usuários e perfis de produto do Brand Portal e gerenciar suas funções usando a interface do usuário do Brand Portal. Esse privilégio não está disponível para Visualizadores e Editores.
seo-description: Administrators can use Adobe Admin Console to create Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 0%

---

# Gerenciar usuários, grupos e funções de usuário {#manage-users-groups-and-user-roles}

Os administradores podem usar o Adobe Admin Console para criar usuários e perfis de produto do Experience Manager Assets Brand Portal e gerenciar suas funções usando a interface do usuário do Brand Portal. Esse privilégio não está disponível para Visualizadores e Editores.

Entrada [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), você pode exibir todos os produtos associados à sua organização. Um produto pode ser qualquer solução de Experience Cloud, como Adobe Analytics, Adobe Target ou Experience Manager Assets Brand Portal. Você deve escolher o produto AEM Brand Portal e criar Perfis de produto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Esses perfis de produto são sincronizados com a interface do usuário do Brand Portal a cada 8 horas e visíveis como grupos no Brand Portal. Depois de adicionar usuários e criar perfis de produtos, e adicionar usuários a esses perfis de produtos, você pode atribuir funções a usuários e grupos no Brand Portal.

>[!NOTE]
>
>Para criar grupos no Brand Portal, no Adobe [!UICONTROL Admin Console], use **[!UICONTROL Produtos > Perfis de produto]**, em vez de **[!UICONTROL Página Usuário > Grupos de usuários]**. Perfis de produto no Adobe [!UICONTROL Admin Console] são usados para criar grupos no Brand Portal.

## Adicionar um usuário {#add-a-user}

Se você for um administrador de produto, use o Adobe [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) para criar usuários e atribuí-los a perfis de produtos (*antes conhecidas como configurações de produto*), que são exibidos como grupos no Brand Portal. Você pode usar grupos para executar operações em massa, como gerenciamento de funções e compartilhamento de ativos.

>[!NOTE]
>
>Os novos usuários que não têm acesso ao Brand Portal podem solicitar acesso na tela de logon do Brand Portal. Para obter mais informações, consulte [Solicitar acesso ao Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). Depois de receber notificações de solicitação de acesso na área de notificações, clique na notificação relevante e, em seguida, clique em **[!UICONTROL Conceder acesso]**. Como alternativa, siga o link no email de solicitação de acesso recebido. Em seguida, para adicionar um usuário por meio de [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), siga as Etapas 4 a 7 no procedimento abaixo.

>[!NOTE]
>
>Você pode fazer logon no [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) diretamente ou da Brand Portal. Se você fizer logon diretamente, siga as Etapas 4 a 7 no procedimento abaixo para adicionar um usuário.

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![Logotipo do AEM](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Usuários]**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-5.png)

1. No [!UICONTROL Funções do usuário] clique no link **[!UICONTROL Gerenciamento]** e clique em **[!UICONTROL Admin Console do Launch]**.

   ![Funções de usuário para iniciar o Admin Console](assets/launch_admin_console.png)

1. No Admin Console, siga um destes procedimentos para criar um novo usuário:

   * Na barra de ferramentas na parte superior, clique em **[!UICONTROL Visão geral]**. No [!UICONTROL Visão geral] clique em **[!UICONTROL Atribuir usuários]** no cartão de produto do Brand Portal.

   ![Visão geral do Admin Console](assets/admin_console_overviewadduser.png)

   * Na barra de ferramentas na parte superior, clique em **[!UICONTROL Usuários]**. No [!UICONTROL Usuários] página, [!UICONTROL Usuários] no painel esquerdo é selecionado por padrão. Clique em **[!UICONTROL Adicionar usuário]**.

   ![Admin Console Adicionar usuários](assets/admin_console_adduseruserpage.png)

1. Na caixa de diálogo adicionar usuário, digite a ID de email do usuário que deseja adicionar ou selecione o usuário na lista de sugestões que aparecem ao digitar.

   ![Adicionar usuário ao Brand Portal](assets/add_user_to_aem_bp.png)

1. Atribua o usuário a pelo menos um perfil de produto (conhecido anteriormente como configurações de produto) para que ele possa acessar o Brand Portal. Selecione o perfil de produto apropriado na **[!UICONTROL Selecione um perfil para este produto]** campo.
1. Clique em **[!UICONTROL Salvar]**. Um email de boas-vindas é enviado ao usuário recém-adicionado. O usuário convidado pode clicar no link do email de boas-vindas para acessar o Brand Portal. O usuário pode fazer logon usando a ID de email ([!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]ou [!UICONTROL ID Federada]) configurado no Admin Console. Para obter mais informações, consulte [Experiência de login pela primeira vez](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >Se um usuário não conseguir fazer logon no Brand Portal, o administrador da organização deve visitar o Adobe [!UICONTROL Admin Console] e verifique se o usuário está presente e se foi adicionado a pelo menos um perfil de produto.

   Para obter informações sobre a concessão de privilégios administrativos ao usuário, consulte [Fornecer privilégios de administrador aos usuários](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Adicionar um perfil de produto {#add-a-product-profile}

Perfis de produto (antes conhecidos como configurações de produto) no [!UICONTROL Admin Console] são usados para criar grupos no Brand Portal para que você possa executar operações em massa, como gerenciamento de funções e compartilhamento de ativos no Brand Portal. **Brand Portal** O é o perfil de produto padrão disponível; você pode criar mais perfis de produto e adicionar usuários aos novos perfis de produto.

>[!NOTE]
>
>Você pode fazer logon no [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) diretamente ou da Brand Portal. Se você fizer logon no [!UICONTROL Admin Console] diretamente, siga as Etapas 4 a 7 no procedimento abaixo para adicionar um perfil de produto.

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![Logotipo do AEM](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Usuários]**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-6.png)

1. No [!UICONTROL Funções do usuário] clique no link **[!UICONTROL Gerenciamento]** e clique em **[!UICONTROL Admin Console do Launch]**.

   ![Admin Console do Launch](assets/launch_admin_console.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Produtos]**.
1. No [!UICONTROL Produtos] página, [!UICONTROL Perfis de produto] é selecionada por padrão. Clique em **[!UICONTROL Novo perfil]**.

   ![Adicionar novo perfil de produto](assets/admin_console_addproductprofile.png)

1. No [!UICONTROL Criar um novo perfil] , forneça o nome do perfil, o nome de exibição, a descrição do perfil e escolha se deseja notificar os usuários por email quando eles forem adicionados ou removidos do perfil.

   ![Criar perfil de produto](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Clique em **[!UICONTROL Concluído]**. O grupo de configuração do produto, por exemplo **[!UICONTROL Grupo de vendas]**, é adicionado ao Brand Portal.

   ![Perfis de produto](assets/admin_console_productprofileadded.png)

## Adicionar usuários a um perfil de produto {#add-users-to-a-product-profile}

Para adicionar usuários a um grupo do Brand Portal, adicione-os ao perfil de produto correspondente (conhecido anteriormente como configurações de produto) em [!UICONTROL Admin Console]. Você pode adicionar usuários individualmente ou em massa.

>[!NOTE]
>
>Você pode fazer logon no [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) diretamente ou da Brand Portal. Se você fizer logon diretamente no Admin Console, siga as etapas 4 a 7 do procedimento abaixo para adicionar usuários a um perfil de produto.

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![Logotipo do AEM](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Usuários]**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-7.png)

1. No [!UICONTROL Funções do usuário] clique no link **[!UICONTROL Gerenciamento]** e clique em **[!UICONTROL Admin Console do Launch]**.

   ![Lançamento [!DNL Admin Console]](assets/launch_admin_console.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Produtos]**.
1. No [!UICONTROL Produtos] página, [!UICONTROL Perfis de produto] é selecionada por padrão. Abra o perfil de produto ao qual deseja adicionar um usuário, por exemplo, [!UICONTROL Grupo de vendas].

   ![Perfis de produto](assets/admin_console_productprofileadded.png)

1. Para adicionar usuários individuais ao perfil de produto, faça o seguinte:

   * Clique em **[!UICONTROL Adicionar usuário]**.

   ![Agrupar para mapear o perfil de produto no Brand Portal](assets/admin_console_productprofilesalesgroup.png)

   * No [!UICONTROL Adicionar Usuário ao Grupo de Vendas] digite a ID de email do usuário que deseja adicionar ou selecione-o na lista de sugestões que aparecem ao digitar.

   ![Adicionar usuário a um grupo](assets/admin_console_addusertosalesgroup.png)

   * Clique em **[!UICONTROL Salvar]**.



1. Para adicionar usuários em massa ao perfil do produto, faça o seguinte:

   * Escolher **[!UICONTROL reticências (...) > Adicionar usuários por CSV]**.

   ![Adicionar usuários em massa](assets/admin_console_addbulkusers.png)

   * No **[!UICONTROL Adicionar usuários por CSV]** baixe um modelo CSV ou arraste e solte um arquivo CSV.

   ![Adicionar usuários por csv](assets/admin_console_addbulkuserscsv.png)

   * Clique em **[!UICONTROL Carregar]**.
   Se você adicionou usuários ao perfil de produto padrão, ou seja, Brand Portal, um email de boas-vindas será enviado à ID de email dos usuários adicionados. Os usuários convidados podem acessar o Brand Portal clicando no link do email de boas-vindas e fazendo logon com uma [!UICONTROL Adobe ID]. Para obter mais informações, consulte [Experiência de login pela primeira vez](../using/brand-portal-onboarding.md).

   Os usuários adicionados a um perfil personalizado ou a um novo perfil de produto não recebem notificações por email.

## Fornecer privilégios de administrador aos usuários {#provide-administrator-privileges-to-users}

Você pode fornecer privilégios de administrador do sistema ou de administrador de produto a um usuário do Brand Portal. Não fornecer outros direitos administrativos disponíveis no [!UICONTROL Admin Console], como administrador de perfil de produto, administrador de grupo de usuários e administrador de suporte. Para saber mais sobre essas funções, consulte [Funções administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
>
>Você pode fazer logon no [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) diretamente ou da Brand Portal. Se você fizer logon no [!UICONTROL Admin Console] diretamente, siga as Etapas 4 a 8 no procedimento abaixo para adicionar um usuário a um perfil de produto.

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![AEMLogo](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Usuários]**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-8.png)

1. No [!UICONTROL Funções do usuário] clique no link **[!UICONTROL Gerenciamento]** e clique em **[!UICONTROL Admin Console do Launch]**.

   ![Admin Console do Launch](assets/launch_admin_console.png)

1. Na barra de ferramentas na parte superior, clique em **[!UICONTROL Usuários]**.
1. No [!UICONTROL Usuários] página, [!UICONTROL Usuários] no painel esquerdo é selecionado por padrão. Clique no nome do usuário ao qual você deseja fornecer privilégios de administrador.

   ![Adicionar usuários no Admin Console](assets/admin_console_adduseruserpage.png)

1. Na página de perfil do usuário, localize o **[!UICONTROL Direitos administrativos]** na parte inferior e escolha **[!UICONTROL reticências (...) > Editar direitos administrativos]**.
   ![Direitos de administrador no Admin Console](assets/admin_console_editadminrights.png)

1. No [!UICONTROL Editar administrador] selecione Administrador do sistema ou Administrador do produto.

   ![Editar direitos administrativos no Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >O Brand Portal oferece suporte somente às funções de Administrador do sistema e Administrador do produto.
   >
   >A Adobe recomenda que você evite usar a função de Administrador do sistema, pois ela concede privilégios de administrador em toda a organização para todos os produtos de uma organização. Por exemplo, um administrador de sistema de uma organização que inclui três produtos da Experience Cloud tem todo o conjunto de privilégios para os três produtos. Somente um administrador do sistema pode configurar o Experience Manager Assets para que os ativos possam ser publicados do Experience Manager Assets para o Brand Portal. Para obter mais informações, consulte [Configurar o Experience Manager Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >Por outro lado, a função de Administrador de produto concede privilégios de administrador somente para um produto específico. Se você quiser impor um controle de acesso mais granular no Brand Portal, use a função de Administrador de produto e selecione o produto como Brand Portal.

   >[!NOTE]
   >
   >A Brand Portal não oferece suporte aos privilégios de administrador de perfil de produto (conhecido anteriormente como administrador de configuração). Evite atribuir direitos de administrador de perfil de produto a um usuário.

1. Revise a seleção do tipo de administrador e clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >Para revogar privilégios de administrador para um usuário, faça as alterações apropriadas no **[!UICONTROL Editar administrador]** e clique em **[!UICONTROL Salvar]**.


## Gerenciar funções de usuário {#manage-user-roles}

Um Administrador pode modificar funções para usuários no Brand Portal.

Além da função de Administrador, a Brand Portal oferece suporte às seguintes funções:

* [!UICONTROL Visualizador]: os usuários com essa função podem exibir os arquivos e as pastas que um Administrador compartilha com eles. Os visualizadores também podem pesquisar e baixar ativos. No entanto, os visualizadores não podem compartilhar conteúdo (arquivos, pastas, [!UICONTROL coleções]) com outros usuários.
* [!UICONTROL Editor]: Os usuários com esta atribuição têm todos os privilégios de um Visualizador. Além disso, os editores podem compartilhar conteúdo (pastas, [!UICONTROL coleções], links) com outros usuários.

1. Na barra de ferramentas do AEM na parte superior, clique no logotipo Adobe para acessar as ferramentas administrativas.

   ![AEMLogo](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Usuários]**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-9.png)

1. No [!UICONTROL Funções do usuário] página, a variável [!UICONTROL Usuários] é selecionada por padrão. Para o usuário cuja função você deseja alterar, selecione **[!UICONTROL Editor]** ou **[!UICONTROL Visualizador]** do **[!UICONTROL Função]** menu suspenso.

   ![Modificar funções de usuários](assets/modify_user_role.png)

   Para modificar a atribuição de vários usuários simultaneamente, selecione os usuários e escolha a atribuição apropriada na **[!UICONTROL Função]** menu suspenso.

   >[!NOTE]
   >
   >A variável [!UICONTROL Função] a lista para usuários Administradores está desativada. Não é possível selecionar esses usuários para modificar suas funções.


   >[!NOTE]
   >
   >A função de usuário também estará desativada se o usuário for membro do grupo Editor. Para revogar privilégios de edição do usuário, remova o usuário do grupo Editor ou altere a atribuição do grupo inteiro para Visualizador.


1. Clique em **[!UICONTROL Salvar]**. A função é modificada para o usuário correspondente. Se você selecionou vários usuários, as funções de todos eles serão modificadas simultaneamente.

   >[!NOTE]
   >
   >As alterações nas permissões do usuário se refletem no **[!UICONTROL Funções do usuário]** somente após os usuários fazerem logon novamente no Brand Portal.

## Gerenciar funções e privilégios de grupo {#manage-group-roles-and-privileges}

Um Administrador pode associar privilégios específicos a um [grupo](../using/brand-portal-adding-users.md#main-pars-title-278567577) de usuários no Brand Portal. A variável **[!UICONTROL Grupos]** na guia **[!UICONTROL Funções do usuário]** permite aos administradores:

* Atribuir funções a grupos de usuários
* Restringir grupos de usuários a baixar representações originais de arquivos de imagem (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) da Brand Portal.

>[!NOTE]
>
>Para os ativos compartilhados como o link, a permissão para acessar representações originais de arquivos de imagem será aplicada com base nas permissões do usuário que está compartilhando os ativos.

Para modificar a função e o direito de acessar representações originais de membros de grupos específicos, siga estas etapas:

1. No **[!UICONTROL Funções do usuário]** , navegue até o **[!UICONTROL Grupos]** guia.
1. Selecione os grupos para os quais deseja alterar as funções.
1. Selecione a função apropriada na **[!UICONTROL Função]** lista suspensa.

   Para permitir que os membros de um grupo tenham acesso a representações originais de arquivos de imagem (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) que eles baixam do portal ou link compartilhado, mantenha o **[!UICONTROL Acesso ao original]** selecionada para esse grupo. Por padrão, **[!UICONTROL Acesso ao original]** for selecionada para todos os usuários. Para impedir que um grupo de usuários acesse representações originais, desmarque a opção correspondente a esse grupo.

   ![Funções do grupo de usuários](assets/access-original-rend.png)

   >[!NOTE]
   >
   >Se um usuário for adicionado a vários grupos e se um desses grupos tiver restrições, as restrições serão aplicadas a esse usuário.
   >
   >Além disso, as restrições para acessar representações originais de arquivos de imagem não se aplicam aos administradores, mesmo que sejam membros de grupos restritos.


1. Clique em **[!UICONTROL Salvar]**. A função é modificada para os grupos correspondentes.

   >[!NOTE]
   >
   >A associação de usuário para grupo ou a associação de grupo de um usuário é sincronizada com o Brand Portal a cada 8 horas. As alterações nas funções de usuário ou grupo entram em vigor após a execução do próximo trabalho de sincronização.
