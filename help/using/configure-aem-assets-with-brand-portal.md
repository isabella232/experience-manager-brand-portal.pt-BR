---
title: Configurar o AEM Assets com o Brand Portal
seo-title: Configurar o AEM Assets com o Brand Portal
description: Saiba mais sobre a configuração de AEM Assets com o Brand Portal.
seo-description: Saiba mais sobre a configuração de AEM Assets com o Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---


# Configurar o AEM Assets com o Brand Portal {#configure-integration}

Os ativos Adobe Experience Manager (AEM) são configurados com o Brand Portal por meio do Adobe Developer Console, que obtém um token IMS para autorização do locatário do Brand Portal. O Brand Portal agora é compatível com o serviço em nuvem AEM Assets, AEM Assets 6.3 e posteriores.

A configuração dos AEM Assets poderia atender ao Brand Portal, permitindo que você publique e distribua ativos com os usuários do Brand Portal. Enquanto isso, a configuração do Brand Portal no AEM 6.3 (e superior) permite a publicação de ativos, a distribuição de ativos e os recursos de contribuição de ativos para os usuários do Brand Portal.

>[!NOTE]
>
>***Para AEM Assets 6.3 e superior***
>
>Anteriormente, o Brand Portal estava configurado na interface clássica via Gateway OAuth herdado, que usa a troca de token JWT para obter um Token de acesso IMS para autorização.
>
>A configuração por meio do Legacy OAuth não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio do Adobe Developer Console.


>[!TIP]
>
>***Somente para clientes existentes***
>
>A configuração antiga do OAuth Gateway continuará funcionando para os clientes existentes.
>
>Caso encontre problemas com a configuração herdada do OAuth Gateway, exclua a configuração existente e crie uma nova configuração por meio do Adobe Developer Console.


As etapas para configurar AEM Assets com o Brand Portal são diferentes dependendo da versão do AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

| **Versão do AEM** | **Nova configuração** | **Configuração de atualização** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |


