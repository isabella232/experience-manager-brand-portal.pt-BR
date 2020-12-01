---
title: Seleção de recursos no Brand Portal
seo-title: Seleção de recursos no Brand Portal
description: Saiba mais sobre o recurso de origem de ativos lançado no Portal de Marcas dos Ativos Adobe Experience Manager.
seo-description: Saiba mais sobre o recurso de origem de ativos lançado no Portal de Marcas dos Ativos Adobe Experience Manager.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: ativos
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 9c937603cf325919cb49d3418b06266fa1b93cf1
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# Visão geral da Origem de ativos {#overview-asset-sourcing-in-bp}

**A** Origem de ativos permite que os usuários AEM (administradores/não administradores) criem novas pastas com uma propriedade  **de** contribuição de ativos adicional, garantindo que a nova pasta criada seja aberta para o envio de ativos pelos usuários do Brand Portal. Isso aciona automaticamente um fluxo de trabalho que cria duas subpastas adicionais, chamadas **SHARED** e **NEW**, na pasta **Contribution** recém-criada. O administrador do AEM define o requisito fazendo upload de um resumo sobre os tipos de ativos que devem ser adicionados à pasta de contribuição, bem como de um conjunto de ativos de linha de base, à pasta **SHARED** para garantir que os usuários do BP tenham as informações de referência de que precisam. O administrador pode conceder aos usuários ativos do Brand Portal acesso à pasta de contribuição antes de publicar a pasta recém-criada **Contribution** no Brand Portal. Quando o usuário terminar de adicionar conteúdo na pasta **NEW**, poderá publicar a pasta de contribuição de volta no ambiente do autor AEM. Observe que pode levar alguns minutos para concluir a importação e refletir o conteúdo recém-publicado no AEM Assets.

Além disso, toda a funcionalidade existente permanece inalterada. Os usuários do Brand Portal podem visualização, pesquisar e baixar ativos da pasta de contribuição, bem como de outras pastas permitidas. E os administradores podem compartilhar ainda mais a pasta de contribuição, modificar as propriedades e adicionar ativos às coleções.

## Pré-requisitos {#prerequisites}

* AEM 6.5.2 ou superior.
* Certifique-se de que sua instância do AEM Assets esteja configurada com o Brand Portal. Consulte, [Configurar o AEM Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Certifique-se de que seu locatário do Brand Portal esteja configurado com uma instância do autor da AEM Assets.

>[!NOTE]
>
>A Origem de ativos não é suportada no AEM Assets como um Cloud Service.


>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Seleção de recursos do Portal de marcas](assets/asset-sourcing.png)


>[!NOTE]
>
>Há um problema conhecido no AEM 6.5.4. Os usuários do Brand Portal não podem publicar os ativos da pasta de contribuição na AEM Assets ao atualizar para o Adobe Developer Console.
>
>O problema foi corrigido no AEM 6.5.5. Você pode atualizar sua instância do AEM Assets para o service pack mais recente AEM 6.5.5 e [atualizar suas configurações](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) no Adobe Developer Console.
>
>Para uma correção imediata no AEM 6.5.4, é recomendável [baixar o hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalar na instância do autor.


## Consulte também:{#reference-articles}

**Para administradores**

* [Configurar origem de ativos em AEM](brand-portal-configure-asset-sourcing.md)
* [Carregar lista de usuários do Brand Portal](brand-portal-configure-asset-sourcing.md)
* [Configurar pasta de contribuição](brand-portal-contribution-folder.md)
* [Carregar ativos da linha de base para a pasta de contribuição](brand-portal-upload-baseline-assets.md)
* [Publicar pasta de contribuição no Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Para usuários do Brand Portal**

* [Baixar os requisitos de ativos](brand-portal-download-asset-requirements.md)
* [Carregar novos ativos para a pasta de contribuição](brand-portal-upload-assets-to-contribution-folder.md)
* [Publicar pasta de contribuição no AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
