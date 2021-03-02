---
title: Origem de ativos no Brand Portal
seo-title: Origem de ativos no Brand Portal
description: Obtenha um insight sobre o recurso de seleção de ativos lançado no Portal de marcas do Adobe Experience Manager Assets.
seo-description: Obtenha um insight sobre o recurso de seleção de ativos lançado no Portal de marcas do Adobe Experience Manager Assets.
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
source-git-commit: 5a61c42762e111b824163ce7d054d413a4da56bc
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---


# Visão geral da origem dos ativos {#overview-asset-sourcing-in-bp}

**A** origem dos ativos permite que os usuários do AEM (administradores/usuários não administradores) criem novas pastas com uma propriedade adicional  **de** contribuição de ativos, garantindo que a nova pasta criada seja aberta para o envio de ativos pelos usuários do Brand Portal. Isso aciona automaticamente um workflow que cria duas subpastas adicionais, chamadas **SHARED** e **NEW**, na pasta recém-criada **Contribution**. O administrador do AEM então define o requisito fazendo o upload de um resumo sobre os tipos de ativos que devem ser adicionados à pasta de contribuição, bem como um conjunto de ativos da linha de base, à pasta **SHARED** para garantir que os usuários da BP tenham as informações de referência necessárias. O administrador pode conceder acesso aos usuários ativos do Brand Portal à pasta de contribuição antes de publicar a pasta recém-criada **Contribuição** no Brand Portal. Quando o usuário terminar de adicionar conteúdo na pasta **NEW**, ele poderá publicar a pasta de contribuição de volta no ambiente de autor do AEM. Observe que pode levar alguns minutos para concluir a importação e refletir o conteúdo recém-publicado nos AEM Assets.

Além disso, todas as funcionalidades existentes permanecem inalteradas. Os usuários do Brand Portal podem visualizar, pesquisar e baixar ativos da pasta de contribuição, bem como das outras pastas permitidas. Além disso, os administradores podem compartilhar a pasta de contribuição, modificar propriedades e adicionar ativos às coleções.

## Pré-requisitos {#prerequisites}

* Instância do AEM Assets as a Cloud Service, AEM Assets 6.5.2 ou superior.
* Certifique-se de que a instância do AEM Assets esteja configurada com o Brand Portal. Consulte [Configurar o AEM Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Certifique-se de que o locatário do Brand Portal esteja configurado com uma instância do autor do AEM Assets.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Seleção de ativos do Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Há um problema conhecido no AEM Assets 6.5.4. Os usuários do Brand Portal não podem publicar os ativos da pasta de contribuição no AEM Assets ao atualizar para o Console do desenvolvedor.
>
>O problema é corrigido no AEM 6.5.5. Você pode atualizar a instância do AEM Assets para o service pack mais recente do AEM 6.5.5 e [atualizar suas configurações](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) no Console do desenvolvedor.
>
>Para uma correção imediata no AEM 6.5.4, é recomendável [baixar o hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalar na instância do autor.

## Configurar origem de ativos {#configure-asset-sourcing}

**A origem** do ativo é configurada na instância do autor do AEM Assets. Os administradores podem ativar a configuração do sinalizador de recurso de origem de ativos a partir de **Configuração do Console da Web AEM** e fazer upload da lista de usuários ativos do Brand Portal em **AEM Assets**.

>[!NOTE]
>
>A origem dos ativos é ativada por padrão no AEM Assets as a Cloud Service. O administrador do AEM pode fazer upload diretamente dos usuários ativos do Brand Portal para permitir que eles acessem o recurso de origem dos ativos.

>[!NOTE]
>
>Antes de começar com a configuração, verifique se a instância do AEM Assets está configurada com o Brand Portal. Consulte [Configurar o AEM Assets com o Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

O vídeo a seguir demonstra como configurar a origem dos ativos na instância do autor do AEM Assets:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### Ativar origem de ativos {#enable-asset-sourcing}

Os administradores do AEM podem ativar o sinalizador de recurso de origem de ativos na Configuração do console da Web do AEM (também conhecido como Gerenciador de configuração).

>[!NOTE]
>
>Esta etapa não se aplica aos ativos AEM as a Cloud Service.


**Para ativar a origem dos ativos:**
1. Faça logon na instância do autor do AEM Assets e abra o Configuration Manager.
URL padrão: http:// localhost:4502/system/console/configMgr.
1. Pesquise usando a palavra-chave **Origem de Ativos** para localizar **[!UICONTROL Configuração do Sinalizador de Recursos de Origem de Ativos]**.
1. Clique em **[!UICONTROL Configuração do Sinalizador de Recurso de Origem de Ativos]** para abrir a janela de configuração.
1. Marque a caixa de seleção **[!UICONTROL feature.flag.ative.status]**.
1. Clique em **[!UICONTROL Salvar]**.

![](assets/enable-asset-sourcing.png)

### Fazer upload da lista de usuários do Brand Portal {#upload-bp-user-list}

Os administradores do AEM podem fazer upload do arquivo de configuração de usuário do Brand Portal (.csv) contendo a lista de usuários do Brand Portal ativa no AEM Assets. Uma pasta de contribuição só pode ser compartilhada com os usuários ativos do Brand Portal definidos na lista de usuários. O administrador também pode adicionar novos usuários no arquivo de configuração e fazer upload da lista de usuários modificada.

>[!NOTE]
>
>O formato do arquivo CSV é igual ao compatível com o Admin Console para importação de usuários em massa. Email, nome e sobrenome são obrigatórios.

Os administradores podem adicionar novos usuários no Admin Console do AEM, consulte [Gerenciar usuários](brand-portal-adding-users.md) para obter informações detalhadas. Após adicionar usuários no Admin Console, eles podem ser adicionados ao arquivo de configuração do usuário do Brand Portal e, em seguida, atribuídos permissão para acessar a pasta de contribuição.

**Para fazer upload da lista de usuários do Brand Portal:**
1. Faça logon na instância do AEM Assets.
1. No painel **Ferramentas**, navegue até **[!UICONTROL Ativos]** > **[!UICONTROL Usuários do Brand Portal]**.

1. A janela Colaboradores de upload do Brand Portal é aberta.
Navegue pelo computador local e faça o upload do arquivo **configuração (.csv)** contendo a lista de usuários ativos do Brand Portal.
1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/upload-user-list2.png)


Os administradores podem fornecer acesso a usuários específicos nesta lista de usuários enquanto configuram uma pasta de contribuição. Somente os usuários atribuídos a uma pasta de contribuição terão acesso à pasta de contribuição e publicarão ativos do Brand Portal para o AEM Assets.

## Consulte também:{#reference-articles}

* [Configurar e publicar a pasta de contribuição no Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publicar a pasta de contribuição no AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
