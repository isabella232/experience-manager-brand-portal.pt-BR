---
title: Notas de versão
seo-title: Notas de versão
description: Saiba mais sobre os recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos no Adobe Experience Manager Assets Brand Portal 2021.02.0.
seo-description: Saiba mais sobre as melhorias, os problemas críticos corrigidos e os problemas conhecidos no Adobe Experience Manager Assets Brand Portal 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 10%

---


# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos no Adobe Experience Manager Assets Brand Portal 2021.02.0.

## Informações da versão {#release-information}

| Produto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versão | 2021.02.0 |
| Data | Fevereiro de 2021 |

## Visão geral {#overview}

O Adobe Experience Manager (AEM) Assets Brand Portal ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros externos e usuários comerciais internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização de ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, visualizem, baixem e exportem ativos em formatos corporativos aprovados, a qualquer hora e em qualquer lugar.

## Novidades da versão 2021.02.0 {#whats-new-in-2021.02.0}

### Novos recursos {#new-features}

Esta versão inclui os seguintes novos recursos:

* O AEM Assets as a Cloud Service é configurado automaticamente com o Brand Portal ao ativar o Brand Portal no Cloud Manager.

* O recurso de origem dos ativos agora está disponível no AEM Assets as a Cloud Service. Ela permite que os usuários do Brand Portal façam upload de ativos para as pastas de contribuição permitidas e publiquem a pasta de contribuição do Brand Portal para o AEM Assets como uma instância do Cloud Service.

* Uma configuração adicional de **[!UICONTROL Download de ativo]** foi introduzida nas **[!UICONTROL Configurações de download]**. Ele cria uma pasta separada para cada ativo ao baixar as pastas, as coleções ou o download em massa dos ativos.

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

### Aprimoramentos {#enhancements}

Esta versão inclui os seguintes aprimoramentos:

* Para download de pasta, uma pasta separada é criada para cada ativo usando o link de compartilhamento independentemente das **[!UICONTROL Configurações de download]**.
* O **[!UICONTROL Relatório de uso do Brand Portal]** foi modificado para refletir apenas os usuários ativos do Brand Portal.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemas críticos corrigidos {#critical-issues-fixed}

Esta versão inclui correções para os seguintes problemas críticos:

* Caso apenas os ativos originais sejam baixados, o ativo reflete sua própria extensão e não abre até que a extensão seja alterada manualmente para zip.
* A interface do usuário da pasta de coleção não responde ao clicar na seta de navegação.
* **** O botão Criar está visível na  **** Exibição de coluna, mesmo quando as pastas estão vazias.
* **[!UICONTROL A]** pesquisa Omni falha com uma mensagem de erro 414 (Request-URI Too Long) se o dispatcher for ignorado ao acessar a instância do Brand Portal.
* Uma pasta zip vazia é baixada se o ativo contiver uma vírgula (`,`) no nome do arquivo.
* Os usuários do visualizador têm a opção de adicionar usuários à coleção que criaram.
* Comportamento inconsistente é observado quando um ativo (miniatura ou renderização da Web) é baixado usando o link de compartilhamento.

Consulte [novidades do Brand Portal 2021.02.0](whats-new.md).


### Problemas conhecidos {#known-issues}

Esta versão inclui o seguinte problema conhecido:

* Os usuários não estão recebendo notificações por email dos fluxos de trabalho de publicação da origem dos ativos.

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

Para verificar quais plataformas são certificadas para execução com esta versão do Brand Portal, consulte a coluna **Suporte para interface otimizada para toque** na tabela na seção **Navegadores suportados para criação de interface de usuário** de [Requisitos técnicos](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

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
