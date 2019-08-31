---
title: Suporte de vídeo dinâmico no Brand Portal
seo-title: Suporte de vídeo dinâmico no Brand Portal
description: Suporte de vídeo dinâmico no Brand Portal
seo-description: Suporte de vídeo dinâmico no Brand Portal
uuid: a 3502 a 4 d -3971-4 ea 4-953 c -44 ba 04446269
contentOwner: mgulati
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
topic-tags: download-instalação
discoiquuid: e 18 d 992 a-a 3 b 5-45 f 2-9696-8161993213 ee
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Suporte de vídeo dinâmico no Brand Portal {#dynamic-video-support-on-brand-portal}

Visualize e reproduza vídeos de forma adaptável no Brand Portal com suporte ao Dynamic Media. Baixe também as representações dinâmicas do portal e links compartilhados.
Usuários do Brand Portal podem:

* Visualize vídeos na página Detalhes do ativo, Exibição de cartão e na página de visualização de compartilhamento de link.
* Reproduza códigos de vídeo na página Detalhes do ativo.
* Exiba representações dinâmicas na guia Representações na página Detalhes do ativo.
* Baixe os códigos de vídeo e pastas que contêm vídeos.

>[!NOTE]
>
>Para trabalhar com vídeos e publicá-los no Brand Portal, verifique se sua instância de Autor de AEM está configurada no modo Híbrido de Dynamic Media ou [!DNL Scene 7] no modo Dynamic Media.

Para visualizar, reproduzir e baixar vídeos, o Brand Portal expõe as duas configurações a seguir para administradores:

* [Configuração
híbrida de Dynamic Media](#configure-dm-hybrid-settings)Se a instância do Autor de AEM estiver sendo executada no modo híbrido de mídia dinâmica.
* [Dynamic Media [! Configuração
do DNL Scene 7]](#configure-dm-scene7-settings)Se a instância do Autor de AEM estiver sendo executada no[!DNL Scene 7] modo de mídia dinâmica.
Defina uma dessas configurações com base nas configurações definidas na instância do Autor de AEM com o qual o locatário do Portal de marcas é replicado.

>[!NOTE]
>
>Os vídeos dinâmicos não são suportados nos localizadores do Brand Portal integrados com o autor de AEM em execução no [!UICONTROL modo de execução do Scene 7 Connect] .

## Como são reproduzidos vídeos dinâmicos? {#how-are-dynamic-videos-played}

![Os códigos de vídeo são obtidos da nuvem](assets/VideoEncodes.png)

Se configurações de Dynamic Media ([híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[! Configurações do DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) são configuradas no Brand Portal, as representações dinâmicas são buscadas do [!DNL Scene 7] servidor. Os códigos de vídeo são, portanto, visualizados e reproduzidos sem atrasos e distorção de qualidade.

Como os códigos de vídeo não são armazenados no repositório do Brand Portal e são obtidos do [!DNL Scene 7] servidor, certifique-se de que as configurações de Mídia dinâmica na Instância do autor de AEM e no Portal de marca sejam as mesmas.

>[!NOTE]
>
>Os visualizadores de vídeo e as predefinições do visualizador não são compatíveis com o Brand Portal. Os vídeos são visualizados e reproduzidos nos visualizadores padrão no Brand Portal.

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos no Brand Portal, certifique-se de:

* **Inicie o modo de autor de AEM no modo
DM (Dynamic Media)** inicie a instância de Autor de AEM (com a qual o Brand Portal está integrado) no [modo Dynamic Media híbrido](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) ou [Dynamic Media [! Modo DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configurar os serviços de nuvem de Dynamic Media no autor
de AEM** com base no modo de AEM Author de Dynamic Media está em execução, defina um dos [serviços em nuvem do Dynamic Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) ou [[! Serviços em nuvem do DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) no autor de AEM das **ferramentas** | **Serviços em nuvem** | **Dynamic Media**.
* **Configurar mídia dinâmica no portal
de marca** com base nas configurações de nuvem do Dynamic Media no autor de AEM, configure [as configurações do Dynamic Media](#configure-dm-hybrid-settings) ou [[! Configurações do DNL Scene 7]](#configure-dm-scene7-settings) das ferramentas administrativas do Brand Portal.
Certifique-se de [que os locatários](#separate-tenants) separados do Portal de marcas sejam usados para instâncias de Autor de AEM configuradas com modos de Dynamic Media híbrido e Dynamic Media [!UICONTROL Scene 7] , se você estiver usando funcionalidades de Dynamic Media híbrido e Dynamic Media [!UICONTROL S 7].
* **Publicar pastas com codificação de vídeo aplicada às codificações de vídeo** Aplicar [portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 
e publicar a pasta que contém ativos de mídia avançada da instância de autor de AEM para o Portal de marcas.
* **IPs de hiperist de permissões no SPS se a visualização segura estiver ativada**
se estiver usando o Dynamic Media-[!DNL Scene 7] (com [visualização segura ativada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para uma empresa), então recomenda-se que [!DNL Scene 7] os [usuários de permissões do administrador da empresa sejam compatíveis com os IPs](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) de associados públicos para as respectivas regiões usando o FLS ([!UICONTROL Scene 7] Publishing System).
Os IPs de egress são os seguintes:

| **Região** | **IP de egress** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Para adicionar uma lista de permissões desses IPs de vinculação, consulte [Preparar sua conta para o serviço de teste seguro](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Práticas recomendadas

Para garantir que seus ativos de vídeo dinâmicos sejam visualizados, reproduzidos e baixados do Brand Portal (e links compartilhados), siga estas práticas:

### Separadores separados para modos de Dynamic Media híbrido e Dynamic Media Scene 7 {#separate-tenants}

Se você estiver usando recursos de Dynamic Media [!DNL Scene 7] e Dynamic Media híbrido, recomenda-se que você use diferentes locatários do Brand Portal para instâncias de autor de AEM configuradas com [!DNL Scene 7] modos de Dynamic Media híbrido e Dynamic Media.
![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Mesmos detalhes de configuração na instância do autor de AEM e no Brand Portal

Certifique-se de que os detalhes de configuração, como [!UICONTROL Título], [!UICONTROL ID de registro], [!UICONTROL URL do serviço de vídeo] (em [!UICONTROL Híbrido]de mídia dinâmica) e [!UICONTROL Título], as credenciais ([!UICONTROL Email] e senha), [!UICONTROL Região], [!UICONTROL Empresa] (no Dynamic Media [!DNL Scene 7]) sejam os mesmos no Portal da marca e [!UICONTROL na configuração do AEM Cloud].

### Ipelist public egress IPs for Dynamic Media Scene Mode

Se o Scene Media [!UICONTROL Scene 7]-ter a visualização [segura ativada-](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)é usada para enviar ativos de vídeo para o Brand Portal, o [!UICONTROL Scene 7] estabelece um servidor de imagem dedicado para ambientes de armazenamento temporário ou aplicativos internos. Qualquer solicitação a esse servidor verifica o endereço IP de origem. Se a solicitação de entrada não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada.
O Administrador da empresa [!UICONTROL Scene -7] , portanto, configura uma lista aprovada de endereços IP para o ambiente [!UICONTROL de teste] seguro da sua empresa, por meio [!UICONTROL do SPS] (Scene -7 Publishing System) UI. Certifique-se de que o IP de egã para sua respectiva região (do seguinte) seja adicionado à lista aprovada.
Para adicionar uma lista de permissões desses IPs de vinculação, consulte [Preparar sua conta para o serviço de teste seguro](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Os IPs de egã são os seguintes:

| **Região** | **IP de egress** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configurações de configuração de mídia dinâmica (híbridas) {#configure-dm-hybrid-settings}

Se a instância do Autor de AEM estiver em execução no modo híbrido de mídia dinâmica, use [!UICONTROL o bloco de vídeo] do painel de ferramentas administrativas para configurar as configurações do gateway do Dynamic Media.
>[!NOTE]
>
>Os perfis de codificação [de vídeo](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) não são publicados no Brand Portal, em vez disso, são obtidos do servidor [!UICONTROL Scene 7] . Portanto, para que os códigos de vídeo sejam reproduzidos com sucesso no Brand Portal, certifique-se de que os detalhes de configuração sejam os mesmos do [[! Configuração do UICTROL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) na instância do autor de AEM.
Para configurar configurações de Mídia dinâmica nos inquilinos do Brand Portal:

1. Selecione o logotipo do AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Portal da marca.

2. No painel de ferramentas administrativas, selecione o **[!UICONTROL bloco Vídeo]** .

![Configuração híbrida de mídia dinâmica no portal da marca](assets/DMHybrid-Video.png)

**[!UICONTROL A página Editar configuração]** de mídia dinâmica é aberta.

![Configuração híbrida de mídia dinâmica no Brand Portal](assets/edit-dynamic-media-config.png)

3. Especifique **[!UICONTROL a ID de registro]** e **[!UICONTROL o URL do serviço de vídeo]** (URL do DM-Gateway). Certifique-se de que esses detalhes sejam os mesmos em **[!UICONTROL Ferramentas &gt; Serviços em nuvem]** na sua instância do Autor de AEM.

4. Selecione **Salvar** para salvar a configuração.

## Configuração das configurações do Dynamic Media Scene 7 {#configure-dm-scene7-settings}

Se a instância do Autor de AEM estiver sendo executada no modo Dynamic Media- [!UICONTROL Scene 7] , use **[!UICONTROL o bloco de Configuração]** de mídia dinâmica no painel de ferramentas administrativas para configurar as configurações do servidor [!UICONTROL Scene 7] .

Para configurar configurações do Dynamic Media [!UICONTROL Scene 7] nos inquilinos do Brand Portal:

1. Selecione o logotipo do AEM para acessar as ferramentas administrativas na barra de ferramentas na parte superior, no Portal da marca.

2. No painel de ferramentas administrativas, selecione o **[!UICONTROL quadro Configuração]** de mídia dinâmica.
   ![Configuração do DM [!UICONTROL Scene 7] no Brand Portal](assets/DMS7-Tile.png)

[!UICONTROL A página Editar configuração] de mídia dinâmica é aberta.

![Configuração do Scene 7 no Brand Portal](assets/S7Config.png)

3. Forneça:
   * [!UICONTROL Título]
   * Credenciais ([!UICONTROL ID] e [!UICONTROL senha de email]) para acessar o servidor Scene 7
   * [!UICONTROL Região]
Certifique-se de que esses valores sejam os mesmos da sua instância de Autor de AEM.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Forneça o nome **[!UICONTROL da Empresa]** e **[!UICONTROL Salve]** a configuração.
