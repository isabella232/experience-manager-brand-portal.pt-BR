---
title: Administrar configurações de locatários gerais
seo-title: Administrar configurações de locatários gerais
description: Configure a aceleração de download, a criação de coleções inteligentes públicas, a criação de coleções públicas e permita que os usuários administradores excluam ativos em locatários.
seo-description: Configure a aceleração de download, a criação de coleções inteligentes públicas, a criação de coleções públicas e permita que os usuários administradores excluam ativos em locatários.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: 59faef1d9ecdabad95326717548d534229cbff16
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 4%

---


# Administrar configurações de locatários gerais {#administer-general-tenant-configurations}

O Portal de marcas da AEM Assets permite que as organizações configurem os seguintes recursos para locatários específicos:

* Exclusão de ativos por administradores
* Criação de coleções públicas por usuários não administradores
* Criação de coleções inteligentes públicas por usuários não administradores
* Hierarquia pai de pastas compartilhadas visível para usuários não administradores

Essas configurações foram fornecidas como **[!UICONTROL Configurações gerais]** no painel de ferramentas administrativas.

![](assets/general-config.png)

****   AConfiguração para permitir que os administradores excluam ativos do Brand Portal. (O padrão está ativado)

**Configuração**   BC para permitir que usuários não administradores criem coleções públicas. (O padrão está ativado)

**Configuração**   para permitir que usuários não administradores criem coleções inteligentes públicas. (O padrão está ativado)

**Configuração**  DC para exibir a hierarquia de pastas (da raiz) de pastas compartilhadas para usuários não administradores (Editores, Visualizadores, Usuários convidados). (O padrão está desativado)

## Ativar/desativar configurações Gerais {#enable-disable-general-configurations}

Para ativar/desativar cada uma dessas configurações:

1. Faça logon com privilégios de administrador.
1. Selecione o logotipo AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior.
1. No painel de ferramentas administrativas, selecione **[!UICONTROL Geral]** para abrir a página **[!UICONTROL Configurações gerais]**.
1. Use o respectivo switch de alternância para ativar/desativar qualquer uma das configurações Gerais.
1. **[!UICONTROL Salve as alterações.]**
1. Faça logout para permitir que as alterações entrem em vigor.

## Permitir que usuários administradores excluam ativos do Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Permitir que os usuários]** excluam a configuração permite que as organizações permitam (ou restrinjam) que usuários com privilégios de administrador excluam ativos e pastas do Brand Portal.

## Permitir a criação de coleções públicas por não administradores {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Permitir que coleções públicas criações ]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) controlem a configuração se não administradores podem criar coleções públicas no Brand Portal. A configuração é ativada por padrão. Ao desativar as organizações de configuração, é possível evitar que muitas coleções públicas estejam em seu portal para que o espaço do sistema possa ser salvo.

## Permitir a criação de coleções inteligentes públicas por não administradores {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Permitir que coleções inteligentes públicas ]](../using/brand-portal-searching.md#main-pars-header-500620467) criaçãocontrolem a configuração se não administradores podem salvar suas pesquisas como coleções inteligentes e torná-las públicas para esse locatário. A configuração é ativada por padrão. Ao desativar as organizações de configuração, é possível evitar que um grande número de coleções inteligentes públicas sejam criadas por usuários não administradores no Brand Portal da organização.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Ativar hierarquia de pastas {#enable-folder-hierarchy}

[[!UICONTROL Ativar a configuração da ]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) hierarquia de pastas permite que os administradores controlem como os usuários não administradores (Editores, Visualizadores e Usuários convidados) visualizam as pastas compartilhadas depois de fazer logon.
