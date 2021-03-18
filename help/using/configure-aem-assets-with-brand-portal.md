---
title: Configurar o AEM Assets com o Brand Portal
seo-title: Configurar o AEM Assets com o Brand Portal
description: Obtenha informações sobre como configurar o AEM Assets com o Brand Portal.
seo-description: Obtenha informações sobre como configurar o AEM Assets com o Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Administrador
translation-type: tm+mt
source-git-commit: 6b9433bd5a225a2bbaddc09980c9f7b866a75fe8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 23%

---


# Configurar o AEM Assets com o Brand Portal {#configure-integration}

A configuração do Adobe Experience Manager Assets com o Brand Portal permite a publicação de ativos, a distribuição de ativos e os recursos de contribuição de ativos para os usuários do Brand Portal. Ela permite que os usuários do AEM Assets publiquem e distribuam ativos com os usuários do Brand Portal. Os usuários do Brand Portal podem acessar os ativos compartilhados e contribuir carregando novos ativos nas pastas de contribuição de ativos e publicando-os de volta no AEM Assets.

A configuração do AEM Assets com o Brand Portal é compatível com:
* Ativos AEM as a Cloud Service
* AEM Assets (no local e serviço gerenciado) 6.3 e superior

O AEM Assets as a Cloud Service é configurado automaticamente com o Brand Portal ao ativar o Brand Portal no Cloud Manager. O workflow de ativação cria as configurações necessárias no backend e ativa o Brand Portal na mesma organização IMS que a do AEM Assets como uma instância do Cloud Service.

Enquanto isso, o AEM Assets (no local e serviço gerenciado) é configurado manualmente com o Brand Portal usando o Adobe Developer Console, que obtém um token Adobe Identity Management Services (IMS) para autorização do locatário do Brand Portal.

>[!NOTE]
>
>***Para AEM Assets 6.3 e superior***
>
>Anteriormente, o Brand Portal era configurado na interface clássica por meio do Gateway OAuth herdado, que usa a troca JSON Web token (JWT) para obter um token IMS para autorização.
>
>A configuração por meio do Legacy OAuth não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio do Console do desenvolvedor do Adobe.


>[!TIP]
>
>***Somente para clientes existentes (no local e serviço gerenciado)***
>
>A configuração herdada do Gateway OAuth continuará funcionando para os clientes existentes.
>
>Caso encontre problemas com a configuração herdada do Gateway OAuth, exclua a configuração existente e crie uma nova configuração por meio do Console do desenvolvedor do Adobe.

As etapas para configurar o AEM Assets com o Brand Portal são diferentes dependendo da versão do AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

| **Versão do AEM** | **Nova configuração** | **Atualizar configuração** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Ativar Brand Portal](https://docs.adobe.com/content/help/pt-BR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/br/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/br/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/br/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |
