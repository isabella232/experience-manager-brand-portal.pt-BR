---
title: Administrar configurações de locatários gerais
seo-title: Administrar configurações de locatários gerais
description: Configure a aceleração de download, a criação de [!UICONTROL coleções] públicas inteligentes, a criação de [!UICONTROL coleções] públicas e permita que os usuários administradores excluam ativos em locatários.
seo-description: Configure a aceleração de download, a criação de [!UICONTROL coleções] públicas inteligentes, a criação de [!UICONTROL coleções] públicas e permita que os usuários administradores excluam ativos em locatários.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: ff0c8c23b6c76dc9027b560b9db4af2f4b35313e
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 3%

---


# Administrar configurações de locatários gerais {#administer-general-tenant-configurations}

O Portal de marcas do AEM Assets permite que as organizações configurem os seguintes recursos para locatários específicos:

* Exclusão de ativos por administradores
* Criação de coleções públicas por usuários não administradores
* Criação de coleções inteligentes públicas por usuários não administradores
* Aceleração de download
* Hierarquia pai de pastas compartilhadas visível para usuários não administradores

Essas configurações foram fornecidas como configurações de Configurações **** gerais no painel de ferramentas administrativas.

![](assets/general-configs.png)

**Uma** configuração para permitir que os administradores excluam ativos do Brand Portal. (O padrão está ativado)

**B** Configuração para permitir que usuários não administradores criem coleções públicas. (O padrão está ativado)

**C** Configuration para permitir que usuários não administradores criem coleções inteligentes públicas. (O padrão está ativado)

**D** Configuração para permitir a aceleração de download de ativos baixados do portal e dos links compartilhados. (O padrão está desativado)

**E** Configuração para exibir a hierarquia de pastas (da raiz) de pastas compartilhadas para usuários não administradores (editores, visualizadores, usuários convidados). (O padrão está desativado)

## Ativar/desativar configurações gerais {#enable-disable-general-configurations}

Para ativar/desativar cada uma dessas configurações:

1. Faça logon com privilégios de administrador.
1. Selecione o logotipo do AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior.
1. No painel de ferramentas administrativas, selecione **[!UICONTROL Geral]** para abrir a página Configurações **** gerais.
1. Use o respectivo switch de alternância para ativar/desativar qualquer uma das configurações Gerais.
1. **[!UICONTROL Salve as alterações.]**
1. Faça logout para permitir que as alterações entrem em vigor.

## Permitir que usuários administradores excluam ativos do Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Permitir que os usuários excluam]** a configuração permite que as organizações permitam (ou restrinjam) que usuários com privilégios de administrador excluam ativos e pastas do Brand Portal.

## Permitir a criação de coleções públicas por não administradores {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Permitir que coleções públicas criem]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) controles de configuração se não administradores podem criar coleções públicas no Brand Portal. A configuração é ativada por padrão. Ao desativar as organizações de configuração, é possível evitar que muitas coleções públicas estejam em seu portal para que o espaço do sistema possa ser salvo.

## Permitir a criação de coleções inteligentes públicas por não administradores {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Permitir que coleções inteligentes públicas criem]](../using/brand-portal-searching.md#main-pars-header-500620467) controles de configuração se não administradores podem salvar suas pesquisas como coleções inteligentes e torná-las públicas para esse locatário. A configuração é ativada por padrão. Ao desativar as organizações de configuração, é possível evitar que um grande número de coleções inteligentes públicas sejam criadas por usuários não administradores no Brand Portal da organização.

## Permitir aceleração de download {#allow-download-acceleration}

[[!UICONTROL Permitir a configuração de aceleração]](../using/accelerated-download.md) de download permite que as organizações permitam downloads acelerados de ativos do Brand Portal e links compartilhados, integrando-se ao IBM Aspera Connect que é um aplicativo de instalação sob demanda. O aplicativo usa tecnologia proprietária para remover os custos indiretos de TCP.

## Ativar hierarquia de pastas {#enable-folder-hierarchy}

[[!UICONTROL Ativar a configuração da Hierarquia]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) de pastas permite que os administradores controlem como os usuários não administradores (Editores, Visualizadores e Usuários convidados) visualizam as pastas compartilhadas depois de fazer logon.
