---
title: Novidades do AEM Assets Brand Portal
seo-title: Novidades do AEM Assets Brand Portal
description: Dê uma olhada nos novos recursos e melhorias da versão 2021.02.0.
seo-description: Dê uma olhada nos novos recursos e melhorias da versão 2021.02.0.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: 979545105694eca65652d6c8e6ad5b9fdd9eea86
workflow-type: tm+mt
source-wordcount: '6069'
ht-degree: 3%

---


# Novidades do AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

O Adobe Experience Manager (AEM) Assets Brand Portal ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros externos e usuários comerciais internos em todos os dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização de ativos e reduz o risco de não conformidade e acesso não autorizado. O Adobe está trabalhando para melhorar a experiência geral do Brand Portal. Veja a seguir os novos recursos e aprimoramentos.

## O que mudou em 2021.02.0 {#what-changed-in-feb-2021}

O Brand Portal 2021.02.0 é uma versão aprimorada que inclui o fluxo de trabalho de automação do Brand Portal no AEM Assets as a Cloud Service, facilita o recurso de origem de ativos no AEM Assets as a Cloud Service, melhorias na experiência de download de ativos e inclui correções críticas. Também permite que os administradores configurem o comportamento padrão de download de pastas, coleções e download em massa de ativos no nível do locatário. O **[!UICONTROL Relatório de uso do Brand Portal]** também foi modificado para refletir os usuários ativos do Brand Portal. Consulte as [Notas de versão do Brand Portal](brand-portal-release-notes.md) mais recentes.

### Automação do Brand Portal no AEM Assets as a Cloud Service {#bp-automation-on-cloud-service}

O AEM Assets as a Cloud Service é configurado automaticamente com o Brand Portal ao ativar o Brand Portal no Cloud Manager. Um usuário do Cloud Manager aciona o fluxo de trabalho de ativação que cria as configurações necessárias no backend e ativa o Brand Portal na mesma organização IMS que a do AEM Assets como uma instância do Cloud Service.

Anteriormente, o AEM Assets as a Cloud Service era configurado manualmente com o Brand Portal usando o Adobe Developer Console, que obtém um token Adobe Identity Management Services (IMS) para autorização do locatário do Brand Portal.

Consulte [ativar Brand Portal no AEM Assets como um Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=en).

### Origem de ativos no AEM Assets como Cloud Service {#asset-sourcing-on-cloud-service}

O recurso de origem dos ativos agora está disponível no AEM Assets as a Cloud Service. O recurso é ativado por padrão para todos os usuários do serviço de nuvem. Os usuários permitidos do Brand Portal podem contribuir com o fornecimento de ativos carregando novos ativos nas pastas de contribuição e publicando a pasta de contribuição do Brand Portal para o AEM Assets como uma instância do Cloud Service. Os administradores podem revisar e aprovar a contribuição dos usuários do Brand Portal para distribuí-los ainda mais para outros usuários do Brand Portal.

Anteriormente, a origem dos ativos só estava disponível no AEM Assets (no local e no serviço gerenciado).

Consulte [Origem de ativos no Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/asset-sourcing-in-brand-portal/brand-portal-asset-sourcing.html?lang=en).

### Download de ativo {#asset-download-setting}

Além das **[!UICONTROL Configurações de Download]** existentes, os administradores do Brand Portal agora podem configurar a configuração **[!UICONTROL Download de Ativos]**. Essa configuração permite que os administradores controlem o comportamento padrão de download de pastas, coleções e download em massa de ativos (mais de 20 ativos) no nível do locatário.

<!--
Earlier, all the asset renditions were directly downloaded in a zip folder in case of folder, collection, and bulk download of assets. As the **[!UICONTROL Download]** dialog is skipped for folders or collections, there was no mechanism to control the downloading behaviour of the assets. Due to this, the users were finding it difficut to search for a particular asset rendition from a folder containing huge bunch of downloaded renditions. 
-->

Anteriormente, todas as representações de ativos eram baixadas diretamente em uma pasta zip. A caixa de diálogo **[!UICONTROL Download]** foi ignorada para pastas e coleções, e não havia método para controlar o comportamento de download dos ativos, dificultando a pesquisa de uma representação específica de um grande número de downloads.

**[!UICONTROL A configuração]** Download de ativos agora oferece uma opção para criar uma pasta separada para cada ativo ao baixar as pastas, as coleções ou o download em massa dos ativos.

Se a configuração **[!UICONTROL Download de ativos]** estiver desativada, as pastas ou coleções serão baixadas em uma pasta zip contendo todas as representações de ativos na mesma pasta, exceto para baixar os ativos usando o link de compartilhamento.


Faça logon no locatário do Brand Portal como administrador e navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Download]**. Os administradores podem ativar a configuração **[!UICONTROL Download de ativo]** para criar uma pasta separada para cada ativo ao baixar pastas, coleções e download em massa de ativos.

![](assets/download-settings-new.png)

Consulte [baixar ativos do Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/download/brand-portal-download-assets.html?lang=en).
<!--
### Download using Share link {#download-using-share-link}

The default behavior of downloading the assets using share link is now independent of the **[!UICONTROL Download Settings]**. A separate folder is created for each asset while downloading the assets using share link. 
-->

### Relatório de uso {#usage-report}

O **[!UICONTROL Relatório de uso do Brand Portal]** foi modificado para refletir apenas os usuários ativos do portal da marca. Os usuários do portal da marca que não estão atribuídos a nenhum perfil de produto no Admin Console são considerados usuários inativos e não são refletidos no **[!UICONTROL Relatório de uso]**.

Anteriormente, os usuários ativos e inativos eram mostrados no Relatório de uso.

![](assets/usage-report.png)

## O que mudou em 2020.10.0 {#what-changed-in-oct-2020}

O Brand Portal 2020.10.0 é uma versão de aprimoramento que tem como foco simplificar a experiência de download de ativos e inclui correções críticas. O aprimoramento inclui fluxo de trabalho novo e aprimorado para download de ativos, opções adicionais para excluir representações, download direto do painel **[!UICONTROL Representações]**, configuração para permitir direitos de acesso e download para um grupo específico de usuários e navegação fácil para os arquivos, coleções e links compartilhados de todas as páginas do Brand Portal. Consulte as [Notas de versão do Brand Portal](brand-portal-release-notes.md) mais recentes.


### Experiência de download simplificada {#download-dialog}

Anteriormente, a caixa de diálogo **[!UICONTROL Download]** aparecia com várias opções, como criar uma pasta separada para cada ativo, ativo de email, selecionar ativo original, representações personalizadas, representações dinâmicas, excluir representações do sistema e ativar a aceleração de download, que eram ambíguas para usuários não técnicos ou novos, especialmente quando vários ativos ou pastas eram selecionados para download. Além disso, o usuário não pôde ver todas as representações de ativos ou excluir uma representação personalizada ou dinâmica específica.

A nova caixa de diálogo **[!UICONTROL Download]** generaliza o processo de seleção e filtragem de ativos, o que torna mais fácil para os usuários do Brand Portal tomarem decisões eficazes ao baixar as representações de ativos. Ele lista todos os ativos selecionados e suas representações, dependendo da configuração [**[!UICONTROL Download]**](brand-portal-download-assets.md) e das configurações **[!UICONTROL Download]**.

>[!NOTE]
>
>Todos os usuários agora terão **[!UICONTROL Fast Download]** ativado por padrão e requer [IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) instalado na extensão de seu navegador antes de baixar os ativos do Brand Portal.

<!--
If any of the **[!UICONTROL Custom Rendition]** or **[!UICONTROL System Rendition]** is enabled in the [**[!UICONTROL Download]**](brand-portal-download-assets.md) configuration and **[!UICONTROL Download]** settings are enabled for the group users, the new **[!UICONTROL Download]** dialog appears with all the renditions of the selected assets or folders containing assets in a list view. 
-->

Na caixa de diálogo **[!UICONTROL Download]**, os usuários podem:

* Exibir todas as representações disponíveis de qualquer ativo na lista de download.
* Exclua representações dos ativos que não são necessárias para download.
* Aplique o mesmo conjunto de representações a todos os tipos de ativos semelhantes em um clique.
* Aplique um conjunto diferente de representações para diferentes tipos de ativos.
* Criar uma pasta separada para cada ativo.
* Baixe os ativos selecionados e suas representações.

O fluxo de trabalho de download permanece constante para ativos autônomos, vários ativos, pastas contendo ativos, ativos licenciados ou não e baixando ativos usando o link de compartilhamento. Consulte [etapas para baixar ativos do Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

![caixa de diálogo de download](assets/download-dialog-box.png)

### Navegação rápida {#quick-navigation}

Anteriormente, a opção para exibir **[!UICONTROL Arquivos]**, **[!UICONTROL Coleções]** e **[!UICONTROL Links compartilhados]** ficavam ocultos e exigiam vários cliques sempre que o usuário desejava alternar para outra exibição.

No Brand Portal 2020.10.0, os usuários podem navegar para **[!UICONTROL Arquivos]**, **[!UICONTROL Coleções]** e **[!UICONTROL Links compartilhados]** de todas as páginas do Brand Portal com um clique usando os links de navegação rápida.

![navegação em coleção](assets/collection-navigation.png)

### Painel de representação aprimorado {#rendition-panel}

Anteriormente, os usuários só podiam exibir o ativo original e suas representações no painel **[!UICONTROL Representações]** se qualquer uma das **[!UICONTROL Representação personalizada]** ou **[!UICONTROL Representação do sistema]** estivesse ativada na configuração **[!UICONTROL Download]**. Além disso, os usuários precisavam baixar todas as representações de ativos, pois não havia filtro para excluir representações personalizadas ou dinâmicas específicas que não eram necessárias.

<!--
Earlier, if any of the custom or system renditions was enabled in the **[!UICONTROL Download]** settings, an additional **[!UICONTROL Download]** dialog appeared on clicking the **[!UICONTROL Download]** button wherein the user had to manually select the set of renditions (original asset, custom renditions, dynamic renditions) to download.
There was no filter to exclude specific custom or dynamic renditions which were not required for download.
-->

No Brand Portal 2020.10.0, os usuários podem excluir representações específicas e [baixar diretamente as representações selecionadas do painel Representações](brand-portal-download-assets.md#download-assets-from-asset-details-page) na página Detalhes do ativo sem precisar abrir a caixa de diálogo **[!UICONTROL Download]**.


<!-- 
In Brand Portal 2020.10.0, direct download and exclude renditions features are introduced in the **[!UICONTROL Renditions]** panel on the asset details page. All the renditions (original asset, custom renditions, dynamic renditions) under the rendition panel are now associated with a check box and are enabled by default. 

The user can clear the check boxes to exclude the renditions which are not required for download. And can click on the **[!UICONTROL Download]** button in the **[!UICONTROL Renditions]** panel to directly download the selected set of renditions in a zip folder without having to open the **[!UICONTROL Download]** dialog.
-->

![painel representações](assets/renditions-panel.png)


### Definir configurações de download {#download-permissions}

Além das configurações existentes **[!UICONTROL Download]**, os administradores do Brand Portal também podem definir configurações para diferentes grupos de usuários para visualizar e (ou) baixar o ativo original e suas representações na página de detalhes do ativo.

Faça logon no locatário do Brand Portal como administrador e navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Usuários]**.

Na página **[!UICONTROL Funções de usuário]**, navegue até a guia **[!UICONTROL Grupos]** para definir as configurações de exibição e (ou) download para os grupos de usuários.

Anteriormente, as configurações estavam disponíveis apenas para impedir que os usuários do grupo baixassem o ativo original.

A guia **[!UICONTROL Groups]** na página **[!UICONTROL User Roles]** permite que os administradores definam as configurações de visualização e download:

* Se as configurações **[!UICONTROL Baixar Original]** e **[!UICONTROL Baixar Representações]** estiverem ativadas, os usuários do grupo selecionado poderão exibir e baixar os ativos originais e suas representações.
* Se ambas as configurações estiverem desativadas, os usuários só poderão visualizar os ativos originais. As representações de ativos não estão visíveis para os usuários na página de detalhes do ativo.
* Se apenas a configuração **[!UICONTROL Baixar original]** estiver ativada, os usuários poderão exibir e baixar apenas os ativos originais da página de detalhes do ativo.
* Se apenas a configuração **[!UICONTROL Download de representações]** estiver ativada, os usuários poderão exibir o ativo original, mas não poderão baixá-lo. No entanto, o usuário pode exibir e baixar as representações do ativo.

Consulte [configurar o download de ativos](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions).

![view-download-permission](assets/download-permissions.png)

>[!NOTE]
>
>Se um usuário for adicionado a vários grupos e um desses grupos tiver restrições, as restrições serão aplicadas ao usuário.


<!--
>Restrictions to access the original asset and their renditions do not apply to administrators even if they are members of restricted groups.
 >
 >The users can always download assets and their renditions from the repository using a `curl` request even if the download configurations are turned-off.
 >
-->

## O que mudou na 6.4.7 {#what-changed-in-647}

A versão 6.4.7 do Brand Portal traz o Visualizador de documentos, aprimora a experiência para baixar ativos e inclui correções críticas. Consulte as [Notas de versão do Brand Portal](brand-portal-release-notes.md) mais recentes.

<!--
Brand Portal 6.4.7 release brings in the Document Viewer, leverages the Brand Portal administrators to configure asset download, and centers top customer requests. See latest [Brand Portal Release Notes](brand-portal-release-notes.md).
-->

### Visualizador de documentos {#doc-viewer}

O Visualizador de documentos melhora a experiência de visualização de PDF. Ele fornece uma experiência semelhante à do Adobe Document Cloud ao exibir os arquivos PDF no Brand Portal.

Anteriormente, opções limitadas estavam disponíveis para exibir os arquivos PDF.

Com o Visualizador de documentos, os usuários do Brand Portal agora têm as opções de exibir páginas, visualizar marcadores, pesquisar texto na página, ampliar, diminuir o zoom, navegar para as páginas anteriores e posteriores, alternar para a página, ajustar para a janela, ajustar para a tela e ocultar ou mostrar a barra de ferramentas.

>[!NOTE]
>
>A experiência de exibição para outros formatos de documento permanece inalterada.


![](assets/doc-viewer.png)

### Baixar experiência {#download-configurations}

O processo de download de ativos é remodelado, fornecendo uma experiência simplificada ao usuário ao [baixar ativos do Brand Portal](brand-portal-download-assets.md).

O fluxo de trabalho existente de download de ativos do Brand Portal é inevitavelmente seguido pela aparência de uma caixa de diálogo **[!UICONTROL Download]** com várias opções de download para escolher.

No Brand Portal 6.4.7, os administradores do Brand Portal podem definir as configurações de ativo **[!UICONTROL Download]**. As configurações disponíveis são:
* **[!UICONTROL Download rápido]**
* **[!UICONTROL Representações personalizadas]**
* **[!UICONTROL Representações do sistema]**

O administrador do Brand Portal pode habilitar qualquer combinação para configurar o download de ativos.

<!--In Brand Portal 6.4.7, fast download, custom renditions, and system renditions are the three configurations available.-->

* Se as configurações de **[!UICONTROL Representações personalizadas]** e **[!UICONTROL Representações do sistema]** estiverem desativadas, as representações originais dos ativos serão baixadas sem qualquer diálogo adicional que simplifique a experiência de download para os usuários do Brand Portal.

* Se qualquer uma das **[!UICONTROL Representação personalizada]** ou **[!UICONTROL Representação do sistema]** estiver ativada, a caixa de diálogo **[!UICONTROL Download]** será exibida e o ativo original juntamente com as representações de ativos serão baixados. Ativar **[!UICONTROL Fast Download]** acelera o processo de download.

Com base na configuração, o fluxo de trabalho de download permanece constante para ativos autônomos, vários ativos, pastas contendo ativos, ativos licenciados ou não licenciados e download de ativos usando o link de compartilhamento.


## O que mudou na 6.4.6 {#what-changed-in-646}

No Brand Portal 6.4.6, o canal de autorização entre o AEM Assets e o Brand Portal é alterado. O Brand Portal agora é compatível com o AEM Assets as a Cloud Service, AEM Assets 6.3 e superior. No AEM Assets 6.3 e superior, o Brand Portal foi configurado anteriormente na interface clássica por meio do Gateway OAuth herdado, que usa a troca de token JWT para obter um token de Acesso IMS para autorização. O AEM Assets agora está configurado com o Brand Portal por meio do Adobe Developer Console, que obtém um token IMS para autorização do locatário do Brand Portal.

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

As etapas para configurar o AEM Assets com o Brand Portal são diferentes dependendo da versão do AEM e se você está configurando pela primeira vez ou atualizando as configurações existentes:

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **Versão do AEM** | **Nova configuração** | **Atualizar configuração** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Criar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e superior)** | [Criar configuração](https://docs.adobe.com/content/help/br/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Atualizar configuração](https://docs.adobe.com/content/help/pt-BR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e superior)** | [Criar configuração](https://helpx.adobe.com/br/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Atualizar configuração](https://helpx.adobe.com/br/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Entre em contato com o suporte | Entre em contato com o suporte |

>[!NOTE]
>
>É recomendável atualizar sua instância do AEM para o service pack mais recente.

Consulte as [Notas de versão do Brand Portal](brand-portal-release-notes.md) mais recentes.

Consulte [Perguntas frequentes do Brand Portal](brand-portal-faqs.md).

## O que mudou na 6.4.5 {#what-changed-in-645}


O Brand Portal 6.4.5 é uma versão do recurso que tem como objetivo fornecer aos usuários do Brand Portal (agências/equipes externas) a capacidade de carregar conteúdo no Brand Portal e publicá-lo nos AEM Assets, sem precisar acessar o ambiente de criação. Esse recurso é chamado de **[Origem de ativos no Brand Portal](brand-portal-asset-sourcing.md)** e melhorará a experiência do cliente fornecendo um mecanismo bidirecional para que os usuários contribuam e compartilhem ativos com outros usuários globais do Brand Portal.

### Origem de ativos no Brand Portal {#asset-sourcing-in-bp}

A origem dos ativos permite AEM usuários (administradores/usuários não administradores) criar novas pastas com uma propriedade adicional **Contribuição de ativos**, garantindo que a nova pasta criada seja aberta para o envio de ativos por usuários do Brand Portal. Isso aciona automaticamente um workflow que cria duas subpastas adicionais, chamadas NEW e SHARED, dentro da pasta recém-criada **Contribution**.

O usuário AEM então define o requisito fazendo o upload de um resumo sobre os tipos de ativos que devem ser adicionados à pasta de contribuição, bem como o upload de ativos da linha de base, para a pasta **SHARED** para garantir que os usuários da BP tenham as informações de referência necessárias. O administrador pode conceder acesso aos usuários ativos do Brand Portal à pasta de contribuição antes de publicar a pasta recém-criada **Contribuição** no Brand Portal.


Quando o usuário terminar de adicionar conteúdo na pasta **NEW**, ele poderá publicar a pasta de contribuição de volta no ambiente do autor do AEM. Observe que pode levar alguns minutos para concluir a importação e refletir o conteúdo recém-publicado no AEM Assets.

Além disso, todas as funcionalidades existentes permanecem inalteradas. Os usuários do Brand Portal podem visualizar, pesquisar e baixar ativos da pasta de contribuição, bem como das outras pastas permitidas. Além disso, os administradores podem compartilhar a pasta de contribuição, modificar as propriedades e adicionar ativos às coleções.

>[!NOTE]
>
>A origem dos ativos no Brand Portal é compatível com AEM 6.5.2.0 e superior.
>
>O recurso não é compatível com as versões anteriores - AEM 6.3 e AEM 6.4.

### Fazer upload de ativos para a pasta de contribuição {#upload-assets-in-bp}

Os usuários do Brand Portal com permissões apropriadas podem baixar os requisitos de ativos para entender a necessidade de contribuição e fazer upload de vários ativos ou pastas que contêm vários ativos para a pasta de contribuição. No entanto, observe que os usuários do Brand Portal só podem fazer upload de ativos para a subpasta **NEW**. A pasta **SHARED** destina-se à distribuição de requisitos e ativos de linha de base.

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### Publicar a pasta de contribuição no AEM Assets {#publish-assets-to-aem}

Quando o upload for concluído na pasta **NEW**, os usuários do Brand Portal poderão publicar a pasta de contribuição de volta para o AEM. Pode levar alguns minutos para importar e refletir o conteúdo/ativos publicados no AEM Assets. Consulte [Publicar a pasta de contribuição para o AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## O que mudou na 6.4.4 {#what-changed-in-644}

A versão 6.4.4 do Brand Portal foca em melhorias na pesquisa de texto e nas principais solicitações do cliente. Consulte as [Notas de versão do Brand Portal](brand-portal-release-notes.md) mais recentes.

### Melhorias de pesquisa

O Brand Portal 6.4.4 em diante oferece suporte à pesquisa de texto parcial no predicado de propriedade no painel de filtragem. Para permitir pesquisa de texto parcial, é necessário ativar **Pesquisa parcial** no Predicado de propriedade no formulário de pesquisa.

Leia para saber mais sobre pesquisa de texto parcial e pesquisa curinga.

#### Pesquisa de frase parcial {#partial-phrase-search}

Agora é possível pesquisar ativos especificando apenas uma parte, ou seja, uma palavra ou duas, da frase pesquisada no painel de filtragem.

**Use**
caseA pesquisa parcial de frase é útil quando você não tem certeza da combinação exata de palavras que ocorrem na frase pesquisada.

Por exemplo, se o formulário de pesquisa no Brand Portal usar o Predicado de propriedade para pesquisa parcial no título dos ativos, a especificação do termo **camp** retorna todos os ativos com a palavra camp na frase de título.

![](assets/partialphrasesearch.png)

#### Pesquisa curinga {#wildcard-search}

O Brand Portal permite usar o asterisco (*) na consulta de pesquisa junto com uma parte da palavra na frase pesquisada.

****
Caso de usoSe você não tiver certeza das palavras exatas que ocorrem na frase pesquisada, poderá usar uma pesquisa curinga para preencher as lacunas em sua consulta de pesquisa.

Por exemplo, especificar **climb*** retorna todos os ativos com palavras que começam com os caracteres **climb** em sua frase de título, se o formulário de pesquisa no Brand Portal usar o Predicado de propriedade para pesquisa parcial no título dos ativos.

![](assets/wildcard-prop.png)

Da mesma forma, especificando:

* ***** cria todos os ativos com palavras que terminam com caracteres  **** ultrapassando sua frase de título.

* ***climb*** retorna todos os ativos que têm palavras incluindo os caracteres que  **** excedem sua frase de título.

>[!NOTE]
>
>Ao marcar a caixa de seleção **Pesquisa parcial**, **Ignorar maiúsculas e minúsculas** é selecionado por padrão.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## O que mudou na 6.4.3 {#what-changed-in}

A versão 6.4.3 do Brand Portal tem como foco — fornecendo às organizações um alias alternativo, além da ID do locatário no URL de acesso do Brand Portal, nova configuração de hierarquia de pastas, aprimoramentos no suporte a vídeo, publicação agendada da instância do autor do AEM para o Brand Portal, melhorias operacionais — e atende a solicitações do cliente.

### Navegação da hierarquia de pastas para não administradores

Agora, os administradores podem configurar como as pastas são exibidas para usuários não administradores (editores, visualizadores e usuários convidados) no logon. [A configuração Ativar ](../using/brand-portal-general-configuration.md) hierarquia de pastas é adicionada em Configurações  **gerais**, no painel Ferramentas administrativas. Se a configuração for:

* **ativada**, a árvore de pastas que começa na pasta raiz está visível para usuários não administradores. Dessa forma, a concessão de uma experiência de navegação semelhante aos administradores.
* **desativado**, somente as pastas compartilhadas são exibidas na landing page.

![](assets/enable-folder-hierarchy.png)

A funcionalidade [Ativar hierarquia de pasta](../using/brand-portal-general-configuration.md) (quando ativada) ajuda a diferenciar as pastas com os mesmos nomes compartilhados de hierarquias diferentes. Ao fazer logon, usuários não administradores agora visualizam as pastas pai virtual (e ancestral) das pastas compartilhadas.

![](assets/disabled-folder-hierarchy1-2.png)

![](assets/enabled-hierarchy1-2.png)

As pastas compartilhadas são organizadas nos respectivos diretórios em pastas virtuais. Você pode reconhecer essas pastas virtuais com um ícone de cadeado.

Observe que a miniatura padrão das pastas virtuais é a imagem em miniatura da primeira pasta compartilhada.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Pesquisar na hierarquia ou caminho de pasta específico

**O predicado** Navegador de caminhos é introduzido no Formulário de pesquisa para permitir a pesquisa de ativos em um diretório específico. O caminho de pesquisa padrão do predicado de pesquisa para Navegador de caminhos é `/content/dam/mac/<tenant-id>/`, que pode ser configurado ao editar o formulário de pesquisa padrão.

* Os usuários administradores podem usar o Navegador de caminhos para navegar até qualquer diretório de pastas no Brand Portal.
* Usuários não administradores podem usar o Navegador de caminhos para navegar somente para as pastas (e navegar de volta para as pastas pai) compartilhadas com eles.

   Por exemplo, `/content/dam/mac/<tenant-id>/folderA/folderB/folderC` é compartilhado com um usuário não administrador. O usuário pode pesquisar ativos na pastaC usando o Navegador de caminhos. Esse usuário também pode navegar para folderB e folderA (já que são ancestrais da folderC compartilhada com o usuário).

![](assets/edit-search-form.png)


Agora é possível restringir a pesquisa de ativos em uma pasta específica que você buscou, em vez de começar na pasta raiz.

Observe que pesquisar nessas pastas retorna resultados somente dos ativos que foram compartilhados com o usuário.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Suporte para representações de vídeo do Dynamic Media

Os usuários cuja instância do autor do AEM esteja no modo híbrido do Dynamic Media podem visualizar e baixar as representações de mídia dinâmica, além dos arquivos de vídeo originais.

Para permitir a pré-visualização e o download de representações de mídia dinâmica em contas de locatários específicas, os administradores precisam especificar **Configuração do Dynamic Media** (URL do serviço de vídeo (URL do Gateway DM) e ID de registro para buscar o vídeo dinâmico) na configuração **Vídeo** do painel de ferramentas administrativas.


Os vídeos do Dynamic Media podem ser visualizados em:

* Página Detalhes do ativo
* Exibição de cartão do ativo
* Página de visualização de compartilhamento de link

É possível baixar os códigos de vídeo do Dynamic Media em:

* Brand Portal
* Link compartilhado

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publicação agendada para o Brand Portal

Fluxo de trabalho de publicação de ativos (e pastas) de [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) A instância do autor no Brand Portal pode ser agendada para uma data e hora posterior.

Da mesma forma, os ativos publicados podem ser removidos do portal em uma data posterior (hora), agendando o fluxo de trabalho Cancelar publicação do Brand Portal .

![](assets/schedule-publish.png)

![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias do locatário configurável no URL

As organizações podem personalizar o URL do portal, com um prefixo alternativo no URL. Para obter um alias para o nome do locatário em seu URL de portal existente, as organizações precisam entrar em contato com o suporte ao Adobe.

Observe que somente o prefixo do URL do Brand Portal pode ser personalizado e não o URL inteiro.\
Por exemplo, uma organização com o domínio existente **geomettrix.brand-portal.adobe.com** pode obter **geomettrixinc.brand-portal.adobe.com** criado mediante solicitação.

No entanto, a instância do autor do AEM pode ser [configurada](https://helpx.adobe.com/br/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) somente com o URL da ID do locatário e não com o URL do alias do locatário (alternativo).

As organizações podem atender às suas necessidades de marca, personalizando o URL do portal, em vez de aderir ao URL fornecido pelo Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Fazer download de aprimoramentos de experiência

O lançamento oferece uma experiência de download simplificada com um número reduzido de cliques e avisos, em:

* Optar por baixar apenas as representações (e não os ativos originais).
* Baixar os ativos quando o acesso às renderizações originais é restrito.

## O que mudou na 6.4.6 {#what-changed-in-1}

A versão do Brand Portal 6.4.2 traz uma variedade de recursos para atender às necessidades de distribuição de ativos das organizações e ajudá-las a alcançar um grande número de usuários distribuídos globalmente por meio do acesso de Convidado e da experiência ideal com downloads acelerados. O Brand Portal também oferece maior controle às organizações por meio de novas configurações para administradores, relatórios recém-adicionados e atende a solicitações de clientes.

### Acesso de convidado

![](assets/bp-login-screen-1.png)

AEM Portal da Marca permite acesso de convidado ao portal. Um usuário convidado não precisa de credenciais para entrar no portal e pode acessar e baixar todas as pastas públicas e coleções. Os usuários convidados podem adicionar ativos a seu lightbox (coleção privada) e baixar o mesmo. Eles também podem visualizar a pesquisa de tags inteligentes e os predicados de pesquisa definidos pelos administradores. A sessão de convidado não permite que os usuários criem coleções e pesquisas salvas ou as compartilhe mais, acesse as configurações de pastas e coleções e compartilhe ativos como links.

Em uma organização, várias sessões de convidado simultâneas são permitidas, o que é limitado a 10% da cota total do usuário por organização.

Uma sessão de convidado permanece ativa por duas horas. Portanto, o estado do lightbox também é preservado até duas horas a partir da hora de início da sessão. Após duas horas, a sessão de convidado deve ser reiniciada, para que o estado do lightbox seja perdido.

### Downloads acelerados

Os usuários do Brand Portal podem aproveitar os downloads rápidos baseados no IBM Aspera Connect para obter velocidades 25 vezes mais rápidas e desfrutar de uma experiência de download contínua, independentemente de sua localização em todo o mundo. Para baixar os ativos mais rapidamente no Brand Portal ou no link compartilhado, os usuários precisam selecionar a opção **Ativar aceleração de download** na caixa de diálogo de download, desde que a aceleração de download esteja ativada em sua organização.

![](assets/donload-assets-dialog-2.png)

Para habilitar o download acelerado baseado em IBM Aspera para a organização, os administradores **Ativar Aceleração de Download** (que está desabilitada por padrão) de [Configurações Gerais](brand-portal-general-configuration.md#allow-download-acceleration) no painel de ferramentas administrativas. Para saber mais sobre os pré-requisitos e as etapas de solução de problemas para baixar arquivos de ativos mais rapidamente do Brand Portal e links compartilhados, consulte [Guia para acelerar downloads do Brand Portal](../using/accelerated-download.md#main-pars-header).

### Relatório de logons do usuário

Um novo relatório, para rastrear os logons de usuários, foi introduzido. O relatório **Logons de Usuário** pode ser fundamental para permitir que as organizações auditem e mantenham uma verificação sobre os administradores delegados e outros usuários do Brand Portal.

Os logs de relatório exibem nomes, IDs de email, personas (administrador, visualizador, editor, convidado), grupos, último logon, status da atividade e contagem de logon de cada usuário da implantação do Brand Portal 6.4.2 até o momento da geração do relatório. Os administradores podem exportar o relatório como .csv. Juntamente com outros relatórios, o relatório Logons de usuário permite que as organizações monitorem mais detalhadamente as interações do usuário com os recursos de marca aprovados, garantindo assim a conformidade com os escritórios de conformidade corporativa.

![](assets/user-logins-1.png)

### Acesso a representações originais

Os administradores podem restringir o acesso do usuário aos arquivos de imagem originais (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .gmbox, psd, image/vnd.adobe.photoshop) e dar acesso a representações de baixa resolução que baixam do Brand Portal ou do link compartilhado. Esse acesso pode ser controlado no nível do grupo de usuários na guia Grupos da página Funções do usuário no painel Ferramentas administrativas.

![](assets/access-original-rend-1.png)

* Por padrão, todos os usuários podem baixar representações originais, pois o Acesso ao Original está ativado para todos.
* Os administradores precisam desmarcar as respectivas caixas de seleção para impedir que um grupo de usuários acesse as representações originais.
* Se um usuário for membro de vários grupos, mas apenas um dos grupos tiver restrições, as restrições se aplicarão a esse usuário.
* As restrições não se aplicam a administradores, mesmo sendo membros de grupos restritos.
* As permissões do usuário que compartilha ativos como link se aplicam aos usuários que baixam ativos usando links compartilhados.

### Caminho da hierarquia de pastas nas visualizações de Cartão e Lista

Os cartões de pastas, na Exibição de cartão, agora exibem informações de hierarquia de pastas para usuários não administradores (Editor, Visualizador e Usuário convidado). Essa funcionalidade permite que os usuários saibam o local das pastas que estão acessando, em relação à hierarquia principal.

As informações de hierarquia de pastas são particularmente úteis na diferenciação de pastas com nomes semelhantes a outras pastas compartilhadas de uma hierarquia de pasta diferente. Se os usuários não administradores não estiverem cientes da estrutura de pastas dos ativos compartilhados com eles, os ativos/pastas com nomes semelhantes parecerão confusos.

* Os caminhos mostrados nos respectivos cartões são truncados para se ajustarem aos tamanhos dos cartões. No entanto, os usuários podem ver o caminho completo como uma dica de ferramenta ao passar o cursor do mouse sobre o caminho truncado.

![](assets/folder-hierarchy1-1.png)

Exibição de lista mostra o caminho da pasta de ativos em uma coluna para todos os usuários do Brand Portal.

![](assets/list-view-1.png)

### Opção de visão geral para exibir propriedades de ativos

O Brand Portal oferece a opção Visão geral para usuários não administradores (Editores, Visualizadores, Usuários convidados) para exibir as Propriedades do ativo de ativos/pastas selecionadas. A opção Visão geral está visível:

1. Na barra de ferramentas, na parte superior, ao selecionar um ativo/pasta.
2. Na lista suspensa ao selecionar o Seletor de painéis.

Ao selecionar a opção Visão geral enquanto um ativo/pasta é selecionado, os usuários podem ver o título, o caminho e o horário da criação do ativo. Enquanto isso, na página Detalhes do ativo, a opção Visão geral permite que os usuários vejam os metadados do ativo.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Novas configurações

Seis novas configurações são adicionadas aos administradores para ativar/desativar as seguintes funcionalidades em locatários específicos:

* Permitir acesso de convidado
* Permitir que usuários solicitem acesso ao Brand Portal
* Permitir que administradores excluam ativos do Brand Portal
* Permitir criação de coleções públicas
* Permitir a criação de coleções inteligentes públicas
* Permitir aceleração de download

As configurações acima estão disponíveis em Access e General settings no painel de ferramentas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Interface do usuário do Adobe I/O para configurar integrações de oAuth

O Brand Portal 6.4.2 em diante usa a interface Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para criar o aplicativo JWT, que permite a configuração de integrações oAuth para permitir a integração do AEM Assets com o Brand Portal. Anteriormente, a interface do usuário para configurar integrações OAuth era hospedada em `https://marketing.adobe.com/developer/`. Para saber mais sobre a integração do AEM Assets com o Brand Portal para publicação de ativos e coleções no Brand Portal, consulte [Configurar integração do AEM Assets com o Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html).

## Melhorias de pesquisa

Os administradores podem fazer a propriedade predicar não diferencia maiúsculas de minúsculas usando o predicado de propriedade atualizado, que tem uma verificação para Ignorar maiúsculas e minúsculas. Essa opção está disponível para predicado de propriedade e predicado de propriedade de vários valores.\
No entanto, a pesquisa que não diferencia maiúsculas de minúsculas é comparativamente mais lenta que a pesquisa padrão por predicado de propriedade. Se houver muitos predicados que não diferenciam maiúsculas de minúsculas no filtro de pesquisa, a pesquisa poderá desacelerar. É, portanto, aconselhável usar judiciosamente a pesquisa que não diferencia maiúsculas de minúsculas.

## O que mudou na 6.4.1 {#what-changed-in-2}

O Brand Portal 6.4.1 é uma versão de atualização da plataforma que traz vários novos recursos e aprimoramentos vitais, como navegação, pesquisa e aprimoramentos de desempenho para fornecer experiências completas aos clientes.

### Melhorias de navegação

* Novo painel Árvore de conteúdo para navegar rapidamente por uma hierarquia de ativos.

![](assets/contenttree-2.png)

* Foram introduzidos novos atalhos de teclado, por exemplo _(p)_ para navegação até a página de propriedades, _(e)_ para Editar e _(ctrl+c)_ para operações de cópia.
* Melhoria na rolagem e na experiência de carregamento lento na exibição de cartão e lista para a navegação de um grande número de ativos.
* Exibição de cartão aprimorada com suporte para placas de tamanho diferente com base na configuração de exibição.

![](assets/cardviewsettings-1.png)

* A exibição de cartão agora exibe o carimbo de data/hora ao passar o cursor do mouse sobre o rótulo de data.

* Exibição de Coluna aprimorada com **Mais detalhes** no instantâneo de ativo, que permite navegar até a página de detalhes de um ativo.

![](assets/columnmoredetail.png)

* A exibição em Lista agora exibe os nomes de arquivo dos ativos na primeira coluna por padrão, além das informações de local, tipo de ativo, dimensões, tamanho, classificação e publicação. É possível usar as novas **Configurações de exibição** para configurar a quantidade de detalhes a serem exibidos na exibição em Lista.

* Melhoria na experiência de detalhes do ativo com a capacidade de navegar para frente e para trás entre ativos usando novos botões de navegação e visualizar a contagem de ativos.

![](assets/navbtn.png)

* Novo recurso para visualizar arquivos de áudio, carregados do AEM, na página de detalhes do ativo.
* Novo recurso Ativos relacionados fornecido nas propriedades dos Ativos. Os ativos relacionados a outros ativos de origem/derivados no AEM e publicados no Brand Portal agora têm seu relacionamento intacto no Brand Portal, com links para os ativos relacionados na página de propriedades.
* Uma nova configuração para impedir que usuários não administradores criem coleções públicas foi introduzida. As organizações podem trabalhar com a equipe de suporte do Adobe para configurar esse recurso em contas específicas.

### Melhorias de pesquisa

* Recurso introduzido para retornar à mesma posição nos resultados da pesquisa, após navegar até um item de pesquisa, sem executar a consulta de pesquisa novamente.
* Novos resultados da Pesquisa contam para exibir o número de resultados da pesquisa fornecidos.
* Filtro de pesquisa do tipo de arquivo aprimorado com a capacidade de filtrar resultados de pesquisa com base em tipos MIME refinados, como .jpg, .png e .psd, em comparação com as opções de imagens, documentos, multimídia anteriores.
* Filtros de pesquisa aprimorados para coleções, com carimbos de data e hora precisos em vez da funcionalidade de controle deslizante de hora anterior.
* Novos filtros de tipo de acesso foram introduzidos para procurar coleções que são públicas ou não.

![](assets/accesstypefilter.png)

### Otimizações de download

* Um único arquivo grande é baixado diretamente, sem a criação do arquivo zip, melhorando assim a velocidade e a taxa de transferência.
* O limite de download do Zip para o recurso de compartilhamento de link aumentou para 5 GB, de 1 GB.

* Agora os usuários podem optar por baixar somente os arquivos personalizados e originais e evitar representações prontas para uso, enquanto baixam ativos do Brand Portal ou por meio do recurso de links compartilhados.

![](assets/excludeautorendition.png)

### Melhorias de desempenho

* Melhoria de até 100% na velocidade de download de ativos.
* Aprimoramento de até 40% na resposta de pesquisa para ativos.
* Melhoria de até 40% no desempenho da navegação.

**Observação**: As melhorias citadas são conforme os testes feitos em laboratório.

### Recursos de relatório aprimorados

**Relatório de compartilhamento de links introduzidoUm novo**
relatório, que fornece informações sobre links compartilhados, foi introduzido. O relatório Compartilhamento de links lista todos os URLs, para os ativos, compartilhados com usuários internos e externos em toda a organização no período de tempo especificado. Ele também informa quando o link foi compartilhado, por quem e quando ele expira.

![](assets/navigatereport.png)

**Modificado o ponto de entrada para acessar o**
relatório de Uso. O relatório de Uso agora é consolidado com outros relatórios e agora pode ser visualizado no console Relatórios de ativos. Para acessar o console Relatórios de ativos , navegue até **Criar/gerenciar relatórios** no painel Ferramentas administrativas.

![](assets/accessassetreport.png)

**A experiência do usuário aprimorada com a interface**
de relatórios no Brand Portal tornou-se mais intuitiva e confere maior controle às organizações. Além de criar vários relatórios, os administradores agora podem revisitar os relatórios gerados e baixá-los ou excluí-los, pois esses relatórios são salvos no Brand Portal.

Cada relatório que está sendo criado pode ser personalizado adicionando ou removendo colunas padrão. Além disso, colunas personalizadas podem ser adicionadas aos relatórios Download, Expiração e Publicação para controlar o grau de granularidade.

### Ferramentas administrativas aprimoradas

O seletor de propriedades foi aprimorado nas ferramentas de administração para Metadados, Pesquisa e Relatórios com recursos de navegação e Type-ahead para simplificar a experiência administrativa.

### Outras melhorias

* Os ativos publicados no Brand Portal a partir dos AEM 6.3.2.1 e 6.4 agora podem ser disponibilizados publicamente para usuários gerais do Brand Portal, marcando a caixa de seleção Publicação de pasta pública na caixa de diálogo Replicação do AEM Assets Brand Portal.

![](assets/public-folder-publish.png)

* Os administradores são notificados por meio de emails de solicitação de acesso, além das notificações na área de notificação do Brand Portal, se alguém tiver solicitado acesso ao Brand Portal.

## O que mudou na 6.3.2 {#what-changed-in-3}

O Brand Portal 6.3.2 inclui funcionalidades novas e aprimoradas voltadas para as principais solicitações do cliente e aprimoramentos gerais de desempenho.

### Solicitar acesso ao Brand Portal {#request-access-to-brand-portal}

Agora os usuários podem solicitar acesso ao Brand Portal usando o novo recurso **need access** disponível na tela de logon do Brand Portal.

![](assets/bplogin_request_access.png)

Dependendo de os usuários terem uma Adobe ID ou precisarem criar uma Adobe ID, os usuários podem seguir o fluxo de trabalho apropriado para enviar uma solicitação. Os administradores de produtos do Brand Portal recebem essas solicitações na área de notificação e concedem acesso por meio do Adobe Admin Console.

Para obter mais informações, consulte [Solicitar acesso ao Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Aprimoramento no relatório de ativos baixados {#enhancement-in-the-assets-downloaded-report}

O relatório de ativos baixados agora inclui a contagem de download de ativos por usuário dentro da data e do intervalo de tempo especificados. Os usuários podem baixar esse relatório no formato .csv e compilar dados como a contagem total de download de um ativo licenciado.

![](assets/reports_download_downloaded_by.png)

Para obter mais informações, consulte as Etapas 3 e 6 em [Criar e gerenciar relatórios adicionais](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Notificação de manutenção do Brand Portal {#brand-portal-maintenance-notification}

O Brand Portal agora exibe um banner de notificação alguns dias antes de uma atividade de manutenção futura. Um exemplo de notificação:

![](assets/bp_maintenance_notification-1.png)

Para obter mais informações, consulte [Notificação de manutenção do Brand Portal](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### Aprimoramento de ativos licenciados compartilhados usando o recurso de compartilhamento de link {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Ao baixar ativos licenciados usando o recurso de compartilhamento de link, agora é solicitado que você concorde com o contrato de licença desses ativos.

![](assets/copyright_management.png)

Para obter mais informações, consulte Etapa 12 em [Compartilhar ativos como um link](../using/brand-portal-link-share.md#shareassetsasalink).

### Aprimoramento do seletor de usuários {#user-picker-enhancement}

O desempenho do seletor de usuários agora é aprimorado para atender às necessidades dos clientes com uma grande base de usuários.

### Alterações na marca da Experience Cloud {#experience-cloud-branding-changes}

O Brand Portal agora está em conformidade com a nova marca Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## O que mudou na 6.3.1 {#what-changed-in-4}

O Brand Portal 6.3.1 inclui funcionalidades novas e aprimoradas voltadas para o alinhamento do Brand Portal com o AEM.

### Interface do usuário atualizada {#upgraded-user-interface}

Para alinhar a experiência do usuário do Brand Portal com o AEM, o Adobe está fazendo a transição para a interface do usuário do Coral 3. Essa alteração melhora a utilização geral, incluindo navegação e aparência.

#### Experiência de navegação aprimorada {#enhanced-navigational-experience}

* Acesso rápido às ferramentas administrativas por meio do novo logotipo do Adobe:

![](assets/aemlogo-3.png)

* Navegação do produto por meio de uma sobreposição:

![](assets/overlay_navigation.png)

* Navegação rápida para pastas principais:

![](assets/navigationparentfolders.png)

* Pesquisa e navegação rápidas para o conteúdo e as ferramentas necessárias:

![](assets/omnisearchicon.png)

### Experiência de navegação aprimorada {#enhanced-browsing-experience}

* Nova exibição de coluna para navegar pelas pastas aninhadas:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* Na lista de ativos em uma pasta, o ativo mais recente carregado aparece na parte superior.

### Experiência de pesquisa aprimorada {#enhanced-search-experience}

* O novo recurso de pesquisa Omni facilita o acesso rápido a conteúdo, recursos ou tags relevantes por meio de sugestões automáticas ao digitar palavras-chave de pesquisa. A pesquisa Omni está disponível em todos os recursos de pesquisa.

![](assets/omnisearch_whatsnew.png)

* Você também pode adicionar filtros de pesquisa à pesquisa Omni para restringir ainda mais e agilizar sua pesquisa.

![](assets/omnisearch_withfilters.png)

* A nova pesquisa baseada na classificação de ativos permite pesquisar ativos com classificações, se publicada pela AEM Assets.
* O novo recurso de pesquisa de vários valores aceita várias palavras-chave com o operador AND para descobrir ativos mais rapidamente.
* O novo recurso de reforço de pesquisa permite melhorar a relevância da pesquisa para que ativos específicos apareçam na parte superior dos resultados da pesquisa.
* O novo recurso de pesquisa baseado em caminho permite fornecer o caminho para uma pasta aninhada para poder pesquisar ativos nessa pasta.

#### Nova pesquisa baseada em tags inteligentes {#new-smart-tags-based-search}

Se imagens com tags inteligentes forem publicadas do AEM Assets para o Brand Portal, você poderá pesquisar por essas imagens no Brand Portal usando os nomes das tags inteligentes como palavras-chave de pesquisa. Este recurso está disponível somente para arquivos.

### Experiência aprimorada de download {#enhanced-downloading-experience}

Após baixar uma pasta aninhada, é possível preservar a hierarquia da pasta original. Os ativos dentro de uma pasta aninhada podem ser baixados em uma única pasta, em vez de pastas separadas.

### Desempenho aprimorado {#improved-performance}

Aprimoramentos nos recursos de navegação, pesquisa e download melhoram significativamente o desempenho do Brand Portal.

### Novo gerenciamento de direitos digitais para ativos {#new-digital-rights-management-for-assets}

Os administradores podem definir a data e a hora de expiração dos ativos antes de compartilhá-los. Depois que um ativo expira, ele fica visível para visualizadores e editores, mas não é baixável. Quando um ativo expira, os administradores recebem uma notificação.

### Classificação de ativo aprimorada {#enhanced-asset-sorting}

A classificação de ativos em uma pasta na exibição de lista não está mais restrita ao número de ativos que estão sendo exibidos na primeira página. Todos os ativos em uma pasta são classificados, independentemente de todos estarem listados na primeira página.

### Relatórios aprimorados {#reporting-capabilities}

Os administradores podem criar e gerenciar três tipos de relatórios: ativos baixados, expirados e publicados. A capacidade de configurar as colunas em um relatório e exportar os relatórios para o formato CSV também está disponível.

![](assets/newreport.png)

### Metadados adicionais {#additional-metadata}

O Brand Portal 6.3.1 apresenta metadados adicionais, que estão ao mesmo nível do AEM Assets 6.3. Você pode usar o formulário Editor de esquema para controlar os metadados que devem estar visíveis na página Propriedades do ativo. Os metadados do ativo não estão visíveis para os usuários de compartilhamento de link externo, que só podem visualizar e baixar ativos usando o URL de compartilhamento de link.

![](assets/additionsinmetadata.png)

### Recursos adicionais para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar as personalizações no wallpaper da tela de logon, os administradores podem visualizar as alterações.

![](assets/wallpaperpreview.png)

* Depois que um administrador adiciona novos usuários, eles não precisam aceitar convites para serem adicionados ao Brand Portal, então eles são adicionados automaticamente.

### Novos recursos de publicação no AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* AEM administradores podem publicar esquema de metadados do AEM Assets no Brand Portal usando o AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponível no quarto trimestre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Os administradores de AEM podem publicar todas as tags do AEM Assets no Brand Portal usando o AEM 6.2 SP1-CFP7 e o AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* No AEM Assets, é possível publicar ativos e coleções que têm tags, incluindo tags inteligentes. Em seguida, você pode pesquisar por esses ativos ou coleções usando essas tags como palavras-chave de pesquisa no Brand Portal.
