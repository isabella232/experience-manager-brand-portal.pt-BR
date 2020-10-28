---
title: Notas de versão
seo-title: Notas de versão
description: Saiba mais sobre os recursos, melhorias, problemas críticos corrigidos e problemas conhecidos no Portal de marcas dos ativos Adobe Experience Manager 2020.10.0.
seo-description: Saiba mais sobre os aprimoramentos, os problemas críticos corrigidos e os problemas conhecidos no Portal de marcas dos ativos Adobe Experience Manager 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 5cf924ce71433e33506449bbad608d5e57a41b8d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 10%

---


# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, melhorias, problemas críticos corrigidos e problemas conhecidos no Portal de marcas dos Ativos Adobe Experience Manager 2020.10.0.

## Informações da versão {#release-information}

| Produto | Portal de marcas do Adobe Experience Manager Assets |
|---|---|
| Versão | 2020.10.0 |
| Data | Outubro de 2020 |

## Visão geral {#overview}

O Portal de marcas de ativos Adobe Experience Manager (AEM) ajuda você a facilmente adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, pré-visualizações, baixem e exportem ativos em formatos corporativos aprovados, a qualquer momento e em qualquer lugar.

## Novidades da versão 2020.10.0 {#whats-new-in-2020.10.0}

### New Features {#new-features}

Esta versão inclui os seguintes novos recursos:

* A caixa de diálogo **[!UICONTROL Download]** é remodelada em uma visualização de lista com opções adicionais para excluir as representações que não são obrigatórias, aplicar o mesmo conjunto de regras para tipos de ativos semelhantes e baixar as representações de ativos selecionadas. Consulte [as etapas para fazer o download de ativos do Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* A navegação para **[!UICONTROL Arquivos]**, **[!UICONTROL Coleções]** e Links **** compartilhados agora é possível em todas as páginas do Brand Portal em um clique.

* O painel **[!UICONTROL Representações]** na página de detalhes do ativo agora permite que os usuários do Brand Portal selecionem o ativo original e (ou) representações específicas do ativo e os baixem diretamente do painel **[!UICONTROL Representações]** sem precisar abrir a caixa de diálogo **[!UICONTROL Download]** . Consulte [baixar ativos da página](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page)de detalhes do ativo.

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Além das configurações de **[!UICONTROL Download]** existentes, os administradores do Brand Portal também podem [configurar permissões para diferentes grupos de usuários](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) para visualização e (ou) baixar o ativo original e suas representações da página de detalhes do ativo. Essas configurações definirão quem pode acessar e (ou) baixar as representações de ativos.

### Aprimoramentos {#enhancements}

Esta versão inclui os seguintes aprimoramentos:

* O limite de tempo limite da sessão para os usuários convidados foi reduzido de 2 horas para 15 minutos.
* A opção de páginas **[!UICONTROL de]** Visualização adicionais foi removida para PDFs de várias páginas, pois o usuário agora pode visualização as páginas de PDF do Adobe Document Cloud Viewer.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Problemas conhecidos {#known-issues}

Esta versão inclui o seguinte problema conhecido:

* A pesquisa nos Relatórios **[!UICONTROL de]** ativos mostra o processamento na interface do produto sem nenhum resultado de pesquisa.
* Os códigos DM de vídeo não estão visíveis para usuários não administradores na página de detalhes do ativo.
* O alinhamento do tamanho de representações individuais de ativos e do tamanho total de download está distorcido na caixa de diálogo Download.



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

A interface de usuário do Brand Portal está disponível nos seguintes idiomas:

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

Para determinar quais plataformas são certificadas para execução com esta versão do Brand Portal, consulte a coluna **Suporte para interface otimizada para toque na tabela na seção Navegadores** suportados para criação da interface **do usuário dos requisitos** [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)técnicos.

## Links {#links}

* [Página do produto Adobe Experience Manager em adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentação do Portal de marcas de ativos](https://helpx.adobe.com/br/experience-manager/brand-portal/user-guide.html)

## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente e precisar de acesso, entre em contato com seu gerente de contas do Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Acesso ao produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente Adobe](https://helpx.adobe.com/contact.html)
