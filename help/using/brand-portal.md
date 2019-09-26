---
title: Visão geral do AEM Assets Brand Portal
seo-title: Visão geral do AEM Assets Brand Portal
description: AEM Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
seo-description: AEM Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: referência
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introdução
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# Overview of AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

As a marketer, you sometimes need to collaborate with channel partners and internal business users to quickly create, manage, and deliver relevant digital content to customers. Timely delivery of relevant content across the entire customer journey is critical to driving greater demand, conversion, engagement, and customer loyalty.

However, it is a challenge to develop solutions that support efficient and secure sharing of approved brand logos, guidelines, campaign assets, or product shots with extended internal teams, partners, and resellers.

**Adobe Experience Manager (AEM) Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.** Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado.

The browser-based portal environment enables you to easily upload, browse, search, preview, and export assets in approved formats.

## User personas in Brand Portal {#Personas}

Brand Portal supports the following user roles:

* Usuário convidado
* Visualizador
* Editor
* Administrator

A tabela a seguir lista as tarefas que os usuários nessas funções podem executar:

|  | **Navegar** | **Pesquisar** | **Download** | **Compartilhar pastas** | **Compartilhar uma coleção** | **Share assets as a link** | **Acesso às Ferramentas administrativas** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Usuário convidado** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizador** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrador** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Os usuários convidados podem navegar, acessar e pesquisar ativos somente em pastas públicas e coleções.

### Guest user {#guest-user}

Qualquer usuário com acesso limitado aos ativos no Brand Portal sem passar pela autenticação é um usuário convidado. A sessão de convidado permite que os usuários acessem pastas públicas e coleções. Como usuário convidado, você pode navegar pelos detalhes do ativo e ter uma visualização completa dos ativos de membros de pastas públicas e coleções. Você pode pesquisar, baixar e adicionar ativos públicos à coleção do [!UICONTROL Lightbox] .

No entanto, a sessão de convidado impede que você crie coleções e pesquisas salvas, além de compartilhá-las ainda mais. Os usuários em uma sessão de convidado não podem acessar as configurações de pastas e coleções e não podem compartilhar ativos como links. Esta é uma lista de tarefas que um usuário convidado pode executar:

[Procurar e acessar ativos públicos](browse-assets-brand-portal.md)

[Pesquisar ativos públicos](brand-portal-searching.md)

[Baixar ativos públicos](brand-portal-download-users.md)

[Adicionar ativos a [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizador {#viewer}

Um usuário padrão no Brand Portal normalmente é um usuário com a função de Visualizador. Um usuário com essa função pode acessar pastas, coleções e ativos permitidos. O usuário também pode navegar, visualizar, baixar e exportar ativos (execuções originais ou específicas), definir configurações de conta e procurar ativos. Esta é uma lista de tarefas que um visualizador pode executar:

[Procurar ativos](browse-assets-brand-portal.md)

[Pesquisar ativos](brand-portal-searching.md)

[Baixar ativos](brand-portal-download-users.md)

### Editor {#editor}

Um usuário com a função de Editor pode executar todas as tarefas que um Visualizador pode executar. Além disso, e o Editor pode exibir os arquivos e pastas compartilhados por um administrador. O usuário com a função de um Editor também pode compartilhar conteúdo (arquivos, pastas, coleções) com outras pessoas.

Além das tarefas que um visualizador pode executar, um editor pode executar as seguintes tarefas adicionais:

[Compartilhar pastas](brand-portal-sharing-folders.md)

[Compartilhar uma coleção](brand-portal-share-collection.md)

[Compartilhar ativos como um link](brand-portal-link-share.md)

### Administrator {#administrator}

An administrator includes a user marked as system administrator or Brand Portal product administrator in [!UICONTROL Admin Console]. An administrator can add and remove system administrators and users, define presets, send email to users, and view portal usage and storage reports.

An administrator can perform all tasks that an Editor can perform the following additional tasks:

[Manage users, groups, and user roles](brand-portal-adding-users.md)

[Customize wallpaper, page headers, and emails](brand-portal-branding.md)

[Use custom search facets](brand-portal-search-facets.md)

[Use the metadata schema form](brand-portal-metadata-schemas.md)

[Apply image presets or dynamic renditions](brand-portal-image-presets.md)

[Work with reports](brand-portal-reports.md)

In addition to the above tasks, an Author in AEM Assets can perform the following tasks:

[Configure AEM Assets integration with Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publicar pastas no Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publicar coleções no Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alternate alias for Brand Portal url {#tenant-alias-for-portal-url}

Brand Portal 6.4.3 onwards, organizations can have one alternate (alias) URL for existing URL of their Brand Portal tenant. O URL do alias pode ser criado com um prefixo alternativo no URL.\
Note that only the prefix of the Brand Portal URL can be customized and not the entire URL. Por exemplo, uma organização com o domínio existente **[!UICONTROL geomettrix.brand-portal.adobe.com]** pode obter **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** criado mediante solicitação.

No entanto, a instância do autor de AEM pode ser [configurada](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) somente com o URL de ID do locatário e não com o URL de alias do locatário (alternativo).

>[!NOTE]
>
>Para obter um alias para o nome do locatário no URL do portal existente, as organizações precisam entrar em contato com o suporte da Adobe com uma nova solicitação de criação de alias do locatário. Essa solicitação é processada primeiro verificando se o alias está disponível e depois criando o alias.
>
>Para substituir o alias antigo ou excluí-lo, é necessário seguir o mesmo processo.

## Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Os usuários podem solicitar acesso ao Brand Portal na tela de logon. Essas solicitações são enviadas para administradores do Brand Portal, que concedem acesso aos usuários por meio do Adobe [!UICONTROL Admin Console]. Depois que o acesso é concedido, os usuários recebem um email de notificação.

Para solicitar acesso, faça o seguinte:

1. Na página de logon do Brand Portal, selecione **[!UICONTROL Clique aqui]** correspondente à opção **[!UICONTROL Precisa de acesso?]**. Entretanto, para entrar na sessão de convidado, selecione o **[!UICONTROL Clique aqui]** correspondente ao Acesso **[!UICONTROL de convidado?]**.

   ![Tela de logon do Brand Portal](assets/bp-login-requestaccess.png)

   A página [!UICONTROL Solicitar acesso] é aberta.

2. Para solicitar acesso ao Brand Portal de uma organização, é necessário ter uma [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]ou [!UICONTROL Federated ID]válida.

   Na página [!UICONTROL Solicitar acesso] , faça logon usando sua ID (cenário 1) ou crie uma ID [!UICONTROL da] Adobe (cenário 2):<br />
   ![[!UICONTROL Request access]](assets/bplogin_request_access_2.png)

   **Cenário 1**
   1. Se você tiver uma [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]ou [!UICONTROL Federated ID], clique em **[!UICONTROL Entrar]**.
A página [!UICONTROL Entrar] é aberta.
   2. Forneça suas credenciais [!UICONTROL da Adobe ID] e clique em **[!UICONTROL Fazer logon]**.<br />
   ![Login da Adobe](assets/bplogin_request_access_3.png)

   Você é redirecionado para a página [!UICONTROL Solicitar acesso] .<br />
   **Cenário 2**
   1. Se você não tiver uma [!UICONTROL Adobe ID], para criar uma, clique em **[!UICONTROL Obter uma Adobe ID]** na página [!UICONTROL Solicitar acesso] .
A página [!UICONTROL Entrar] é aberta.
   2. Click **[!UICONTROL Get an Adobe ID]**.
A página [!UICONTROL Inscrever] é aberta.
   3. Digite seu nome e sobrenome, ID de e-mail e senha.
   4. Select Sign up.****<br />
   ![](assets/bplogin_request_access_5.png)

   You are redirected to the Request Access page.

3. The next page displays your name and email ID used to request access. Leave a comment for the administrator, and click Submit.****<br />

   ![](assets/bplogin-request-access.png)

## Product administrators grant access {#grant-access-to-brand-portal}

Brand Portal product administrators receive access requests in their Brand Portal notification area and through emails in their inbox.

![Notificação de acesso solicitada](assets/bplogin_request_access_7.png)

Para conceder acesso, os administradores de produtos precisam clicar na notificação relevante na área de notificação do Brand Portal e clicar em **[!UICONTROL Conceder acesso]**.
Alternatively, product administrators can follow the link provided in the access request email to visit Adobe Admin Console and add the user to the relevant product configuration.

You are redirected to the Adobe [!UICONTROL Admin Console] home page. [](https://adminconsole.adobe.com/enterprise/overview) Use Adobe Admin Console to create users and assign them to product profiles (formerly known as product configurations), which show as groups in Brand Portal.  For more information about adding users in Admin Console, see Add a user (follow Steps 4-7 in the procedure to add a user).[](brand-portal-adding-users.md#add-a-user)

## Brand Portal languages {#brand-portal-language}

You can change Brand Portal language from Adobe Experience Cloud Settings.

![Notificação de acesso solicitada](assets/BPLang.png)

To change the language:

1. Select User &gt; Edit Profile from the top menu.<br />
   ![Editar perfil](assets/EditBPProfile.png)

2. Na página Configurações [!UICONTROL da] Experience Cloud, selecione um idioma no menu suspenso [!UICONTROL Idioma] .

## Notificação de manutenção do Brand Portal {#brand-portal-maintenance-notification}

Antes que o Brand Portal esteja programado para manutenção, uma notificação será exibida como um banner depois que você fizer logon no Brand Portal. Uma notificação de amostra:

![](assets/bp_maintenance_notification.png)

Você pode descartar esta notificação e continuar usando o Brand Portal. Esta notificação é exibida em cada nova sessão.

## Informações sobre a versão e o sistema {#release-and-system-information}

* [Novidades](whats-new.md)
* [Notas de versão](brand-portal-release-notes.md)
* [Formatos de arquivo suportados](brand-portal-supported-formats.md)

## Related resources {#related-resources}

* [Atendimento ao cliente da Adobe](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [Fóruns do AEM](https://www.adobe.com/go/aod_forums_en)