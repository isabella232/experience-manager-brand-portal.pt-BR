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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Suporte de vídeo dinâmico no Brand Portal {#dynamic-video-support-on-brand-portal}

Visualize e reproduza vídeos de forma adaptável com [!DNL Brand Portal] o suporte de Mídia dinâmica. Baixe também as representações dinâmicas do portal e links compartilhados.
[!DNL Brand Portal] os usuários podem:

* Visualize vídeos na página Detalhes do ativo, Exibição de cartão e na página de visualização de compartilhamento de link.
* Reproduza códigos de vídeo na página Detalhes do ativo.
* Exiba representações dinâmicas na guia Representações na página Detalhes do ativo.
* Baixe os códigos de vídeo e pastas que contêm vídeos.

>[!NOTE]
>
>Para trabalhar com vídeos e publicá-los, [!DNL Brand Portal]verifique se a instância [!DNL AEM] do Autor está configurada no modo Híbrido de Dynamic Media ou [!DNL Scene 7] no modo Dynamic Media.

Para visualizar, reproduzir e baixar vídeos, [!DNL Brand Portal] expõe as duas configurações a seguir para administradores:

* [Configuração
de Dynamic Media híbrida](#configure-dm-hybrid-settings)se a instância [!DNL AEM] do Autor estiver sendo executada no modo Híbrido de mídia dinâmica.
* [Dynamic Media [! Configuração
do DNL Scene 7]](#configure-dm-scene7-settings)se [!DNL AEM] a instância do Autor estiver sendo executada no[!DNL Scene 7] modo de mídia dinâmica.
Defina uma dessas configurações com base nas configurações definidas na instância [!DNL AEM] do Autor com o [!DNL Brand Portal] qual o locatário é replicado.

>[!NOTE]
>
>Os vídeos dinâmicos não são suportados nos [!DNL Brand Portal] inquilinos integrados com [!DNL AEM] o Autor em execução no [!UICONTROL modo de execução do Scene 7 Connect] .

## Como são reproduzidos vídeos dinâmicos? {#how-are-dynamic-videos-played}

![Os códigos de vídeo são obtidos da nuvem](assets/VideoEncodes.png)

Se configurações de Dynamic Media ([híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[! Configurações do DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) são configuradas [!DNL Brand Portal], as representações dinâmicas são buscadas do [!DNL Scene 7] servidor. Os códigos de vídeo são, portanto, visualizados e reproduzidos sem atrasos e distorção de qualidade.

Como os códigos de vídeo não são armazenados no [!DNL Brand Portal] repositório e são obtidos do [!DNL Scene 7] servidor, certifique-se de que as configurações de Dynamic Media na [!DNL AEM] instância do autor sejam [!DNL Brand Portal] as mesmas.

>[!NOTE]
>
>Não há suporte para visualizadores de vídeo e predefinições do visualizador [!DNL Brand Portal]. Os vídeos são visualizados e reproduzidos nos visualizadores padrão.[!DNL Brand Portal]

## Pré-requisitos {#prerequisites}

Para trabalhar com vídeos dinâmicos ativados [!DNL Brand Portal], certifique-se de:

* **Inicie[!DNL AEM]o autor no modo
DM (Dynamic Media)** inicie a [!DNL AEM] instância Autor (com [!DNL Brand Portal] a qual está integrado) no [modo Dynamic Media híbrido](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) ou [Dynamic Media [! Modo DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configurar os serviços de nuvem do Dynamic Media no[!DNL AEM]Autor**
com base no modo [!DNL AEM] de Autor de mídia dinâmica que está sendo criado, defina um dos [serviços em nuvem do Dynamic Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) ou [[! Serviços em nuvem do DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) em [!DNL AEM] Autor a partir **de ferramentas** | **Serviços em nuvem** | **Dynamic Media**.
* **Configurar mídia dinâmica no portal
de marca** com base nas configurações de nuvem do Dynamic Media no [!DNL AEM] autor, configurar [configurações de Dynamic Media](#configure-dm-hybrid-settings) ou [[! Configurações do DNL Scene 7]](#configure-dm-scene7-settings) de [!DNL Brand Portal] ferramentas administrativas.
Certifique-se [de que [! Os localizadores](#separate-tenants) do DNL Brand Portal] são usados para [!DNL AEM] instâncias do Autor configuradas com modos de Dynamic Media híbrido e Dynamic Media [!UICONTROL Scene 7] , se você estiver usando funcionalidades de Dynamic Media Híbrido e Dynamic Media [!UICONTROL S 7].
* **Publicar pastas com codificação de vídeo aplicada às codificações de vídeo** Aplicar [portal
de marca](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) e publicar a pasta que contém ativos de mídia avançada da [!DNL AEM] instância do Autor.[!DNL Brand Portal]
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

Para garantir que seus ativos de vídeo dinâmicos sejam visualizados com êxito, reproduzidos e baixados [!DNL Brand Portal] de (e links compartilhados), siga estas práticas:

### Separadores separados para modos de Dynamic Media híbrido e Dynamic Media Scene 7 {#separate-tenants}

Se você estiver usando recursos de Dynamic Media [!DNL Scene 7] e Dynamic Media híbrido, recomenda-se que você use [!DNL Brand Portal] diferentes locatários para [!DNL AEM] instâncias do Autor configuradas com modos de Mídia dinâmica e Mídia [!DNL Scene 7] dinâmica.
![Autor e BP um para um mapeamento](assets/BPDynamicMedia.png)

### Mesmos detalhes de configuração na instância do autor de AEM e no Brand Portal

Certifique-se de que os detalhes de configuração, como Título, ID de registro, URL do serviço de vídeo (em Híbrido de mídia dinâmica) e Título, as credenciais (Email e senha), Região, Empresa (no Dynamic Media [!DNL Scene 7]) sejam a mesma na configuração [!DNL Brand Portal] e [!DNL AEM] na configuração da nuvem.

### Ipelist public egress IPs for Dynamic Media Scene Mode

Se o Scene Media Scene 7-com visualização [segura ativada-](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)é usado para servir ativos de vídeo para [!DNL Brand Portal], o Scene 7 estabelece um Servidor de imagens dedicado para ambientes de armazenamento temporário ou aplicativos internos. Qualquer solicitação a esse servidor verifica o endereço IP de origem. Se a solicitação de entrada não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada.
O Administrador da empresa Scene -7, portanto, configura uma lista aprovada de endereços IP para o ambiente de teste seguro da sua empresa, por meio do SPS (Scene -7 Publishing System) UI. Certifique-se de que o IP de egã para sua respectiva região (do seguinte) seja adicionado à lista aprovada.
Para adicionar uma lista de permissões desses IPs de vinculação, consulte [Preparar sua conta para o serviço de teste seguro](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Os IPs de egã são os seguintes:

| **Região** | **IP de egress** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configurações de configuração de mídia dinâmica (híbridas) {#configure-dm-hybrid-settings}

Se [!DNL AEM] a instância do Autor estiver em execução no modo híbrido de mídia dinâmica, use o bloco de vídeo em painel de ferramentas administrativas para configurar as configurações do gateway do Dynamic Media.
>[!NOTE]
>
>Os [perfis](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) de codificação de vídeo não são publicados [!DNL Brand Portal], em vez disso, são obtidos do servidor Scene 7. Portanto, para que os códigos de vídeo sejam reproduzidos com êxito, [!DNL Brand Portal]certifique-se de que os detalhes de configuração sejam iguais à configuração do cloud [Scene 7](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) na instância [!DNL AEM] do Autor.
Para configurar configurações de Dynamic Media em [!DNL Brand Portal] inquilinos:

1. Selecione o [!DNL AEM] logotipo para acessar as ferramentas administrativas na barra de ferramentas na parte superior, em [!DNL Brand Portal].

2. No painel de ferramentas administrativas, selecione o **bloco Vídeo** .
   ![Configuração híbrida de mídia dinâmica no portal da marca](assets/DMHybrid-Video.png)
   **A página Editar configuração** de mídia dinâmica é aberta.
   ![Configuração híbrida de mídia dinâmica no Brand Portal](assets/edit-dynamic-media-config.png)

3. Especifique **a ID de registro** e **o URL do serviço de vídeo** (URL do DM-Gateway). Certifique-se de que esses detalhes sejam os mesmos em **Ferramentas** &gt; **Serviços em nuvem** na sua instância [!DNL AEM] do Autor.

4. Selecione **Salvar** para salvar a configuração.

## Configuração das configurações do Dynamic Media Scene 7 {#configure-dm-scene7-settings}

Se [!DNL AEM] a instância do Autor estiver sendo executada no modo Dynamic Media- [!UICONTROL Scene 7] , use **o bloco de Configuração** de mídia dinâmica no painel de ferramentas administrativas para configurar as configurações do servidor [!UICONTROL Scene 7] .

Para configurar configurações do Dynamic Media [!UICONTROL Scene 7] em [!DNL Brand Portal] inquilinos:

1. Selecione o [!DNL AEM] logotipo para acessar as ferramentas administrativas na barra de ferramentas na parte superior, em [!DNL Brand Portal].

2. No painel de ferramentas administrativas, selecione o **quadro Configuração** de mídia dinâmica.
   ![A configuração do DM Scene 7 na [!DNL Brand Portal]](assets/DMS7-Tile.png)página Editar configuração de mídia dinâmica é aberta.
   ![Configuração do Scene 7 em [!DNL Brand Portal]](assets/S7Config.png)

3. Forneça:
   * Título
   * Credenciais (ID e senha de email) para acessar o servidor Scene 7
   * Região
Certifique-se de que esses valores sejam iguais aos da sua instância [!DNL AEM] do Autor.

4. Select **Connect to Dynamic Media**.

5. Forneça o nome **da Empresa** e **Salve** a configuração.
