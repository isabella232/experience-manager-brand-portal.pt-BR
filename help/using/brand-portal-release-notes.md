---
title: Notas de versão
seo-title: Notas de versão
description: Saiba mais sobre os recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos na versão 2021.06.0 do Adobe Experience Manager Assets Brand Portal.
seo-description: Saiba mais sobre as melhorias, os problemas críticos corrigidos e os problemas conhecidos na versão 2021.06.0 do Adobe Experience Manager Assets Brand Portal.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 54af86b96ef3c3cfe3b1c0db7772d369cac9bb71
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 17%

---

# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos na versão 2021.06.0 do Adobe Experience Manager Assets Brand Portal.

## Informações da versão {#release-information}

| Produto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versão | 2021.06.0 |
| Data | Junho de 2021 |

## Visão geral {#overview}

O Adobe Experience Manager (AEM) Assets Brand Portal ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros e usuários de negócios internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização de ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, visualizem, baixem e exportem ativos em formatos aprovados pela empresa, a qualquer hora e em qualquer lugar.

## Novidades da versão 2021.06.0 {#whats-new-in-2021.06.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.06.0 is an internal release for T2E migration that introduces a new workflow to facilitate orgranization specific entitlement to the Brand Portal users. 

This release includes the following enhancements:

* For a new or migrated T2E organization, the users will have an organization specific entitlement. 


* The new users added to Admin Console will have to **Join Team** to get entitled to the T2E organization. 

* The administrators will get an additional screen to select the T2E organization while navigating from Brand Portal to Admin Console.
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemas críticos corrigidos {#critical-issues-fixed}

O Brand Portal 2021.06.0 é uma versão interna que inclui correções para os seguintes problemas críticos:

* As notificações por email de origem dos ativos não são entregues para algumas organizações.

* Arquivos de vídeo com extensão .mov não estão sendo executados no Brand Portal.

* Na lista suspensa Coleções inteligentes , somente 10 coleções salvas estão visíveis.

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

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* The users will not be able to login to Brand Portal during the migration of their existing organization to T2E. 

  However, the active users will be able to continue to work untill their current session expires or the migration is complete.   
-->

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

Para determinar quais plataformas são certificadas para execução com esta versão do Brand Portal, consulte a coluna **Suporte para interface otimizada para toque** na tabela na seção **Navegadores suportados para criação de interface de usuário** de [Requisitos técnicos](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Links {#links}

* [Página do produto Adobe Experience Manager em adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentação do Assets Brand Portal](https://helpx.adobe.com/br/experience-manager/brand-portal/user-guide.html)

## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente do e precisar de acesso, entre em contato com o gerente de conta do Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Acesso ao produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente do Adobe](https://helpx.adobe.com/contact.html)
