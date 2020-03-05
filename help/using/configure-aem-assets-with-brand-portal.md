---
title: Configurar ativos AEM com o Portal de marcas
seo-title: Configurar ativos AEM com o Portal de marcas
description: Saiba mais sobre como configurar os ativos AEM com o Portal da marca.
seo-description: Saiba mais sobre como configurar os ativos AEM com o Portal da marca.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: eba4ee138d4f594c4c446a3cc8941f04fd46902c

---


# Configurar ativos AEM com o Portal de marcas {#configure-integration}

Os ativos Adobe Experience Manager (AEM) são configurados com o Brand Portal por meio da E/S da Adobe, que obtém um token IMS para autorização do locatário do Brand Portal. A configuração permite a publicação de ativos, distribuição de ativos e recursos de contribuição de ativos para os usuários do Brand Portal.

>[!NOTE]
>
>Anteriormente, o Brand Portal estava configurado na interface clássica via Gateway OAuth herdado, que usa a troca de token JWT para obter um token de Acesso IMS para autorização.
>
>A configuração por meio do Legacy OAuth não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio da E/S da Adobe.
>
>Se você for um usuário do Brand Portal com configuração no gateway OAuth herdado, é recomendável excluir as configurações existentes e criar uma nova configuração em E/S da Adobe.
>
>No entanto, a configuração existente continuará a funcionar se você não modificar as configurações.

As etapas para configurar os ativos AEM com o Brand Portal são diferentes dependendo da versão do AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

| **Versão do AEM** | **Nova configuração** | **Configuração de atualização** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
