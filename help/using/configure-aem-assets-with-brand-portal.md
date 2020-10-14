---
title: Configurar o AEM Assets com o Brand Portal
seo-title: Configurar o AEM Assets com o Brand Portal
description: Saiba mais sobre como configurar o AEM Assets com o Brand Portal.
seo-description: Saiba mais sobre como configurar o AEM Assets com o Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 10%

---


# Configurar o AEM Assets com o Brand Portal {#configure-integration}

A configuração dos ativos Adobe Experience Manager como um Cloud Service com o Adobe Experience Manager Assets Brand Portal permite que você publique e distribua ativos com os usuários do Brand Portal. Enquanto isso, a configuração do AEM 6.3 (e superior) com o Brand Portal permite a publicação de ativos, a distribuição de ativos e os recursos de contribuição de ativos para os usuários do Brand Portal.

Os ativos Adobe Experience Manager são configurados com o Portal de marcas por meio do Console do desenvolvedor do Adobe, que obtém um token de Adobe Identity Management Services (IMS) para autorização do locatário do Portal de marcas.

>[!NOTE]
>
>***Para AEM Assets 6.3 e superior***
>
>Anteriormente, o Brand Portal era configurado na interface clássica via Gateway OAuth Herdado, que usa a troca JSON Web token (JWT) para obter um token IMS para autorização.
>
>A configuração por meio do OAuth herdado não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio do Console do desenvolvedor do Adobe.


>[!TIP]
>
>***Somente para clientes existentes***
>
>A configuração antiga do OAuth Gateway continuará funcionando para os clientes existentes.
>
>Caso encontre problemas com a configuração herdada do OAuth Gateway, exclua a configuração existente e crie uma nova configuração por meio do Console do desenvolvedor do Adobe.

As etapas para configurar o AEM Assets com o Brand Portal são diferentes dependendo da versão AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

| **Versão do AEM** | **Nova configuração** | **Configuração de atualização** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |
