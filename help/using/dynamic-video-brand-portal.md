---
title: Suporte a vídeo dinâmico no Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Suporte a vídeo dinâmico no Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 2%

---

# Suporte a vídeo dinâmico no Brand Portal {#dynamic-video-support-on-brand-portal}

Visualize e reproduza vídeos de forma adaptável no Brand Portal com suporte ao Dynamic Media. Baixe também as representações dinâmicas do portal e dos links compartilhados.
Os usuários do Brand Portal podem:

* Visualize vídeos na página Detalhes do ativo, Exibição de cartão e página de visualização do compartilhamento de link.
* Reproduzir codificações de vídeo na página Detalhes do ativo.
* Exiba representações dinâmicas na guia Representações na página Detalhes do ativo .
* Baixe codificações de vídeo e pastas que contêm vídeos.

>[!NOTE]
>
>Para trabalhar com vídeos e publicá-los no Brand Portal, verifique se a instância do autor do Experience Manager está configurada no modo Dynamic Media Hybrid ou no modo Dynamic Media **[!DNL Scene 7]** .

Para visualizar, reproduzir e baixar vídeos, o Brand Portal expõe as duas configurações a seguir para os administradores:

* [Dynamic Media Hybrid ](#configure-dm-hybrid-settings)
configurationSe a instância do Experience Manager Author estiver em execução no modo Híbrido de mídia dinâmica.
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
MediaConfigurationSe a instância Autor do Experience Manager estiver em execução no **[!DNL Scene 7]** modo de mídia dinâmica.
Defina qualquer uma dessas configurações com base nas configurações definidas na instância do Autor do Experience Manager com a qual o locatário do Brand Portal é replicado.

>[!NOTE]
>
>Vídeos dinâmicos não são compatíveis com locatários do Brand Portal configurados com Autor do Experience Manager em execução no modo de execução **[!UICONTROL Scene7Connect]**.

## Como os vídeos dinâmicos são reproduzidos? {#how-are-dynamic-videos-played}

![Os códigos de vídeo são obtidos da nuvem](assets/VideoEncodes.png)

Se as configurações do Dynamic Media ([Configurações híbridas](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) estiverem configuradas no Brand Portal, as representações dinâmicas serão buscadas no servidor **[!DNL Scene 7]**. Os códigos de vídeo são, portanto, pré-visualizados e reproduzidos sem demora e distorcem a qualidade.

Como as codificações de vídeo não são armazenadas no repositório do Brand Portal e são buscadas no servidor **[!DNL Scene 7]**, verifique se as configurações do Dynamic Media na Instância do autor do AEM e no Brand Portal são as mesmas.

>[!NOTE]
>
>Visualizadores de vídeo e predefinições do visualizador não são compatíveis com o Brand Portal. Os vídeos são visualizados e reproduzidos nos visualizadores padrão do Brand Portal.

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos no Brand Portal, certifique-se de:

* **Inicie o AEM Author no**
modo DM (Dynamic Media): inicie a instância do AEM Author (com a qual o Brand Portal está configurado) no  [modo ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) Dynamic Media Hybrid ou no  [Dynamic  [!DNL Scene 7] Mediamode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html).
* **Configurar os serviços em nuvem da Dynamic Media AEM**
AutorCom base no modo Dynamic Media em que o AEM Author está em execução, defina qualquer um dos serviços em nuvem da  [Dynamic Media ou os serviços em ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) nuvem  [[!DNL Scene 7] no AEM Author a partir de ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) Ferramentas **|** Cloud Services **|** Dynamic Media ****.
* **Configurar o Dynamic Media no Brand**
PortalCom base nas configurações de nuvem do Dynamic Media no AEM Author, configure as configurações ou  [configurações do ](#configure-dm-hybrid-settings) Dynamic Media  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  nas ferramentas administrativas do Brand Portal.
Certifique-se de que [locatários separados do Brand Portal](#separate-tenants) sejam usados para instâncias do autor do AEM configuradas com os modos Dynamic Media Hybrid e Dynamic Media **[!UICONTROL Scene7]**, se estiver usando funcionalidades do Dynamic Media Hybrid e do Dynamic Media **[!UICONTROL S7]**.
* **Publique pastas com códigos de vídeo aplicados ao Brand**
PortalAplique códigos de  [ ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) vídeo e publique a pasta que contém ativos de mídia avançada da instância do autor do AEM no Brand Portal.
* **lista de permissões IPs de saída no SPS se a visualização segura estiver**
ativadaSe estiver usando o Dynamic Media-**[!DNL Scene 7]**  (com a visualização  [segura ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) ativada para uma empresa), recomenda-se que o administrador da  **[!DNL Scene 7]** empresa  [lista de permissões os ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IPs de saída públicos para as respectivas regiões usando a interface flash do SPS (**[!UICONTROL Scene 7]** Publishing System).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189,1 |
| APAC | 63 140 44,54 |

Para incluir uma lista de permissões desses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Práticas recomendadas    

Para garantir que seus ativos de vídeo dinâmico sejam visualizados, reproduzidos e baixados com êxito do Brand Portal (e links compartilhados), siga estas práticas:

### Locatários separados para os modos Dynamic Media Hybrid e Dynamic Media Scene7 {#separate-tenants}

Se estiver usando os recursos Dynamic Media **[!DNL Scene 7]** e Dynamic Media Hybrid, recomenda-se usar diferentes locatários Brand Portal para instâncias de Autor AEM configuradas com os modos Dynamic Media Hybrid e Dynamic Media **[!DNL Scene 7]** .


![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Os mesmos detalhes de configuração na instância de autor do AEM e no Brand Portal

Certifique-se de que os detalhes de configuração, como **[!UICONTROL Título]**, **[!UICONTROL ID de registro]**, **[!UICONTROL URL do serviço de vídeo]** (em **[!UICONTROL Dynamic Media Hybrid]**) e **[!UICONTROL Título]**, credenciais (**[!UICONTROL Email]** e Senha), 12/>Região ]**,**[!UICONTROL  Empresa ]**(no Dynamic Media **[!DNL Scene 7]**)- são as mesmas no Brand Portal e**[!UICONTROL  AEM configuração de nuvem ]**.**[!UICONTROL 

### lista de permissões os IPs de saída públicos para o modo Dynamic Media Scene7

Se o Dynamic Media **[!UICONTROL Scene 7]** com [visualização segura ativada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-for usado para fornecer ativos de vídeo ao Brand Portal, o **[!UICONTROL Scene 7]** criará um servidor de imagem dedicado para ambientes de preparo ou aplicativos internos. Qualquer solicitação para este servidor verifica o endereço IP de origem. Se a solicitação recebida não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada.
O **[!UICONTROL Administrador da empresa do Scene-7]**, portanto, configura uma lista aprovada de endereços IP para o ambiente **[!UICONTROL Teste seguro]** de sua empresa, por meio da interface flash do **[!UICONTROL SPS]** (Scene-7 Publishing System). Certifique-se de que o IP de saída da respectiva região (a partir do seguinte) seja adicionado a essa lista aprovada.
Para incluir uma lista de permissões desses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189,1 |
| APAC | 63 140 44,54 |

## Definir configurações do Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Se a instância do autor do AEM estiver em execução no modo híbrido do dynamic media, use o bloco **[!UICONTROL Video]** do painel de ferramentas administrativas para definir as configurações do gateway do Dynamic Media.

>[!NOTE]
>
>Os [perfis de codificação de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) não são publicados no Brand Portal, em vez disso, são buscados no servidor **[!UICONTROL Scene7]**. Portanto, para que os códigos de vídeo sejam reproduzidos com êxito no Brand Portal, verifique se os detalhes de configuração são iguais ao [Scene7 cloud configuration](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) em sua instância do AEM Author.

Para configurar configurações do Dynamic Media em locatários do Brand Portal:

1. Selecione o logotipo do AEM para acessar ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.
1. No painel Ferramentas administrativas, selecione o bloco **[!UICONTROL Vídeo]**.

   ![Configuração híbrida do Dynamic Media no Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL A página Editar]** configuração do Dynamic Media é aberta.

   ![Configuração híbrida do Dynamic Media no Brand Portal](assets/edit-dynamic-media-config.png)

1. Especifique **[!UICONTROL ID de Registro]** e **[!UICONTROL URL do Serviço de Vídeo]** (URL do Gateway DM). Certifique-se de que esses detalhes sejam os mesmos que em **[!UICONTROL Tools > Cloud Services]** na instância do autor do AEM.
1. Selecione **Save** para guardar a configuração.

## Definir configurações do Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se a instância do autor do AEM estiver em execução no modo Dynamic Media- **[!UICONTROL Scene7]**, use o bloco **[!UICONTROL Dynamic Media Configuration]** do painel de ferramentas administrativas para definir as configurações do servidor **[!UICONTROL Scene7]**.

Para configurar configurações do Dynamic Media **[!UICONTROL Scene7]** em locatários Brand Portal:

1. Selecione o logotipo do AEM para acessar ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.

2. No painel Ferramentas administrativas, selecione o bloco **[!UICONTROL Configuração do Dynamic Media]**.

   ![Configuração do DM  [!UICONTROL Scene 7] no Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL A página Editar]** configuração do Dynamic Media é aberta.

   ![Configuração do Scene7 no Brand Portal](assets/S7Config.png)

3. Fornecer:

   * **[!UICONTROL Título]**
   * Credenciais (**[!UICONTROL Email ID]** e **[!UICONTROL Password]**) para acessar o servidor Scene7
   * **[!UICONTROL Região]**

   Certifique-se de que esses valores sejam os mesmos da sua instância do autor do AEM.

4. Selecione **[!UICONTROL Conectar-se ao Dynamic Media]**.

5. Forneça o **[!UICONTROL Company name]** e **[!UICONTROL Save]** a configuração.
