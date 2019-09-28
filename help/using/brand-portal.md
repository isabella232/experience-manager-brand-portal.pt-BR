---
title: Visão geral do AEM Assets Brand Portal
seo-title: Visão geral do AEM Assets Brand Portal
description: O AEM Assets Brand Portal pode ajudá-lo a facilmente adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos.
seo-description: O AEM Assets Brand Portal pode ajudá-lo a facilmente adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: referência
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introdução
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Visão geral do AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Como profissional de marketing, às vezes é necessário colaborar com parceiros de canal e usuários empresariais internos para criar, gerenciar e fornecer rapidamente conteúdo digital relevante aos clientes. A entrega atempada de conteúdo relevante em toda a jornada do cliente é essencial para aumentar a demanda, a conversão, o envolvimento e a fidelidade do cliente.

No entanto, é um desafio desenvolver soluções que suportem o compartilhamento eficiente e seguro de logotipos de marca aprovados, diretrizes, ativos de campanha ou capturas de produtos com equipes internas, parceiros e revendedores estendidos.

**O portal** de marcas dos ativos Adobe Experience Manager (AEM) pode ajudá-lo a adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado.

O ambiente de portal baseado em navegador permite que você carregue, navegue, pesquise, visualize e exporte ativos facilmente em formatos aprovados.

## Personalidades do usuário no Brand Portal {#Personas}

O Brand Portal suporta as seguintes funções de usuário:

* Usuário convidado
* Visualizador
* Editor
* AdministradorA tabela a seguir lista as tarefas que os usuários nessas funções podem executar:

|  | **Navegar** | **Pesquisar** | **Download** | **Compartilhar pastas** | **Compartilhar uma coleção** | **Compartilhar ativos como um link** | **Acesso às Ferramentas administrativas** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Guest user** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizador** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrador** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Os usuários convidados podem navegar, acessar e pesquisar ativos somente em pastas públicas e coleções.

### Guest user {#guest-user}

Qualquer usuário com acesso limitado aos ativos no Brand Portal sem passar pela autenticação é um usuário convidado. A sessão de convidado permite que os usuários acessem pastas públicas e coleções. Como usuário convidado, você pode navegar pelos detalhes do ativo e ter uma visualização completa dos ativos de membros de pastas públicas e coleções. Você pode pesquisar, baixar e adicionar ativos públicos à coleção do [!UICONTROL Lightbox] .

No entanto, a sessão de convidado impede que você crie coleções e pesquisas salvas, além de compartilhá-las ainda mais. Os usuários em uma sessão de convidado não podem acessar as configurações de pastas e coleções e não podem compartilhar ativos como links. Esta é uma lista de tarefas que um usuário convidado pode executar:

[Procurar e acessar ativos públicos](browse-assets-brand-portal.md)

[Search public assets](brand-portal-searching.md)

[Download public assets](brand-portal-download-users.md)

[Add assets to [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizador {#viewer}

A standard user in Brand Portal is typically a user with the role of Viewer. A user with this role can access permitted folders, collections, and assets. The user can also browse, preview, download, and export assets (original or specific renditions), configure account settings, and search for assets. Here is a list of tasks that a Viewer can perform:

[Browse assets](browse-assets-brand-portal.md)

[Search for assets](brand-portal-searching.md)

[Download assets](brand-portal-download-users.md)

### Editor {#editor}

A user with the role of Editor can perform all tasks that a Viewer can perform. In addition, and Editor can view the files and folders that an administrator shares. The user with the role of an Editor can also share content (files, folders, collections) with others.

Apart from the tasks that a Viewer can perform, an Editor can perform the following additional tasks:

[Share folders](brand-portal-sharing-folders.md)

[Compartilhar uma coleção](brand-portal-share-collection.md)

[Share assets as a link](brand-portal-link-share.md)

### Administrador {#administrator}

Um administrador inclui um usuário marcado como administrador do sistema ou como administrador do produto do Portal de marca no Console [!UICONTROL de administração]. Um administrador pode adicionar e remover administradores e usuários do sistema, definir predefinições, enviar emails para usuários e exibir o uso do portal e os relatórios de armazenamento.

Um administrador pode executar todas as tarefas que um Editor pode executar as seguintes tarefas adicionais:

[Gerenciar usuários, grupos e funções de usuário](brand-portal-adding-users.md)

[Personalizar papel de parede, cabeçalhos de página e e-mails](brand-portal-branding.md)

[Usar aspectos de pesquisa personalizados](brand-portal-search-facets.md)

[Usar o formulário de esquema de metadados](brand-portal-metadata-schemas.md)

[Aplicar predefinições de imagens ou representações dinâmicas](brand-portal-image-presets.md)

[Trabalhar com relatórios](brand-portal-reports.md)

Além das tarefas acima, um Autor no AEM Assets pode executar as seguintes tarefas:

[Configurar a integração do AEM Assets com o Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publish folders to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publish collections to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternativo para url do Brand Portal {#tenant-alias-for-portal-url}

A partir do Brand Portal 6.4.3, as organizações podem ter um URL alternativo (alias) para o URL existente do locatário do Brand Portal. O URL do alias pode ser criado com um prefixo alternativo no URL.\
Observe que somente o prefixo do URL do Portal de Marcas pode ser personalizado e não o URL inteiro. Por exemplo, uma organização com o domínio existente **[!UICONTROL geomettrix.brand-portal.adobe.com]** pode obter **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** criado mediante solicitação.

No entanto, a instância do autor de AEM pode ser [configurada](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) somente com o URL de ID do locatário e não com o URL de alias do locatário (alternativo).

>[!NOTE]
>
>Para obter um alias para o nome do locatário no URL do portal existente, as organizações precisam entrar em contato com o suporte da Adobe com uma nova solicitação de criação de alias do locatário. Essa solicitação é processada primeiro verificando se o alias está disponível e depois criando o alias.
>
>Para substituir o alias antigo ou excluí-lo, é necessário seguir o mesmo processo.

## Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Os usuários podem solicitar acesso ao Brand Portal na tela de logon. Essas solicitações são enviadas para administradores do Brand Portal, que concedem acesso aos usuários por meio do Adobe [!UICONTROL Admin Console]. Depois que o acesso é concedido, os usuários recebem um email de notificação.

Para solicitar acesso, faça o seguinte:

1. Na página de logon do Brand Portal, selecione **[!UICONTROL Clique aqui]** correspondente à opção **[!UICONTROL Precisa de acesso?]**. However, to enter the guest session, select the Click here corresponding to Guest Access?.********

   ![Tela de logon do Brand Portal](assets/bp-login-requestaccess.png)

   A página [!UICONTROL Solicitar acesso] é aberta.

1. To request access to an organization’s Brand Portal, you must have a valid Adobe ID, Enterprise ID, or Federated ID.

   In the Request Access page, sign in using your ID (scenario 1) or create an Adobe ID (scenario 2):<br />
   ![[!UICONTROL Solicitar acesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. If you have an Adobe ID, Enterprise ID, or Federated ID, click Sign In.
****
The Sign in page opens.
   1. Provide your Adobe ID credentials and click Sign in.****<br />
   ![Adobe sign in](assets/bplogin_request_access_3.png)

   You are redirected to the Request Access page.<br />
   **Scenario 2**
   1. If you do not have an Adobe ID, to create one, click Get an Adobe ID from the Request Access page.
****
The Sign in page opens.
   1. Click **[!UICONTROL Get an Adobe ID]**.
A página [!UICONTROL Inscrever] é aberta.
   1. Enter your first and last name, email ID, and password.
   1. Selecione **[!UICONTROL Cadastrar-se]**.<br />
   ![](assets/bplogin_request_access_5.png)

   You are redirected to the Request Access page.

1. A próxima página exibe seu nome e ID de email usados para solicitar acesso. Deixe um comentário para o administrador e clique em **[!UICONTROL Enviar]**.<br />

   ![](assets/bplogin-request-access.png)

## Os administradores de produtos concedem acesso {#grant-access-to-brand-portal}

Os administradores de produtos do Brand Portal recebem solicitações de acesso na área de notificação do Brand Portal e por meio de emails em sua caixa de entrada.

![Notificação de acesso solicitada](assets/bplogin_request_access_7.png)

Para conceder acesso, os administradores de produtos precisam clicar na notificação relevante na área de notificação do Brand Portal e clicar em **[!UICONTROL Conceder acesso]**.
Como alternativa, os administradores de produtos podem seguir o link fornecido no email de solicitação de acesso para visitar o Adobe [!UICONTROL Admin Console] e adicionar o usuário à configuração relevante do produto.

Você é redirecionado para a página inicial do [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) . Use o Adobe [!UICONTROL Admin Console] para criar usuários e atribuí-los a perfis de produtos (anteriormente conhecidos como configurações de produtos), que são exibidos como grupos no Brand Portal. Para obter mais informações sobre como adicionar usuários no [!UICONTROL Admin Console], consulte [Adicionar um usuário](brand-portal-adding-users.md#add-a-user) (siga as Etapas 4 a 7 no procedimento para adicionar um usuário).

## Idiomas do Brand Portal {#brand-portal-language}

Você pode alterar o idioma do Brand Portal nas Configurações [!UICONTROL da Adobe]Experience Cloud.

![Notificação de acesso solicitada](assets/BPLang.png)

Para alterar o idioma:

1. Selecione [!UICONTROL Usuário] &gt; [!UICONTROL Editar perfil] no menu superior.<br />
   ![Editar perfil](assets/EditBPProfile.png)

1. Na página Configurações [!UICONTROL da] Experience Cloud, selecione um idioma no menu suspenso [!UICONTROL Idioma] .

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