---
title: Baixar ativos
seo-title: Baixar ativos
description: Todos os usuários podem baixar simultaneamente vários ativos e pastas acessíveis a eles. Dessa forma, os ativos aprovados da marca podem ser distribuídos com segurança para uso offline.
seo-description: Todos os usuários podem baixar simultaneamente vários ativos e pastas acessíveis a eles. Dessa forma, os ativos aprovados da marca podem ser distribuídos com segurança para uso offline.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 2%

---


# Baixar ativos {#download-assets}

Todos os usuários podem baixar simultaneamente vários ativos e pastas acessíveis a eles no Portal de marcas. Dessa forma, os ativos aprovados da marca podem ser distribuídos com segurança para uso offline. Leia para saber como baixar os ativos aprovados no Brand Portal e o que esperar do desempenho [do](../using/brand-portal-download-users.md#main-pars-header)download.

>[!NOTE]
>
>Somente administradores podem baixar ativos expirados. Para obter mais informações sobre ativos expirados, consulte [Gerenciar direitos digitais de ativos](../using/manage-digital-rights-of-assets.md).

## Etapas para baixar ativos {#steps-to-download-assets}

Para baixar ativos ou pastas que contêm ativos para o Brand Portal, siga estas etapas:

1. Na interface do Brand Portal, execute um dos procedimentos a seguir:

   * Selecione as pastas ou os ativos que deseja baixar. Na barra de ferramentas na parte superior, clique no ícone **[!UICONTROL Download]** .

   ![](assets/downloadassets-1.png)

   * Para baixar uma única pasta ou um ativo, passe o ponteiro sobre a pasta ou o ativo. Nas miniaturas de ação rápida disponíveis, clique no ícone **[!UICONTROL Download]** .

   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Se os ativos que você está baixando também incluírem ativos licenciados, você será redirecionado para a página Gerenciamento **[!UICONTROL de]** direitos autorais. Nesta página, selecione os ativos, clique em **[!UICONTROL Concordar]** e, em seguida, clique em **[!UICONTROL Download]**. Se você optar por discordar, os ativos licenciados não serão baixados.\
   >Os ativos protegidos por licença têm o contrato de [licença anexado](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) a eles, o que é feito ao configurar a propriedade [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadados do ativo no AEM Assets.

   ![](assets/licensed-asset-download-1.png)

   A caixa de diálogo **[!UICONTROL Download]** é exibida com a opção **[!UICONTROL Ativo(s)]** selecionada por padrão.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >Se os ativos que você está baixando forem arquivos de imagem, e você selecionar somente a opção **[!UICONTROL Ativo(s)]** na caixa de diálogo Download, mas não forem [autorizados pelo administrador a ter acesso às representações originais dos arquivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) de imagem, nenhum arquivo de imagem será baixado e um Aviso solicitará que você tenha sido restringido pelo administrador a acessar as representações originais.

   ![](assets/restrictaccess-note.png)

1. Para baixar as representações de ativos além dos ativos, selecione **[!UICONTROL Representações]**. No entanto, para permitir que execuções geradas automaticamente sejam baixadas juntamente com representações personalizadas, desmarque a opção **[!UICONTROL Excluir representações]** geradas automaticamente, que está selecionada por padrão.

   ![](assets/exclude-auto-renditions.png)

   Para baixar somente as representações, desmarque **[!UICONTROL Ativo(s)]**.

   >[!NOTE]
   >
   >Por padrão, somente os ativos são baixados. No entanto, as representações originais dos arquivos de imagem não serão baixadas se você não estiver [autorizado pelo administrador a ter acesso às representações originais dos arquivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)de imagem.

   * Para acelerar o download de arquivos de ativos do Brand Portal, selecione **[!UICONTROL Ativar aceleração]** de download e [siga o assistente](../using/accelerated-download.md#main-pars-header-405749062). Para saber mais sobre o download mais rápido de recursos, consulte o [guia para acelerar os downloads do Brand Portal](../using/accelerated-download.md).

   * Para aplicar uma predefinição de imagem [personalizada ao ativo e suas representações](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), selecione Representações **[!UICONTROL dinâmicas]**. Especifique propriedades predefinidas de imagens personalizadas (tamanho, formato, espaço de cores, resolução e modificador de imagens) para aplicar a predefinição de imagens personalizadas ao baixar o ativo e suas representações. Para baixar somente as representações dinâmicas, selecione **[!UICONTROL Ativo(s)]**.

   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >Para pré-visualização (ou download) de representações dinâmicas de qualquer ativo, verifique se a mídia dinâmica está ativada e se a representação temporária do ativo em Pirâmide existe na instância do autor de AEM, de onde os ativos foram publicados. Quando um ativo é publicado no Brand Portal, sua representação em pirâmide também é publicada. Não há como gerar a execução de tiff em Pirâmide a partir do Portal de Marcas.

   * Para preservar a hierarquia de pastas do Brand Portal ao baixar ativos, selecione **[!UICONTROL Criar pasta separada para cada ativo]**. Por padrão, a hierarquia de pastas do Brand Portal é ignorada e todos os ativos são baixados em uma pasta no sistema local.

   * Para enviar uma notificação por email aos usuários com um link para baixar os ativos, selecione **[!UICONTROL Enviar por email]**.

   ![](assets/download-link.png)

   >[!NOTE]
   >
   >O link de download na notificação por email expira após 45 dias.
   >
   >Os administradores podem personalizar mensagens de email, isto é, logotipo, descrição e rodapé, usando o recurso [Marca](../using/brand-portal-branding.md) .

1. Clique em **[!UICONTROL Download]**.

   Os ativos (e as representações, se selecionadas) são baixados como um arquivo ZIP para a pasta local. No entanto, nenhum arquivo zip será criado se um único ativo for baixado sem nenhuma das representações, garantindo assim um download rápido.

   As representações originais dos ativos selecionados não são baixadas se você não estiver [autorizado pelo administrador a ter acesso às representações](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)originais.

   >[!NOTE]
   >
   >Os ativos selecionados individualmente e baixados ficam visíveis no relatório de ativos baixados. No entanto, se uma pasta que contém ativos for baixada, nem a pasta nem os ativos serão exibidos no relatório de ativos baixados.

   Para saber como baixar ativos de links compartilhados, consulte [baixando ativos de links](../using/brand-portal-link-share.md#main-pars-header-1703469193)compartilhados.

## Desempenho de download esperado {#expected-download-performance}

A experiência de download de arquivo pode variar para usuários em diferentes locais de cliente, dependendo de fatores como conectividade local à Internet e latência do servidor. O desempenho de download esperado para um arquivo de 2 GB observado em diferentes locais do cliente é o seguinte, com o servidor Brand Portal, no Oregon, Estados Unidos:

| Local do cliente | Latência entre cliente e servidor | Velocidade de download esperada | Tempo necessário para baixar um arquivo de 2 GB |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Oeste dos EUA (N. Califórnia) | 18 milissegundos | 7,68 MB/s | 4 minutos |
| Oeste dos EUA (Oregon) | 42 milissegundos | 3,84 MB/s | 9 minutos |
| Leste dos EUA (N. Virgínia) | 85 milissegundos | 1,61 MB/s | 21 minutos |
| APAC (Tóquio) | 124 milissegundos | 1,13 MB/s | 30 minutos |
| Noida | 275 milissegundos | 0,5 MB/s | 68 minutos |
| Sydney | 175 milissegundos | 0,49 MB/s | 69 minutos |
| Londres | 179 milissegundos | 0,32 MB/s | 106 minutos |
| Cingapura | 196 milissegundos | 0,5 MB/s | 68 minutos |

**Observação**: Os dados citados são observados em condições de teste, que podem variar para usuários em locais diferentes que testemunham latência e largura de banda variadas.
