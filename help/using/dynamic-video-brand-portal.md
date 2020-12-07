---
title: Suporte a vídeo dinâmico no Brand Portal
seo-title: Suporte a vídeo dinâmico no Brand Portal
description: Suporte a vídeo dinâmico no Brand Portal
seo-description: Suporte a vídeo dinâmico no Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b69025074080b83ac699da434fc525fea1cb100a
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 3%

---


# Suporte a vídeo dinâmico no Brand Portal {#dynamic-video-support-on-brand-portal}

Pré-visualização e reproduza vídeos de forma adaptável no Brand Portal com suporte para Dynamic Media. Baixe também as renderizações dinâmicas do portal e dos links compartilhados.
Os usuários do Brand Portal podem:

* Vídeos de pré-visualização na página Detalhes do ativo, Visualização do cartão e página de pré-visualização de compartilhamento de link.
* Reproduzir codificações de vídeo na página Detalhes do ativo.
* Visualização representações dinâmicas na guia Representações na página Detalhes do ativo.
* Baixe as codificações e pastas de vídeo que contêm vídeos.

>[!NOTE]
>
>Para trabalhar com vídeos e publicá-los no Brand Portal, verifique se a instância do autor de AEM está configurada no modo Dynamic Media Hybrid ou no modo Dynamic Media **[!DNL Scene 7]**.

Para pré-visualização, reprodução e download de vídeos, o Brand Portal expõe as duas configurações a seguir aos administradores:

* [Configuração ](#configure-dm-hybrid-settings)
do Dynamic Media HybridSe a instância do autor de AEM estiver sendo executada no modo híbrido de mídia dinâmica.
* [Configuração de  [!DNL Scene 7] ](#configure-dm-scene7-settings)
mídia dinâmicaSe a instância do autor de AEM estiver sendo executada no **[!DNL Scene 7]** modo de mídia dinâmica.
Defina qualquer uma dessas configurações com base nas configurações definidas na instância do autor de AEM com a qual o locatário do Brand Portal é replicado.

>[!NOTE]
>
>Vídeos dinâmicos não são suportados em locatários do Brand Portal configurados com o autor de AEM em execução no modo de execução **[!UICONTROL Scene7Connect]**.

## Como os vídeos dinâmicos são reproduzidos? {#how-are-dynamic-videos-played}

![Codificações de vídeo são obtidas da nuvem](assets/VideoEncodes.png)

Se as configurações do Dynamic Media ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) estiverem configuradas no Brand Portal, as renderizações dinâmicas serão obtidas do servidor **[!DNL Scene 7]**. Portanto, as codificações de vídeo são visualizadas e reproduzidas sem demora e distorcem a qualidade.

Como as codificações de vídeo não são armazenadas no repositório do Brand Portal e são obtidas do servidor **[!DNL Scene 7]**, verifique se as configurações do Dynamic Media na instância do autor de AEM e no Portal de marca são as mesmas.

>[!NOTE]
>
>Os visualizadores de vídeo e as predefinições do visualizador não são suportados no Brand Portal. Os vídeos são visualizados e reproduzidos nos visualizadores padrão no Brand Portal.

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos no Brand Portal, certifique-se de:

* **Start do autor de AEM no**
modo DM (Dynamic Media)Inicie a instância do autor de AEM (com a qual o Portal de marca está configurado) no modo  [Dynamic Media Hybrid ou no ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) modo  [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configure os serviços de nuvem do Dynamic Media no**
AutorCom base no modo de Mídia dinâmica em que o autor de AEM está sendo executado, defina os  [serviços de nuvem do ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Dynamic Media ou os serviços de  [[!DNL Scene 7] nuvem ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) no Autor de AEM em  **Ferramentas** |  **Cloud Services** | Mídia  **** dinâmica.
* **Configure o Dynamic Media no**
Portal de MarcasCom base nas configurações de nuvem do Dynamic Media no Autor de AEM, configure as  [configurações do Dynamic Media ou ](#configure-dm-hybrid-settings)   [[!DNL Scene 7] ](#configure-dm-scene7-settings)  as configurações das ferramentas administrativas do Portal de Marcas.
Certifique-se de que [locatários separados do Brand Portal](#separate-tenants) sejam usados para instâncias do autor de AEM configuradas com os modos Dynamic Media Hybrid e Dynamic Media **[!UICONTROL Scene7]**, se você estiver usando funcionalidades do Dynamic Media Hybrid e Dynamic Media **[!UICONTROL S7]**.
* **Publique pastas com códigos de vídeo aplicados ao Brand**
PortalAplique códigos de  [ ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo e publique a pasta que contém os ativos de mídia avançada da instância do autor de AEM no Brand Portal.
* **lista de permissões IPs de saída no SPS se a pré-visualização segura estiver**
ativadaSe estiver usando o Dynamic Media-**[!DNL Scene 7]** (com pré-visualização  [segura ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) ativada para uma empresa), então é aconselhável que o administrador da  **[!DNL Scene 7]** empresa  [lista de permissões os ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IPs de saída públicos para as respectivas regiões usando a interface flash do SPS (**[!UICONTROL Scene 7]** Publishing System).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63 140 44,54 |

Para permitir a lista de qualquer um desses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Práticas recomendadas    

Para garantir que seus ativos de vídeo dinâmico sejam visualizados, reproduzidos e baixados com êxito do Brand Portal (e links compartilhados), siga estas práticas:

### Locatários separados para modos Dynamic Media Hybrid e Dynamic Media Scene 7 {#separate-tenants}

Se você estiver usando os recursos Dynamic Media **[!DNL Scene 7]** e Dynamic Media Hybrid, recomendamos que use diferentes locatários do Portal de Marcas para instâncias de Autor de AEM configuradas com os modos Dynamic Media Hybrid e Dynamic Media **[!DNL Scene 7]**.<br />

![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Mesmos detalhes de configuração na instância do autor de AEM e no Portal de marcas

Certifique-se de que os detalhes de configuração, como **[!UICONTROL Título]**, **[!UICONTROL ID de registro]**, **[!UICONTROL URL do serviço de vídeo]** (em **[!UICONTROL Dynamic Media Hybrid]**) e **[!UICONTROL Título]**, credenciais (**[!UICONTROL Email&lt;a111/> e Senha),**[!UICONTROL  Região ]**,**[!UICONTROL  Empresa ]**(no Dynamic Media **[!DNL Scene 7]**) são as mesmas no Brand Portal e**[!UICONTROL  AEM configuração da nuvem ]**.]**

### lista de permissões IPs de saída públicos para o modo Dynamic Media Scene 7

Se o Dynamic Media **[!UICONTROL Scene 7]** com [pré-visualização segura ativada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)- for usado para fornecer ativos de vídeo ao Brand Portal, o **[!UICONTROL Scene 7]** criará um servidor de imagem dedicado para ambientes de preparo ou aplicações internas. Qualquer solicitação para este servidor verifica o endereço IP da origem. Se a solicitação recebida não estiver dentro da lista aprovada de endereços IP, uma resposta de falha será retornada.
O **[!UICONTROL Administrador da Empresa Scene-7]** configura uma lista aprovada de endereços IP para o ambiente **[!UICONTROL Teste Seguro]** da empresa, por meio de **[!UICONTROL SPS]** (Scene-7 Publishing System) Flash UI. Certifique-se de que o IP de saída para a sua região (a partir do seguinte) seja adicionado a essa lista aprovada.
Para permitir a lista de qualquer um desses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63 140 44,54 |

## Definir configurações do Dynamic Media (Híbrido) {#configure-dm-hybrid-settings}

Se a instância do autor de AEM estiver sendo executada no modo híbrido de mídia dinâmica, use o bloco **[!UICONTROL Vídeo]** do painel de ferramentas administrativas para definir as configurações do gateway de Mídia dinâmica.

>[!NOTE]
>
>Os [perfis de codificação de vídeo](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) não são publicados no Brand Portal, em vez disso, são obtidos do servidor **[!UICONTROL Scene 7]**. Portanto, para que as codificações de vídeo sejam reproduzidas com êxito no Brand Portal, certifique-se de que os detalhes de configuração sejam os mesmos que [[!UICONTROL configuração de nuvem do Scene7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) na sua instância do autor de AEM.

Para configurar as configurações do Dynamic Media nos locatários do Brand Portal:

1. Selecione o logotipo AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.
1. No painel de ferramentas administrativas, selecione o bloco **[!UICONTROL Vídeo]**.

   ![Configuração do Dynamic Media Hybrid no Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL A página Editar]** configuração de mídia dinâmica é aberta.

   ![Configuração do Dynamic Media Hybrid no Brand Portal](assets/edit-dynamic-media-config.png)

1. Especifique **[!UICONTROL ID de Registro]** e **[!UICONTROL URL do Serviço de Vídeo]** (URL do Gateway DM). Certifique-se de que esses detalhes sejam os mesmos em **[!UICONTROL Ferramentas > Cloud Services]** na instância do autor de AEM.
1. Selecione **Salvar** para salvar a configuração.

## Definir configurações do Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se a instância do autor de AEM estiver sendo executada no modo Dynamic Media- **[!UICONTROL Scene 7]**, use o bloco **[!UICONTROL Configuração de Dynamic Media]** do painel de ferramentas administrativas para definir as configurações do servidor **[!UICONTROL Scene 7]**.

Para configurar as configurações do Dynamic Media **[!UICONTROL Scene 7]** nos locatários do Brand Portal:

1. Selecione o logotipo AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.

2. No painel de ferramentas administrativas, selecione o bloco **[!UICONTROL Configuração de Dynamic Media]**.<br />
   ![Configuração do DM  [!UICONTROL Scene 7] no Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL A página Editar]** configuração de mídia dinâmica é aberta.<br />
   ![Configuração do Scene 7 no Brand Portal](assets/S7Config.png)

3. Fornecer:
   * **[!UICONTROL Título]**
   * Credenciais (**[!UICONTROL E-mail ID]** e **[!UICONTROL Senha]**) para aceder ao servidor Scene 7
   * ****
RegiãoCertifique-se de que esses valores sejam os mesmos da sua instância do autor de AEM.

4. Selecione **[!UICONTROL Ligar ao Dynamic Media]**.

5. Forneça o **[!UICONTROL nome da Empresa]** e **[!UICONTROL Salve]** a configuração.
