---
title: Visão geral do Experience Manager Assets Brand Portal
seo-title: Overview of Experience Manager Assets Brand Portal
description: O Experience Manager Assets Brand Portal pode ajudá-lo a adquirir, controlar e distribuir com segurança os ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos.
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: fb2ce4d39fd9e7aa69ba541bd48a6b9cddd3b4c5
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 6%

---

# Visão geral do Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Como profissional de marketing, às vezes é necessário colaborar com parceiros de canal e usuários de negócios internos para criar, gerenciar e fornecer rapidamente conteúdo digital relevante aos clientes. A entrega oportuna de conteúdo relevante em toda a jornada do cliente é essencial para impulsionar maior demanda, conversão, envolvimento e fidelidade do cliente.

No entanto, é um desafio desenvolver soluções que suportem o compartilhamento seguro e eficiente de logotipos de marcas aprovadas, diretrizes, ativos de campanha ou imagens de produtos com equipes internas, parceiros e revendedores estendidos.

**Adobe Experience Manager (AEM) Assets Brand Portal** O se concentra na necessidade do profissional de marketing de colaborar efetivamente com os usuários globais do Brand Portal, fornecendo distribuição de ativos e recursos de contribuição de ativos.

A distribuição de ativos permite que você adquira, controle e distribua com segurança os ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos. Ao passo que a contribuição de ativos permite que os usuários do Brand Portal façam upload de ativos no Brand Portal e os publiquem no Experience Manager Assets, sem precisar acessar o ambiente de criação. O recurso de contribuição é chamado de **Origem de ativos no Brand Portal**. Juntos, ele melhora a experiência geral da Brand Portal em distribuição de ativos e a contribuição dos usuários da Brand Portal (agências/equipes externas), acelera o tempo de entrada no mercado dos ativos e reduz o risco de não conformidade e acesso não autorizado.
Consulte [Origem de ativos no Brand Portal](brand-portal-asset-sourcing.md).

O ambiente do portal baseado em navegador permite que você faça upload, navegue, pesquise, visualize e exporte ativos facilmente em formatos aprovados.

## Configurar o Experience Manager Assets com o Brand Portal {#configure-brand-portal}

A configuração do Adobe Experience Manager Assets com o Brand Portal habilita a publicação de ativos, a distribuição de ativos e os recursos de contribuição de ativos para os usuários do Brand Portal.

>[!NOTE]
>
>A configuração do Experience Manager Assets com Brand Portal é compatível com o Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 e superior.

O Experience Manager Assets as a Cloud Service é configurado automaticamente com o Brand Portal ao ativar o Brand Portal no Cloud Manager. O fluxo de trabalho de ativação cria as configurações necessárias no backend e ativa o Brand Portal na mesma organização IMS da instância as a Cloud Service do Experience Manager Assets.

Enquanto o Experience Manager Assets (no local e managed service) é configurado manualmente com o Brand Portal usando o Adobe Developer Console, que obtém um token Adobe Identity Management Services (IMS) para autorização do locatário do Brand Portal.

Para obter mais informações, consulte [configuração do Experience Manager Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Personalidades do usuário no Brand Portal {#Personas}

O Brand Portal é compatível com as seguintes funções de usuário:

* Usuário convidado
* Visualizador
* Editor
* Administrador

A tabela a seguir lista as tarefas que os usuários nessas funções podem executar:

|  | **Navegar** | **Pesquisar** | **Download** | **Compartilhar pastas** | **Compartilhar uma coleção** | **Compartilhar ativos como um link** | **Acesso às Ferramentas administrativas** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Usuário convidado** | ✓ µ* | ✓* | ✓* | x | x | x | x |
| **Visualizador** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrador** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Os usuários convidados podem navegar, acessar e pesquisar ativos somente em pastas e coleções públicas.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Usuário convidado {#guest-user}

O Experience Manager Assets Brand Portal permite [acesso de convidado](#request-access-to-brand-portal) para o Brand Portal. Um usuário convidado não precisa de credenciais para entrar no portal e tem acesso às pastas e coleções públicas. Como usuário convidado, você pode navegar pelos detalhes do ativo e ter uma exibição completa do ativo dos membros de pastas e coleções públicas. Pesquise, baixe e adicione ativos públicos a [!UICONTROL Lightbox] coleção.

No entanto, a sessão de convidado o impede de criar coleções e pesquisas salvas, e depois compartilha-as. Os usuários em uma sessão de convidado não podem acessar configurações de pasta e coleções e não podem compartilhar ativos como link. Esta é uma lista de tarefas que um usuário convidado pode executar:

* [Procurar e acessar ativos públicos](browse-assets-brand-portal.md)

* [Pesquisar ativos públicos](brand-portal-searching.md)

* [Baixar ativos públicos](brand-portal-download-assets.md)

* [Adicionar ativos ao [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

Para obter mais informações, consulte [acesso de convidado ao Brand Portal](../using/guest-access.md).

### Visualizador {#viewer}

Usuário do Brand Portal definido em [!DNL Admin Console] que tem acesso ao Brand Portal com a função de Visualizador. Um usuário com essa função pode fazer logon no Brand Portal e acessar pastas, coleções e ativos permitidos. O usuário também pode navegar, visualizar, baixar e exportar ativos (representações originais ou específicas), definir configurações de conta e pesquisar ativos. Esta é uma lista de tarefas que um Visualizador pode executar:

* [Procurar ativos](browse-assets-brand-portal.md)

* [Pesquisar por ativos](brand-portal-searching.md)

* [Baixar ativos](brand-portal-download-assets.md)

### Editor {#editor}

Um usuário com a função de Editor pode executar todas as tarefas que um Visualizador pode executar. Além disso, o e o Editor podem exibir os arquivos e pastas compartilhados por um administrador. O usuário com a função de um Editor também pode compartilhar conteúdo (arquivos, pastas, coleções) com outros.

Além das tarefas que um Visualizador pode executar, um Editor pode executar as seguintes tarefas adicionais:

* [Compartilhar pastas](brand-portal-sharing-folders.md)

* [Compartilhar uma coleção](brand-portal-share-collection.md)

* [Compartilhar ativos como um link](brand-portal-link-share.md)

### Administrador {#administrator}

Um administrador inclui um usuário marcado como administrador do sistema ou administrador de produto do Brand Portal no [!UICONTROL Admin Console]. Um administrador pode adicionar e remover administradores e usuários do sistema, definir predefinições, enviar e-mails aos usuários e exibir relatórios de uso do portal e de armazenamento.

>[!NOTE]
>
>No Brand Portal, um usuário marcado com a função de administrador de suporte no [!UICONTROL Admin Console] tem os mesmos privilégios de um administrador do sistema.

Um administrador pode executar todas as tarefas que um Editor pode executar. A seguir estão as tarefas adicionais que um administrador pode executar:

* [Gerenciar usuários, grupos e cargos de usuários](brand-portal-adding-users.md)

* [Personalizar papel de parede, cabeçalhos de página e emails](brand-portal-branding.md)

* [Usar facetas de busca personalizada](brand-portal-search-facets.md)

* [Usar o formulário de esquema de metadados](brand-portal-metadata-schemas.md)

* [Aplicar predefinições de imagens ou representações dinâmicas](brand-portal-image-presets.md)

* [Trabalhar com relatórios](brand-portal-reports.md)

Além das tarefas acima, um Autor no AEM Assets pode executar as seguintes tarefas:

* [Configurar o AEM Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

* [Publicar pastas no Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [Publicar coleções no Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Alias alternativo para o URL do Brand Portal {#tenant-alias-for-portal-url}

A partir do Brand Portal 6.4.3, as organizações podem ter um URL alternativo (alias) para o URL existente de seu locatário do Brand Portal. O URL alias pode ser criado tendo um prefixo alternativo no URL.\
Observe que somente o prefixo do URL do Brand Portal pode ser personalizado, e não o URL inteiro. Por exemplo, uma organização com um domínio existente `geomettrix.brand-portal.adobe.com` pode obter `geomettrixinc.brand-portal.adobe.com` criado mediante solicitação.

No entanto, a instância do autor do AEM pode ser [configurado](../using/configure-aem-assets-with-brand-portal.md) somente com a URL da id do locatário e não com a URL do alias do locatário (alternativo).

>[!NOTE]
>
>Para obter um alias para o nome do locatário no URL do portal existente, as organizações precisam entrar em contato com o Suporte ao cliente com uma nova solicitação de criação de alias de locatário. Essa solicitação é processada verificando primeiro se o alias está disponível e, em seguida, criando o alias.
>
>Para substituir o alias antigo ou excluir o alias antigo, o mesmo processo precisa ser seguido.

## Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Os usuários podem solicitar acesso ao Brand Portal na tela de logon. Essas solicitações são enviadas para administradores do Brand Portal, que concedem acesso aos usuários por meio do Adobe [!UICONTROL Admin Console]. Depois que o acesso for concedido, os usuários receberão um email de notificação.

Para solicitar acesso, faça o seguinte:

1. Na página de logon do Brand Portal, selecione **[!UICONTROL Clique aqui]** correspondente a **[!UICONTROL Precisa de acesso?]**. No entanto, para informar a sessão de convidado, selecione o **[!UICONTROL Clique aqui]** correspondente a **[!UICONTROL Acesso de convidado?]**.

   ![Tela de logon do Brand Portal](assets/bp-login-requestaccess.png)

   A variável [!UICONTROL Solicitar acesso] é aberta.

1. Para solicitar acesso à Brand Portal de uma organização, é necessário ter um [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]ou [!UICONTROL Federated ID].

   No [!UICONTROL Solicitar acesso] faça logon usando sua ID (cenário 1) ou crie uma [!UICONTROL Adobe ID] (cenário 2):

   ![[!UICONTROL Solicitar acesso]](assets/bplogin_request_access_2.png)

   **Cenário 1**

   1. Se você tiver uma [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]ou [!UICONTROL Federated ID], clique em **[!UICONTROL Conectar]**.
A variável [!UICONTROL Fazer logon] é aberta.

   1. Forneça o seu [!UICONTROL Adobe ID] e clique em **[!UICONTROL Fazer logon]**.

      ![Adobe de entrada](assets/bplogin_request_access_3.png)
   Você será redirecionado para a [!UICONTROL Solicitar acesso] página.

   **Cenário 2**

   1. Se você não tiver um [!UICONTROL Adobe ID], para criar um, clique em **[!UICONTROL Obter uma Adobe ID]** do [!UICONTROL Solicitar acesso] página.
A variável [!UICONTROL Fazer logon] é aberta.
   1. Clique em **[!UICONTROL Obter uma Adobe ID]**.
A variável [!UICONTROL Inscrever-se] é aberta.
   1. Insira seu nome e sobrenome, ID de email e senha.
   1. Selecionar **[!UICONTROL Inscrever-se]**.

      ![](assets/bplogin_request_access_5.png)
   Você será redirecionado para a [!UICONTROL Solicitar acesso] página.

1. A próxima página exibe seu nome e a ID de e-mail usada para solicitar acesso. Deixe um comentário para o administrador e clique em **[!UICONTROL Enviar]**.

   ![](assets/bplogin-request-access.png)

## Administradores de produto concedem acesso {#grant-access-to-brand-portal}

Os administradores de produtos do Brand Portal recebem solicitações de acesso na área de notificação do Brand Portal e por meio de emails na caixa de entrada.

![Notificação de acesso solicitado](assets/bplogin_request_access_7.png)

Para conceder acesso, os administradores de produtos precisam clicar na notificação relevante na área de notificação do Brand Portal e, em seguida, clicar em **[!UICONTROL Conceder acesso]**.
Como alternativa, os administradores de produtos podem seguir o link fornecido no email de solicitação de acesso para visitar o Adobe [!UICONTROL Admin Console] e adicione o usuário à configuração de produto relevante.

Você será redirecionado para a [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) página inicial. Usar Adobe [!UICONTROL Admin Console] para criar usuários e atribuí-los a perfis de produtos (conhecidos anteriormente como configurações de produtos), que são exibidos como grupos no Brand Portal. Para obter mais informações sobre como adicionar usuários em [!UICONTROL Admin Console], consulte [Adicionar um usuário](brand-portal-adding-users.md#add-a-user) (siga as Etapas 4 a 7 no procedimento para adicionar um usuário).

## Idiomas do Brand Portal {#brand-portal-language}

Você pode alterar o idioma do Brand Portal de Adobe [!UICONTROL Configurações do Experience Cloud].

![Notificação de acesso solicitado](assets/BPLang.png)

Para alterar o idioma:

1. Selecionar [!UICONTROL Usuário] > [!UICONTROL Editar perfil] no menu superior.

   ![Editar perfil](assets/EditBPProfile.png)

1. Ligado [!UICONTROL Configurações do Experience Cloud] selecione um idioma na lista suspensa [!UICONTROL Idioma] menu suspenso.

## Notificação de manutenção do Brand Portal {#brand-portal-maintenance-notification}

Antes de o Brand Portal ser agendado para manutenção, uma notificação é exibida como um banner após você fazer logon no Brand Portal. Um exemplo de notificação:

![](assets/bp_maintenance_notification.png)

Você pode ignorar esta notificação e continuar usando o Brand Portal. Essa notificação aparece em cada nova sessão.

## Informações sobre versão e sistema {#release-and-system-information}

* [Novidades](whats-new.md)
* [Notas de versão](brand-portal-release-notes.md)
* [Formatos de arquivo não compatíveis](brand-portal-supported-formats.md)

## Recursos relacionados {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [Fóruns sobre AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
