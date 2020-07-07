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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 3%

---


# Suporte a vídeo dinâmico no Brand Portal {#dynamic-video-support-on-brand-portal}

Pré-visualização e reproduza vídeos de forma adaptável no Brand Portal com suporte para Dynamic Media. Baixe também as renderizações dinâmicas do portal e dos links compartilhados.
Os usuários do Brand Portal podem:

* Vídeos de Pré-visualização na página Detalhes do ativo, Visualização do cartão e página de pré-visualização de compartilhamento de link.
* Reproduzir codificações de vídeo na página Detalhes do ativo.
* Visualização representações dinâmicas na guia Representações na página Detalhes do ativo.
* Baixe as codificações e pastas de vídeo que contêm vídeos.

>[!NOTE]
>
>Para trabalhar com vídeos e publicá-los no Brand Portal, certifique-se de que sua instância do AEM Author esteja configurada no modo Dynamic Media Hybrid ou no modo Dynamic Media **[!DNL Scene 7]** .

Para pré-visualização, reprodução e download de vídeos, o Brand Portal expõe as duas configurações a seguir aos administradores:

* [Configuração](#configure-dm-hybrid-settings)do Dynamic Media Hybrid Se a instância do AEM Author estiver sendo executada no modo híbrido de mídia dinâmica.
* [Dynamic [!DNL Scene 7] Mediaconfiguration](#configure-dm-scene7-settings)Se a instância AEM Author estiver sendo executada no modo de mídia dinâmica **[!DNL Scene 7]** .
Defina qualquer uma dessas configurações com base nas configurações definidas na instância AEM Author com a qual o locatário do Brand Portal é replicado.

>[!NOTE]
>
>Vídeos dinâmicos não são suportados em locatários do Brand Portal configurados com AEM Author em execução no modo de execução **[!UICONTROL Scene7Connect]** .

## Como os vídeos dinâmicos são reproduzidos? {#how-are-dynamic-videos-played}

![Codificações de vídeo são obtidas da nuvem](assets/VideoEncodes.png)

Se as configurações do Dynamic Media (configurações[Híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) ) estiverem configuradas no Brand Portal, as renderizações dinâmicas serão obtidas do **[!DNL Scene 7]** servidor. Portanto, as codificações de vídeo são visualizadas e reproduzidas sem demora e distorcem a qualidade.

Como as codificações de vídeo não são armazenadas no repositório do Brand Portal e são obtidas do **[!DNL Scene 7]** servidor, verifique se as configurações da Dynamic Media no AEM Author Instance e no Brand Portal são as mesmas.

>[!NOTE]
>
>Os visualizadores de vídeo e as predefinições do visualizador não são suportados no Brand Portal. Os vídeos são visualizados e reproduzidos nos visualizadores padrão no Brand Portal.

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos no Brand Portal, certifique-se de:

* **Start no modo** DM (Dynamic Media) AEM Author Start para cima na instância AEM Author (com a qual o Portal de marca está configurado) no modo [](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic Media Hybrid ou [Dynamic [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configurar os serviços em nuvem da Dynamic Media no AEM Author** Com base no AEM Author de modo Dynamic Media em execução, defina os serviços [em nuvem da](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Dynamic Media ou os serviços [[!DNL Scene 7] em](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) nuvem no AEM Author **Ferramentas** | **Cloud Service** | **Dynamic Media**.
* **Configure o Dynamic Media no Brand Portal** Com base nas configurações de nuvem do Dynamic Media no AEM Author, defina as configurações [do](#configure-dm-hybrid-settings) Dynamic Media ou [[!DNL Scene 7] as configurações](#configure-dm-scene7-settings) das ferramentas administrativas do Brand Portal.
Certifique-se de que locatários [separados do Brand Portal sejam usados para instâncias de AEM Author configuradas com os modos Dynamic Media Hybrid e Dynamic Media](#separate-tenants) Scene7 **[!UICONTROL , se você estiver usando funcionalidades do Dynamic Media Hybrid e do Dynamic Media]** S7 ****.
* **Publique pastas com codificações de vídeo aplicadas ao Brand Portal** Aplique codificações [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo e publique a pasta que contém os ativos de mídia avançada da instância AEM Author para o Brand Portal.
* **Lista de permissões IPs de saída na SPS se a pré-visualização segura estiver ativada** Se estiver usando o Dynamic Media-**[!DNL Scene 7]** (com pré-visualização [segura ativada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para uma empresa), é aconselhável que o administrador da **[!DNL Scene 7]** empresa [lista de permissões os IPs](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) de saída públicos para as respectivas regiões usando a interface flash do SPS (**[!UICONTROL Scene 7]** Publishing System).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Para permitir a lista desses IPs de saída, consulte [preparar sua conta para o serviço](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)de teste seguro.

## Práticas recomendadas   

Para garantir que seus ativos de vídeo dinâmico sejam visualizados, reproduzidos e baixados com êxito do Brand Portal (e links compartilhados), siga estas práticas:

### Locatários separados para os modos Dynamic Media Hybrid e Dynamic Media Scene 7 {#separate-tenants}

Se você estiver usando os recursos Dynamic Media **[!DNL Scene 7]** e Dynamic Media Hybrid, recomendamos que use diferentes locatários do Portal de marca para instâncias AEM Author configuradas com os modos Dynamic Media Hybrid e Dynamic Media **[!DNL Scene 7]** .<br />

![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Mesmos detalhes de configuração na instância do AEM Author e no Portal da Marca

Certifique-se de que os detalhes de configuração, como **[!UICONTROL Título]**, ID **** de registro, URL **[!UICONTROL do serviço]** de vídeo (no **[!UICONTROL Dynamic Media Hybrid]**) e **[!UICONTROL Título]****** ******** **[!DNL Scene 7]******, credenciais (Email e Senha), Region, Empresa (no Dynamic Media), sejam os mesmos na configuração em e Portal e na configuração em nuvem do AEM.

### Lista de permissões IPs de saída públicos para o modo Dynamic Media Scene 7

Se o Dynamic Media **[!UICONTROL Scene 7]** com pré-visualização [segura ativada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)for usado para fornecer recursos de vídeo ao Brand Portal, o **[!UICONTROL Scene 7]** criará um servidor de imagem dedicado para ambientes de preparo ou aplicativos internos. Qualquer solicitação a este servidor verifica o endereço IP da origem. Se a solicitação recebida não estiver dentro da lista aprovada de endereços IP, uma resposta de falha será retornada.
Portanto, o administrador da Empresa **[!UICONTROL Scene-7]** configura uma lista aprovada de endereços IP para o ambiente de teste **** seguro da empresa, por meio da interface flash do **[!UICONTROL SPS]** (Scene-7 Publishing System). Certifique-se de que o IP de saída para a sua região (a partir do seguinte) seja adicionado a essa lista aprovada.
Para permitir a lista desses IPs de saída, consulte [preparar sua conta para o serviço](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)de teste seguro.
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Definir configurações do Dynamic Media (Híbrido) {#configure-dm-hybrid-settings}

Se a instância AEM Author estiver sendo executada no modo híbrido de mídia dinâmica, use o bloco **[!UICONTROL Vídeo]** do painel de ferramentas administrativas para definir as configurações do gateway Dynamic Media.

>[!NOTE]
>
>Os perfis [de codificação de](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo não são publicados no Brand Portal, em vez disso, são obtidos do servidor **[!UICONTROL Scene 7]** . Portanto, para que as codificações de vídeo sejam reproduzidas com êxito no Brand Portal, certifique-se de que os detalhes de configuração sejam os mesmos da configuração [[!UICONTROL da nuvem do]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Scene7 na instância do AEM Author.

Para configurar as configurações do Dynamic Media nos locatários do Brand Portal:

1. Selecione o logotipo do AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.
1. No painel de ferramentas administrativas, selecione o bloco **[!UICONTROL Vídeo]** .

   ![Configuração híbrida Dynamic Media no Portal de marcas](assets/DMHybrid-Video.png)

   **[!UICONTROL Será aberta a página Editar configuração]** do Dynamic Media.

   ![Configuração híbrida da Dynamic Media no Portal de marcas](assets/edit-dynamic-media-config.png)

1. Especifique a ID **[!UICONTROL de]** registro e o URL **[!UICONTROL do serviço de]** vídeo (URL do Gateway DM). Certifique-se de que esses detalhes sejam os mesmos em **[!UICONTROL Ferramentas > Cloud Service]** na instância do AEM Author.
1. Selecione **Salvar** para salvar a configuração.

## Definir configurações do Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se a instância AEM Author estiver sendo executada no modo Dynamic Media- **[!UICONTROL Scene 7]** , use o bloco gráfico Configuração **** Dynamic Media do painel de ferramentas administrativas para definir as configurações do servidor **[!UICONTROL Scene 7]** .

Para configurar as configurações do Dynamic Media **[!UICONTROL Scene 7]** nos locatários do Brand Portal:

1. Selecione o logotipo do AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.

2. No painel de ferramentas administrativas, selecione o bloco Configuração **** Dynamic Media.<br />
   ![Configuração do DM [!UICONTROL Scene 7] no Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Será aberta a página Editar configuração]** do Dynamic Media.<br />
   ![Configuração do Scene 7 no Brand Portal](assets/S7Config.png)

3. Fornecer:
   * **[!UICONTROL Título]**
   * Credenciais (ID **[!UICONTROL de]** email e **[!UICONTROL senha]**) para acessar o servidor Scene 7
   * **[!UICONTROL Região]** Certifique-se de que esses valores sejam os mesmos da sua instância de AEM Author.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Forneça o nome **[!UICONTROL da]** Empresa e **[!UICONTROL Salve]** a configuração.
