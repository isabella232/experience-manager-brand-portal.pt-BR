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
source-git-commit: 7128c71576ae938a49f9bff0b95b98b7fc480f69
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 3%

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
>Para trabalhar com vídeos e publicá-los no Brand Portal, verifique se a instância do autor do Experience Manager está configurada no modo Dynamic Media Hybrid ou no Dynamic Media **[!DNL Scene7]** modo.

Para visualizar, reproduzir e baixar vídeos, o Brand Portal expõe as duas configurações a seguir para os administradores:

* [Configuração híbrida do Dynamic Media](#configure-dm-hybrid-settings)
Se a instância Experience Manager Author estiver em execução no modo Híbrido do Dynamic Media.
* [Dynamic Media [!DNL Scene7] configuração](#configure-dm-scene7-settings)
Se a instância Experience Manager Author estiver em execução no dynamic media-**[!DNL Scene7]** modo.
Defina qualquer uma dessas configurações com base nas configurações definidas na instância do Autor do Experience Manager com a qual o locatário do Brand Portal é replicado.

>[!NOTE]
>
>Vídeos dinâmicos não são compatíveis com locatários do Brand Portal configurados com Autor do Experience Manager em execução em **[!UICONTROL Scene7Connect]** modo de execução.

## Como os vídeos dinâmicos são reproduzidos? {#how-are-dynamic-videos-played}

![Os códigos de vídeo são obtidos da nuvem](assets/VideoEncodes.png)

Se as configurações do Dynamic Media ([Híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurações) estiverem configuradas no Brand Portal, as representações dinâmicas serão buscadas do **[!DNL Scene7]** servidor. Os códigos de vídeo são, portanto, pré-visualizados e reproduzidos sem demora e distorcem a qualidade.

Como as codificações de vídeo não são armazenadas no repositório Brand Portal e são buscadas no **[!DNL Scene7]** verifique se as configurações do Dynamic Media na Instância do autor do Adobe Experience Manager e no Brand Portal são as mesmas.

>[!NOTE]
>
>Visualizadores de vídeo e predefinições do visualizador não são compatíveis com o Brand Portal. Os vídeos são visualizados e reproduzidos nos visualizadores padrão do Brand Portal.

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos no Brand Portal, certifique-se de:

* **Inicie o Experience Manager Author no modo Dynamic Media**
Inicie a instância Experience Manager Author (com a qual o Brand Portal está configurado) em [Dynamic Media - [!DNL Scene7] modo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) ou [Dynamic Media - Modo híbrido](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) ou
* **Configurar o Dynamic Media Cloud Services no Experience Manager Author**
Com base no modo Dynamic Media (modo Scene7 ou modo Híbrido), o autor do Experience Manager está em execução, defina [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) ou [Dynamic Media Cloud Services (Modo híbrido)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) no Autor do Experience Manager de **Ferramentas** | **Cloud Services** | **Dynamic Media**.
* **Configurar o Dynamic Media no Brand Portal**
Com base nas configurações de nuvem do Dynamic Media no Experience Manager Author, configure [Configurações do Dynamic Media](#configure-dm-hybrid-settings) ou [[!DNL Scene7] configurações](#configure-dm-scene7-settings)  das ferramentas administrativas do Brand Portal.
Certifique-se de que [locatários Brand Portal separados](#separate-tenants) são usadas para instâncias de Autor do Experience Manager configuradas no Dynamic Media - **[!UICONTROL Scene7]** mode e Dynamic Media - Modo híbrido. Especialmente se você usar funcionalidades do Dynamic Media **[!UICONTROL S7]** e Dynamic Media Hybrid.
* **Publicar pastas com códigos de vídeo aplicados ao Brand Portal**
Aplicar [codificações de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) e publique a pasta que contém ativos de mídia avançada da instância do Experience Manager Author para o Brand Portal.
* **lista de permissões IPs de saída no SPS se a visualização segura estiver ativada**
Se estiver usando o Dynamic Media-**[!DNL Scene7]** com [visualização segura ativada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para uma empresa), recomenda-se que **[!DNL Scene7]** administrador da empresa [lista de permissões os IPs de saída públicos](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) para as respectivas regiões que utilizam SPS (**[!UICONTROL Scene7]** Interface do usuário flash do sistema de publicação).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.68, 20.94.203.130 |
| EMEA | 185.34.189.3, 51.132.146.75 |
| APAC | 63 140 44,54 |

Para adicionar uma lista de permissões a esses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Práticas recomendadas    

Para garantir que seus ativos de vídeo dinâmico sejam visualizados, reproduzidos e baixados com êxito do Brand Portal (e links compartilhados), siga estas práticas:

### Locatários separados para Dynamic Media - Scene7 e Dynamic Media - Modos híbridos {#separate-tenants}

Se você usar a Dynamic Media - **[!DNL Scene7]** modo e Dynamic Media - recursos do modo híbrido, use diferentes locatários do Brand Portal para instâncias de Autor do Experience Manager configuradas com o Dynamic Media - **[!DNL Scene7]** e Dynamic Media - Modos híbridos.


![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Os mesmos detalhes de configuração na instância Experience Manager Author e no Brand Portal

Verifique se os detalhes da configuração são os mesmos no Brand Portal e **[!UICONTROL Configuração da nuvem do Experience Manager]**. Os mesmos detalhes de configuração incluem:

* **[!UICONTROL Título]**
* **[!UICONTROL ID de registro]**
* **[!UICONTROL URL do serviço de vídeo]** em **[!UICONTROL Dynamic Media - Modo híbrido]**
* **[!UICONTROL Título]**
* Credenciais (**[!UICONTROL Email]** e Senha)
* **[!UICONTROL Região]**
* **[!UICONTROL Empresa]** no Dynamic Media - **[!DNL Scene7]** modo

### lista de permissões IPs de saída públicos para o modo Dynamic Media Scene7

Se o Dynamic Media **[!UICONTROL Scene7]**- ter [visualização segura ativada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-é usado para fornecer ativos de vídeo ao Brand Portal, em seguida **[!UICONTROL Scene7]** O estabelece um servidor de imagem dedicado para ambientes de preparo ou aplicativos internos. Qualquer solicitação para este servidor verifica o endereço IP de origem. Se a solicitação recebida não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada.
O **[!UICONTROL Scene7]** Portanto, o Administrador da empresa configura uma lista aprovada de endereços IP para o **[!UICONTROL Teste seguro]** ambiente, através **[!UICONTROL SPS]** Interface do usuário flash do (Scene7 Publishing System). Certifique-se de que o IP de saída da respectiva região (a partir do seguinte) seja adicionado a essa lista aprovada.
Para adicionar uma lista de permissões a esses IPs de saída, consulte [preparar sua conta para o serviço de teste seguro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Os IPs de saída são os seguintes:

| **Região** | **IP de saída** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189,1 |
| APAC | 63 140 44,54 |

## Definir configurações do Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Se a instância Autor do Experience Manager estiver em execução no modo híbrido do dynamic media, use **[!UICONTROL Vídeo]** mosaico do painel de ferramentas administrativas para definir as configurações do gateway do Dynamic Media.

>[!NOTE]
>
>O [perfis de codificação de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) não são publicados no Brand Portal, em vez disso, são obtidos do **[!UICONTROL Scene7]** servidor. Portanto, para que os códigos de vídeo sejam reproduzidos com êxito no Brand Portal, verifique se os detalhes de configuração são iguais ao cenário [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) na instância Experience Manager Author.

Para configurar configurações do Dynamic Media em locatários do Brand Portal:

1. Selecione o logotipo do Experience Manager para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.
1. No painel Ferramentas administrativas , selecione o **[!UICONTROL Vídeo]** mosaico.

   ![Configuração híbrida do Dynamic Media no Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Editar configuração do Dynamic Media]** será aberta.

   ![Configuração híbrida do Dynamic Media no Brand Portal](assets/edit-dynamic-media-config.png)

1. Especificar **[!UICONTROL ID de registro]** e **[!UICONTROL URL do serviço de vídeo]** (URL do gateway DM). Certifique-se de que esses detalhes sejam iguais aos desses detalhes em **[!UICONTROL Ferramentas > Cloud Services]** na instância Experience Manager Author.
1. Selecionar **Salvar** para salvar a configuração.

## Definir configurações do Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se a instância do autor do Experience Manager estiver em execução no Dynamic Media- **[!UICONTROL Scene7]** , em seguida, use **[!UICONTROL Configuração do Dynamic Media]** bloco do painel de ferramentas administrativas para configurar o **[!UICONTROL Scene7]** configurações do servidor.

Para configurar o Dynamic Media **[!UICONTROL Scene7]** configurações em locatários da Brand Portal:

1. Selecione o logotipo do Experience Manager para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Brand Portal.

2. No painel Ferramentas administrativas , selecione o **[!UICONTROL Configuração do Dynamic Media]** mosaico.

   ![DM [!UICONTROL Cena 7] configuração no Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Editar configuração do Dynamic Media]** será aberta.

   ![Configuração do Scene7 no Brand Portal](assets/S7Config.png)

3. Fornecer:

   * **[!UICONTROL Título]**
   * Credenciais (**[!UICONTROL ID de email]** e **[!UICONTROL Senha]**) para acessar o servidor do Scene7
   * **[!UICONTROL Região]**

   Certifique-se de que esses valores sejam os mesmos encontrados na instância do Experience Manager Author.

4. Selecionar **[!UICONTROL Conectar-se ao Dynamic Media]**.

5. Forneça a **[!UICONTROL Nome da empresa]** e **[!UICONTROL Salvar]** a configuração.
