---
title: Notas de versão
seo-title: Release Notes
description: Saiba mais sobre os recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos na versão 2021.08.0 do Adobe Experience Manager Assets Brand Portal.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2021.08.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 67a745fed6a13cfdb30e26062eecc3c8d1775e36
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 10%

---

# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos na versão 2021.08.0 do Adobe Experience Manager Assets Brand Portal.

## Informações da versão {#release-information}

| Produto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versão | 2021.08.0 |
| Data | Agosto de 2021 |

## Visão geral {#overview}

O Adobe Experience Manager (AEM) Assets Brand Portal ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros e usuários de negócios internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização de ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, visualizem, baixem e exportem ativos em formatos aprovados pela empresa, a qualquer hora e em qualquer lugar.

## Novidades da versão 2021.08.0 {#whats-new-in-2021.08.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->


### Aprimoramentos {#enhancements}

O Brand Portal 2021.08.0 é uma versão interna que introduz perfis de negócios para clientes corporativos e de equipes para fornecer às organizações um melhor controle sobre seus ativos.

Esta versão inclui os seguintes aprimoramentos:

* Os usuários agora têm direito específico à organização nas organizações novas e migradas. Se um usuário tiver direito a várias organizações, ele precisará selecionar a organização no momento do logon.

* Os novos usuários adicionados ao Admin Console devem **Associar-se à equipe** para terem direito à organização.

>[!NOTE]
>
>Os perfis de negócios estão atualmente aplicáveis às novas organizações criadas após 16 de agosto de 2021.
>
>Até que sua organização seja migrada, você pode continuar a usar os tipos de Adobe ID, Enterprise ID ou Federated ID para acessar a organização.

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemas críticos corrigidos {#critical-issues-fixed}

Esta versão inclui correções para os seguintes problemas críticos:

* As notificações por email de origem dos ativos não são entregues para algumas organizações.

* Arquivos de vídeo com extensão `.mov` não estão sendo executados no Brand Portal.

* Na lista suspensa **[!UICONTROL Coleções inteligentes]** , somente dez coleções salvas estão visíveis.

<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->


### Problemas conhecidos {#known-issues}

Esta versão inclui os seguintes problemas conhecidos:

* Os usuários não podem fazer logon no Brand Portal durante a migração de sua organização existente.

   No entanto, os usuários ativos que estão conectados ao Brand Portal podem continuar trabalhando até que a sessão atual expire.

* Ao navegar do Brand Portal para o Admin Console, os administradores podem ver uma tela extra para selecionar a organização.

* Os usuários não podem remover o perfil de esquema de metadados aplicado de uma pasta.


<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Idiomas {#languages}

A interface do usuário do Brand Portal está disponível nos seguintes idiomas:

* Inglês
* Alemão
* Francês
* Espanhol
* Italiano
* Português do Brasil
* Japonês
* Chinês simplificado
* Coreano

## Plataformas certificadas {#certified-platforms}

Para determinar quais plataformas são certificadas para execução com esta versão do Brand Portal, consulte a coluna **Suporte para interface otimizada para toque** na tabela na seção **Navegadores suportados para criação de interface de usuário** de [Requisitos técnicos](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## Links {#links}

* [Página do produto Adobe Experience Manager em adobe.com](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Documentação do Assets Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente do e precisar de acesso, entre em contato com o gerente de conta do Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support](https://helpx.adobe.com/contact.html)
-->
