---
title: Gerenciar usuários, grupos e funções de usuário
seo-title: Gerenciar usuários, grupos e funções de usuário
description: Os administradores podem usar o Adobe Admin Console para criar usuários e perfis de produto do AEM Assets Brand Portal, além de gerenciar suas funções usando a interface do usuário do Brand Portal. Esse privilégio não está disponível para Visualizadores e editores.
seo-description: Os administradores podem usar o Adobe Admin Console para criar usuários e perfis de produto do AEM Assets Brand Portal, além de gerenciar suas funções usando a interface do usuário do Brand Portal. Esse privilégio não está disponível para Visualizadores e editores.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: referência
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: ba 468 e 80-d 077-4 af 6-b 782-238 fc 557 e 22 b
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Gerenciar usuários, grupos e funções do usuário {#manage-users-groups-and-user-roles}

Os administradores podem usar [!DNL Adobe Admin Console] para criar [!DNL AEM Assets Brand Portal] usuários e perfis de produtos, além de gerenciar suas funções usando a interface do usuário do Brand Portal. Esse privilégio não está disponível para Visualizadores e editores.

No [Console de administração](http://adminconsole.adobe.com/enterprise/overview), você pode exibir todos os produtos associados à sua organização. Um produto pode ser qualquer [!DNL Experience Cloud] solução, como [!DNL Adobe Analytics], [!DNL Adobe Target]ou [!DNL AEM Brand Portal]. Você deve escolher o produto do AEM Brand Portal e criar Perfis de produto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Esses perfis de produto são sincronizados com a interface [!DNL Brand Portal] do usuário a cada 8 horas e visíveis como grupos. [!DNL Brand Portal] Depois [!DNL Brand Portal]de adicionar usuários e criar perfis de produtos e adicionar usuários a esses perfis de produtos, você pode atribuir funções a usuários e grupos.

>[!NOTE]
>
>Para criar grupos em [!DNL Brand Portal], use [!DNL Adobe Admin Console]a página **Produtos** &gt; Perfis **** de produto, em vez de página **Usuário** &gt; Grupos **de usuários**. Perfis de produtos em [!DNL Adobe Admin Console][!DNL Brand Portal]são usados para criar grupos.

## Adicionar um usuário {#add-a-user}

Se você for um administrador de produto, use [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) para criar usuários e atribuí-los a perfis de produtos (*anteriormente conhecidos como configurações de produto*), que são exibidos como grupos. [!DNL Brand Portal] Você pode usar grupos para executar operações em massa, como gerenciamento de funções e compartilhamento de ativos.

>[!NOTE]
Os novos usuários que não têm acesso [!DNL Brand Portal] podem solicitar acesso a partir da tela de logon. [!DNL Brand Portal] Para obter mais informações, consulte [Solicitar acesso a [! DNL Brand Portal]](../using/brand-portal.md#request-access-to-brand-portal). Depois de receber notificações de solicitação de acesso na área de notificação, clique na notificação relevante e clique **em Conceder acesso**. Como alternativa, siga o link no email de solicitação de acesso recebido. Em seguida, para adicionar um usuário a [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview), siga as etapas 4a 7 no procedimento abaixo.

>[!NOTE]
Você pode fazer logon em [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) diretamente ou de [!DNL Brand Portal]. Se você fizer logon diretamente, siga as etapas 4a 7 no procedimento abaixo para adicionar um usuário.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![Logotipo do AEM](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Usuários**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-5.png)

3. Na página **Funções** do usuário, clique na **guia Gerenciamento** e, em seguida, clique **em Iniciar Admin Console**.

   ![Funções do usuário para iniciar o Admin Console](assets/launch_admin_console.png)

4. No Console de administração, execute um dos procedimentos a seguir para criar um novo usuário:

   * Na barra de ferramentas na parte superior, clique **em Visão geral**. Na página **Visão geral** , clique **em Atribuir usuários** do cartão **[!DNL AEM Brand Portal]** de produto.
   ![Visão geral do Console admin.](assets/admin_console_overviewadduser.png)

   * Na barra de ferramentas na parte superior, clique **em Usuários**. Na página **Usuários** , **os usuários** no trilho esquerdo são selecionados por padrão. Clique **em Adicionar usuário**.
   ![Console de administração Adicionar usuários](assets/admin_console_adduseruserpage.png)

5. Na caixa de diálogo Adicionar usuário, digite a ID de e-mail do usuário que deseja adicionar ou selecione o usuário na lista de sugestões que aparecem à medida que você digita.

   ![Adicionar usuário ao Brand Portal](assets/add_user_to_aem_bp.png)

6. Atribua o usuário a pelo menos um perfil de produto (anteriormente chamado de configurações de produto) para que o usuário possa acessar o Portal da marca. Selecione o perfil de produto apropriado no **campo Selecione um perfil para este** campo de produto.
7. Clique em **Salvar**. Um email de boas-vindas é enviado para o usuário que você adicionou. O usuário convidado pode acessar [!DNL Brand Portal] o link no email de boas-vindas e fazer logon usando [!UICONTROL uma Adobe ID]. Para obter mais informações, consulte [Experiência de login pela primeira](../using/brand-portal-onboarding.md)vez.

   >[!NOTE]
   Se um usuário não conseguir fazer logon [!DNL Brand Portal], o Administrador da organização deverá visitar o Adobe [!UICONTROL Admin Console] e verificar se o usuário está presente e foi adicionado a pelo menos um perfil de produto.

   Para obter informações sobre como conceder privilégios administrativos ao usuário, consulte [Fornecer privilégios administrativos aos usuários](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Adicionar um perfil de produto {#add-a-product-profile}

Os perfis de produtos (anteriormente conhecidos como configurações de produto) no [!UICONTROL Console de administração] são usados para criar grupos para [!DNL Brand Portal] que você possa executar operações em massa, como gerenciamento de função e compartilhamento de ativos. [!DNL Brand Portal] **[!DNL Brand Portal]** é o perfil de produto padrão disponível; você pode criar mais perfis de produtos e adicionar usuários aos novos perfis de produtos.

>[!NOTE]
Você pode fazer logon em [[! Console de administração UICONTROL]](http://adminconsole.adobe.com/enterprise/overview) diretamente ou de [!DNL Brand Portal]. Se você fizer logon diretamente no [!UICONTROL Admin Console] , siga as Etapas 4a 7 no procedimento abaixo para adicionar um perfil de produto.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![[!DNL AEM] Logotipo](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Usuários**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-6.png)

3. Na página **Funções** do usuário, clique na **guia Gerenciamento** e, em seguida, clique **em Iniciar Admin Console**.

   ![Iniciar o Admin Console](assets/launch_admin_console.png)

4. Na barra de ferramentas na parte superior, clique **em Produtos**.
5. Na página **Produtos** , **os Perfis de produto** são selecionados por padrão. Clique **em Novo perfil**.

   ![Adicionar novo perfil de produto](assets/admin_console_addproductprofile.png)

6. Na página **Criar um** novo perfil, forneça o nome do perfil, nome de exibição, descrição do perfil e escolha se deseja notificar os usuários por e-mail quando eles forem adicionados ou removidos do perfil.

   ![Criar perfil de produto](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. Clique **em Concluído**. O grupo de configuração de produto, por exemplo, **o grupo Vendas**, é adicionado ao Brand Portal.

   ![Perfis de produtos](assets/admin_console_productprofileadded.png)

## Adicionar usuários a um perfil de produto {#add-users-to-a-product-profile}

Para adicionar usuários a um [!DNL Brand Portal] grupo, adicione-os ao perfil de produto correspondente (anteriormente conhecido como configurações de produto) no [!UICONTROL Console de administração]. Você pode adicionar usuários individualmente ou em massa.

>[!NOTE]
Você pode fazer logon em [[! Admin Console DNL]](http://adminconsole.adobe.com/enterprise/overview) diretamente ou de [!DNL Brand Portal]. Se você fizer logon diretamente no Admin Console, siga as Etapas 4a 7 no procedimento abaixo para adicionar usuários a um perfil de produto.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![[!DNL AEM] Logotipo](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Usuários**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-7.png)

3. Na página **Funções** do usuário, clique na **guia Gerenciamento** e, em seguida, clique **em Iniciar Admin Console**.

   ![Launch [!DNL Admin Console]](assets/launch_admin_console.png)

4. Na barra de ferramentas na parte superior, clique **em Produtos**.
5. Na página **Produtos** , **os Perfis de produto** são selecionados por padrão. Abra o perfil de produto ao qual deseja adicionar um usuário, por exemplo, **o grupo Vendas**.

   ![Perfis de produtos](assets/admin_console_productprofileadded.png)

6. Para adicionar usuários individuais ao perfil de produto, faça o seguinte:

   * Clique **em Adicionar usuário**.
   ![Grupo para mapear o perfil do produto em [!DNL Brand Portal]](assets/admin_console_productprofilesalesgroup.png)

   * Na página **de grupo** Adicionar usuário à vendas, digite a ID de e-mail do usuário que deseja adicionar ou selecione o usuário na lista de sugestões que aparecem à medida que você digita.
   ![Adicionar usuário a um grupo](assets/admin_console_addusertosalesgroup.png)

   * Clique em **Salvar**.



7. Para adicionar usuários em massa ao perfil de produto, faça o seguinte:

   * Escolha reticências(...)****&gt; **Adicionar usuários por CSV**.
   ![Adicionar usuários em massa](assets/admin_console_addbulkusers.png)

   * Na página **Adicionar usuários por CSV** , baixe um modelo CSV ou arraste e solte um arquivo CSV.
   ![Adicionar usuários por csv](assets/admin_console_addbulkuserscsv.png)

   * Clique em **Fazer upload**.
   Se você adicionou usuários ao perfil de produto padrão, ou seja, um [!DNL Brand Portal]email de boas-vindas é enviado para a ID de email dos usuários adicionados. Os usuários convidados podem acessar [!DNL Brand Portal] o link no email de boas-vindas e fazer logon usando [!UICONTROL uma Adobe ID]. Para obter mais informações, consulte [Experiência de login pela primeira](../using/brand-portal-onboarding.md)vez.

   Os usuários adicionados a um perfil personalizado ou novo de produto não recebem notificações por email.

## Fornecer privilégios de administrador aos usuários {#provide-administrator-privileges-to-users}

Você pode fornecer o administrador do sistema ou o privilégio do administrador do produto a um [!DNL Brand Portal] usuário. Não forneça outros direitos administrativos disponíveis no Console [!UICONTROL de administração], como administrador do perfil de produto, administrador do grupo de usuários e administrador de suporte. Para saber mais sobre essas funções, consulte [Funções administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
Você pode fazer logon em [[! Console de administração UICONTROL]](https://adminconsole.adobe.com/enterprise/overview) diretamente ou de [!DNL Brand Portal]. Se você fizer logon diretamente no [!UICONTROL Admin Console] , siga as Etapas 4a 8 no procedimento abaixo para adicionar um usuário a um perfil de produto.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![Aemlogo](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Usuários**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-8.png)

3. Na página **Funções** do usuário, clique na **guia Gerenciamento** e, em seguida, clique **em Iniciar Admin Console**.

   ![Iniciar o Admin Console](assets/launch_admin_console.png)

4. Na barra de ferramentas na parte superior, clique **em Usuários**.
5. Na página **Usuários** , **os usuários** no trilho esquerdo são selecionados por padrão. Clique no nome de usuário do usuário para quem você deseja fornecer privilégios de administrador.

   ![Adicionar usuários no Admin Console](assets/admin_console_adduseruserpage.png)

6. Na página de perfil do usuário, localize a **seção Direitos** administrativos na parte inferior e escolha reticências(...)****&gt; **Editar direitos administrativos**.
   ![Direitos de administrador no Console de administração](assets/admin_console_editadminrights.png)

7. Na página **Editar administrador** , selecione Administrador do sistema ou Administrador de produto.

   ![Editar direitos de administrador no Console de administração](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   [!DNL Brand Portal] suporta somente as funções Administrador do sistema e Administrador do produto.
   [!DNL Adobe] recomenda que você evite usar a função Administrador do sistema, pois concede privilégios de administrador toda a empresa para todos os produtos de uma organização. Por exemplo, um administrador de sistema de uma organização que inclui três produtos da Marketing Cloud tem todo o conjunto de privilégios para todos os três produtos. Somente um Administrador do sistema pode configurar [!DNL AEM] Ativos para que os ativos possam ser publicados em [!DNL AEM] Ativos. [!DNL Brand Portal] Para obter mais informações, consulte [Configurar a integração do AEM Assets com [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).
   Por outro lado, a função Administrador de produto concede privilégios de administrador somente para um produto específico. Se quiser forçar um controle de acesso mais granular dentro [!DNL Brand Portal], use a função Administrador do produto e selecione o produto como **[!DNL AEM Brand Portal]**.

   >[!NOTE]
   [!DNL Brand Portal] não suporta privilégios de administrador do produto (anteriormente conhecidos como privilégios de configuração). Evite atribuir direitos de administrador do perfil de produto a um usuário.

8. Revise a seleção do tipo de administrador e clique **em Salvar**.

   >[!NOTE]
   Para revogar privilégios de administrador para um usuário, faça as alterações apropriadas na página **Editar admin** . e clique **em Salvar**.

## Gerenciar funções de usuário {#manage-user-roles}

Um administrador pode modificar funções para os usuários.[!DNL Brand Portal]

Além da função Administrador [!DNL Brand Portal] , é compatível com as seguintes funções:

* **Visualizador**: Os usuários com essa função podem exibir os arquivos e pastas que um administrador compartilha com eles. Os visualizadores também podem pesquisar e baixar ativos. No entanto, os Visualizadores não podem compartilhar conteúdo (arquivos, pastas, [!UICONTROL coleções]) com outros usuários.
* **Editor**: Os usuários com essa função têm todos os privilégios de um visualizador. Além disso, Editores podem compartilhar conteúdo (pastas, [!UICONTROL coleções], links) com outros usuários.

1. Na [!DNL AEM] barra de ferramentas na parte superior, clique no logotipo da Adobe para acessar as ferramentas administrativas.

   ![Aemlogo](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Usuários**.

   ![Painel Ferramentas administrativas](assets/admin-tools-panel-9.png)

3. Na página **Funções** do usuário, a **guia Usuários** é selecionada por padrão. Para o usuário cuja função você deseja alterar, selecione **Editor** ou **Visualizador** no menu suspenso **Função** .

   ![Modificar funções de usuários](assets/modify_user_role.png)

   Para modificar a função de vários usuários simultaneamente, selecione os usuários e escolha a função apropriada no menu suspenso **Função** .

   >[!NOTE]
   A lista **Função** para usuários do Administrador está desativada. Não é possível selecionar esses usuários para modificar suas funções.

   >[!NOTE]
   A função do usuário também será desabilitada se o usuário for membro do grupo Editor. Para revogar privilégios de edição do usuário, remova o usuário do grupo Editor ou altere a função do grupo inteiro para o Visualizador.

4. Clique em **Salvar**. A função é modificada para o usuário correspondente. Se vários usuários tiverem selecionado, as funções de todos os usuários serão modificadas simultaneamente.

   >[!NOTE]
   As alterações nas permissões do usuário são refletidas na página **Funções** do usuário somente depois que os usuários fazem logon novamente no Brand Portal.

## Gerenciar funções e privilégios do grupo {#manage-group-roles-and-privileges}

Um administrador pode associar privilégios específicos a um [grupo](../using/brand-portal-adding-users.md#main-pars-title-278567577) de usuários no Portal da marca. A guia **Grupos** na página **Funções** do usuário permite que os administradores:

* Atribuir funções a grupos de usuários
* Restrinja grupos de usuários para baixar representações originais de arquivos de imagem (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-bitmap, x-portable-bitmap, x-portable-pixmap, x-xpixmap, x-xon, x-icon, x-icon, x-icon, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) do Portal da marca.

>[!NOTE]
Para os ativos compartilhados como link, a permissão para acessar representações originais de arquivos de imagem será aplicada com base nas permissões do usuário que está compartilhando os ativos.

Para modificar a função e o direito de acessar representações originais para membros do grupo específico, siga estas etapas:

1. Na página **Funções** do usuário, navegue até a **guia Grupos** .
2. Selecione os grupos para os quais você deseja alterar as funções.
3. Selecione a função apropriada na lista suspensa **Função** .

   Para permitir que os membros de um grupo tenham acesso a representações originais de arquivos de imagem (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-bitmap, x-portable-bitmap, x-r@-@ pixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) que eles baixam do portal ou link compartilhado, mantenha a opção **Acesso à original** selecionada para esse grupo. Por padrão, **a opção Acesso à original** é selecionada para todos os usuários. Para impedir que um grupo de usuários acesse representações originais, desmarque a opção correspondente a esse grupo.

   ![Funções de grupo de usuários](assets/access-original-rend.png)

   >[!NOTE]
   Se um usuário for adicionado a vários grupos e um desses grupos tiver restrições, as restrições serão aplicadas a esse usuário.
   Além disso, as restrições para acessar representações originais de arquivos de imagem não se aplicam a administradores, embora sejam membros de grupos restritos.

4. Clique em **Salvar**. A função é modificada para os grupos correspondentes.

   >[!NOTE]
   A associação de usuário a grupo ou a associação de grupo de um usuário é sincronizada [!DNL Brand Portal] a cada 8 horas. As alterações nas funções de usuário ou grupo são eficazes depois que o seguinte serviço de sincronização é executado.
