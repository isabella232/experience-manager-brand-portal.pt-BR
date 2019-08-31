---
title: Administrar configurações gerais de locatário
seo-title: Administrar configurações gerais de locatário
description: Configurar aceleração de download, smart smart [! Coleção de UICONTROL], pública [! Coleção de UICONTROL, e permite que usuários administradores excluam ativos em inquilinos.
seo-description: Configurar aceleração de download, smart smart [! Coleção de UICONTROL], pública [! Coleção de UICONTROL, e permite que usuários administradores excluam ativos em inquilinos.
uuid: 3 c 46 cd 7 c-c 38 b -4 bc 7-b 566-93 f 977 bc 8227
contentOwner: mgulati
topic-tags: administration
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Administrar configurações gerais de locatário {#administer-general-tenant-configurations}

O AEM Assets Brand Portal permite que as organizações configurem os seguintes recursos para localidades específicas:

* Exclusão de ativo por administradores
* Criação de coleção pública por usuários não administradores
* Criação de coleção inteligente pública por usuários não administradores
* Aceleração de download
* Hierarquia principal das pastas compartilhadas visíveis para usuários não administradores

Essas configurações foram fornecidas como **[!UICONTROL configurações gerais de configurações]** no painel de ferramentas administrativas.

![](assets/general-configs.png)

**Uma** configuração para permitir que os administradores excluam ativos do Portal da marca. (O padrão está ativado)

**Configuração B** para permitir que usuários não administradores criem coleções públicas. (O padrão está ativado)

**Configuração C** para permitir que usuários não administradores criem coleções inteligentes públicas. (O padrão está ativado)

**Configuração D** para permitir a aceleração de download dos ativos baixados do portal e dos links compartilhados. (O padrão está desativado)

**Configuração** para exibir a hierarquia de pastas (da raiz) das pastas compartilhadas para usuários não administradores (Editores, Visualizadores, Usuários convidados). (O padrão está desativado)

## Ativar/desativar configurações gerais {#enable-disable-general-configurations}

Para ativar/desativar cada uma dessas configurações:

1. Faça logon com privilégios de administrador.
2. Selecione o logotipo do AEM para acessar ferramentas administrativas, na barra de ferramentas na parte superior.
3. No painel de ferramentas administrativas, selecione **[!UICONTROL Geral]** para abrir a **[!UICONTROL página Configurações]** gerais.
4. Use a respectiva mudança de alternância para ativar/desativar qualquer uma das configurações Gerais.
5. **[!UICONTROL Salve as alterações.]**
6. Faça logout para que as alterações tenham efeito.

## Permitir que usuários administradores excluam ativos do Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Permita que os usuários possam permitir]** que a configuração permita (ou restringir) usuários com privilégios de administrador para excluir ativos e pastas do Portal da marca.

## Permitir a criação de coleções públicas por usuários que não sejam administradores {#allow-public-collections-creation-by-non-admins}

[[! A configuração Habilitar coleções públicas permite](../using/brand-portal-share-collection.md#main-pars-text-1915052376) que os usuários não administradores criem coleções públicas no Brand Portal. A configuração é habilitada por padrão. Desativar as organizações de configuração pode impedir a presença de várias coleções públicas em seu portal para que o espaço do sistema possa ser salvo.

## Permitir a criação de coleções inteligentes públicas por usuários que não sejam administradores {#allow-public-smart-collections-creation-by-non-admins}

[[! A configuração Habilitar coleções inteligentes de coleções permite](../using/brand-portal-searching.md#main-pars-header-500620467) que os usuários não administradores salvem suas pesquisas como coleções inteligentes e tornem-as públicas para o locatário. A configuração é habilitada por padrão. Desativar as organizações de configuração pode evitar ter um grande número de coleções inteligentes públicas criadas por usuários não administradores no Portal da marca da organização.

## Permitir aceleração de download {#allow-download-acceleration}

[[! A configuração Permitir download do UICONTROL permite](../using/accelerated-download.md) que as organizações permitem downloads acelerados de ativos do Brand Portal e links compartilhados, através da integração com a IBM Aspera Connect que é um aplicativo de demanda de instalação. O aplicativo usa tecnologia proprietária para remover sobreposições TCP.

## Ativar hierarquia de pastas {#enable-folder-hierarchy}

[[! A configuração Habilitar a hierarquia de pastas permite](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) que os administradores controlem como os usuários não administradores (Editores, Visualizadores e Usuários convidados) veem as pastas compartilhadas após fazer logon.
