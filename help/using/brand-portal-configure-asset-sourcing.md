---
title: Configurar origem de ativos
seo-title: Configurar origem de ativos
description: Obtenha um insight sobre como configurar o recurso de origem de ativos nos ativos AEM.
seo-description: Obtenha um insight sobre como configurar o recurso de origem de ativos nos ativos AEM.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: add4009bd99e5af8ed0c9ffea63647c166b7c75d

---


# Configurar origem de ativos {#configure-asset-sourcing}

Os administradores de AEM podem configurar a Origem **de** ativos a partir da instância do autor de AEM. O administrador habilita a configuração do sinalizador de recurso Origem de ativos na Configuração **do console da Web do** AEM e faz upload da lista de usuários ativos do Portal de marcas nos ativos **** AEM.

>[!NOTE]
>
>Antes de começar com a configuração, verifique se a instância dos ativos AEM está integrada ao Brand Portal. Consulte [Configurar a integração do AEM Assets com o Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).


O vídeo a seguir demonstra como configurar a origem de ativos na sua instância do autor de AEM:

>[!VIDEO](https://video.tv.adobe.com/v/29771?captions=por_br)

## Ativar Seleção de Fornecedor de Ativos {#enable-asset-sourcing}

Os administradores do AEM podem ativar a Origem de ativos na Configuração do console da Web do AEM (também conhecido como Gerenciador de configuração).

**Para ativar a Seleção de fornecedor de ativos:**
1. Faça logon na instância do autor do AEM e abra o URL padrão do Configuration Manager: http:// localhost:4502/system/console/configMgr
1. Pesquise usando a palavra-chave **Origem** de ativos para localizar a Configuração do sinalizador de recursos de origem de **[!UICONTROL ativos]**
1. Clique em Configuração **[!UICONTROL do sinalizador de recurso de origem de]** ativos para abrir a janela de configuração
1. Ativar **[!UICONTROL feature.flag.ative.status da caixa de seleção]**
1. Clique em **[!UICONTROL Salvar]**.

![](assets/enable-asset-sourcing.png)

## Carregar lista de usuários do Brand Portal {#upload-bp-user-list}

Os administradores do AEM podem carregar o arquivo de configuração de usuário (.csv) do Brand Portal que contém a lista de usuários ativos do Brand Portal nos ativos AEM. Uma pasta de contribuição só pode ser compartilhada com os usuários ativos do Brand Portal definidos na lista de usuários. O administrador também pode adicionar novos usuários ao arquivo de configuração e fazer upload da lista de usuários modificada.

O administrador pode adicionar novos usuários no Admin Console do AEM; consulte [Gerenciar usuários](brand-portal-adding-users.md) para obter informações detalhadas. Depois de adicionar usuários no Admin Console, esses usuários podem ser adicionados ao arquivo de configuração do usuário do Brand Portal e, em seguida, recebem permissão para acessar a pasta de contribuição.

**Para carregar a lista de usuários do Brand Portal:**
1. Faça logon na instância do autor de AEMURL padrão: http:// localhost:4502/aem/start.html
1. No painel **Ferramentas** ![](assets/tools.png) , navegue até **[!UICONTROL Ativos &gt; Usuários do Portal de marcas]**
   ![](assets/upload-user-list1.png)
1. A janela Colaboradores de Upload do Portal de Marcas é aberta.
Procure no computador local e carregue o arquivo **de** configuração (.csv) que contém a lista de usuários ativos do Brand Portal.
1. Clique em **[!UICONTROL Salvar]**.
   ![](assets/upload-user-list2.png)


Os administradores podem fornecer acesso a usuários/grupos específicos nesta lista de usuários ao configurar a pasta de contribuição.

Para obter mais informações, consulte [Configurar pasta](brand-portal-contribution-folder.md)de contribuição.
