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
source-git-commit: f4f92724cdd4ba8c79d3d72de5cba9451dceadb1
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 2%

---


# Baixar ativos {#download-assets}

<!-- Before update in Download experience - 26th Aug 2020 by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

O Portal de marcas do Adobe Experience Manager Assets aprimora a experiência de download, permitindo que os usuários baixem simultaneamente vários ativos e pastas acessíveis a eles no Portal de marcas. Dessa forma, os ativos aprovados da marca podem ser distribuídos com segurança para uso offline. Leia para saber como baixar os ativos aprovados no Brand Portal e o que esperar do desempenho [do](../using/brand-portal-download-assets.md#expected-download-performance)download.

>[!NOTE]
>
>Instale o IBM Aspera Connect 3.9.9 na extensão do seu navegador antes de baixar os ativos do Brand Portal.


<!--
**Types of renditions in Brand Portal:**

* Original asset rendition

  It is the original binary of the asset uploaded in AEM Assets. 
  
  
* System renditions

  These are the thumbnail renditions which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 
  
* Custom renditions

  These are the additional renditions that an asset might have and its dynamic renditions. Any user can create additional custom renditions, whereas, only the AEM administrator can create dynamic renditions of an image in AEM Assets. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md).     
-->

## Configurar download de ativos {#configure-download}

A configuração de download permite que os administradores do Brand Portal definam o conjunto de execuções disponíveis para os usuários do Brand Portal para o download dos ativos. O administrador pode definir as configurações de **[!UICONTROL Download]** de ativos na interface do Brand Portal.

As configurações disponíveis são:

* **[!UICONTROL Download rápido]**

   Permite o download de alta velocidade dos ativos. Para saber mais, consulte o [guia para acelerar os downloads do Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Representações personalizadas]**

   Baixe representações personalizadas e (ou) dinâmicas dos ativos.
Todas as representações de ativos diferentes do ativo original e representações geradas pelo sistema são chamadas de representações personalizadas. Inclui representações estáticas e dinâmicas disponíveis para o ativo. Qualquer usuário pode criar uma execução estática personalizada no AEM Assets, enquanto que, somente o administrador do AEM pode criar execuções dinâmicas personalizadas. Para saber mais, consulte [como aplicar predefinições de imagens ou representações dinâmicas](../using/brand-portal-image-presets.md)

* **[!UICONTROL Representações do sistema]**

   Baixe execuções geradas pelo sistema dos ativos. Estas são as miniaturas que são geradas automaticamente no AEM Assets com base no fluxo de trabalho &quot;Ativo de atualização do DAM&quot;.

Faça logon no locatário do Brand Portal como administrador e navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Download]**. Por padrão, a configuração de Download **** rápido está ativada nas Configurações **[!UICONTROL de]** download.

Os administradores podem habilitar qualquer combinação para configurar o processo de download de ativos.

![](assets/download-configuration.png)


Com base na configuração, o fluxo de trabalho de download permanece constante para ativos independentes, vários ativos, pastas que contêm ativos, ativos licenciados ou não licenciados e o download de ativos usando o link de compartilhamento.


* Se as configurações de Representações **** personalizadas e Representações **[!UICONTROL de]** sistema estiverem desativadas, as representações originais dos ativos serão baixadas sem que qualquer caixa de diálogo adicional seja apresentada aos usuários.

<!--
If all the three download configurations are turned-off, or only the **[!UICONTROL Fast Download]** configuration is enabled, the original assets are directly downloaded on your local system with no additional step required.
Test.. 
-->

* Se qualquer uma das configurações de Representações **** personalizadas ou Representações **** do sistema estiver ativada, uma caixa de diálogo **[!UICONTROL Download]** adicional será exibida, onde você pode escolher baixar o ativo original juntamente com suas representações ou baixar somente representações específicas.

>[!NOTE]
>
>Somente os administradores podem baixar os ativos expirados. Para obter mais informações sobre ativos expirados, consulte [gerenciar direitos digitais de ativos](../using/manage-digital-rights-of-assets.md).


## Etapas para baixar ativos {#steps-to-download-assets}

Veja a seguir as etapas para baixar ativos ou pastas que contêm ativos do Brand Portal:

1. Na interface do Brand Portal, execute um dos procedimentos a seguir:

   * Selecione as pastas ou os ativos que deseja baixar. Na barra de ferramentas na parte superior, clique no ícone **[!UICONTROL Download]** .

      ![](assets/downloadassets-1.png)

   * Para baixar um ativo ou pasta específico, passe o ponteiro do mouse sobre o ativo ou pasta e clique no ícone **[!UICONTROL Download]** disponível nas miniaturas de ação rápida.

      ![](assets/downloadsingleasset-1.png)


      >[!NOTE]
      >
      >Se você estiver baixando os ativos pela primeira vez e não tiver o IBM Aspera Connect instalado em seu navegador, ele solicitará a instalação do Acelerador de download Aspera.

      >[!NOTE]
      >
      >Se os ativos que você está baixando também incluírem ativos licenciados, você será redirecionado para a página Gerenciamento **[!UICONTROL de]** direitos autorais. Nesta página, selecione os ativos, clique em **[!UICONTROL Concordar]** e, em seguida, clique em **[!UICONTROL Download]**. Se você optar por discordar, os ativos licenciados não serão baixados.
      > 
      >Os ativos protegidos por licença têm o contrato de [licença anexado](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) a eles, o que é feito ao configurar a propriedade [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadados do ativo nos Ativos Experience Manager.

      ![](assets/licensed-asset-download-1.png)

      Se qualquer configuração de Representações **** personalizadas ou Representações **** do sistema estiver ativada nas Configurações **[!UICONTROL de]** download, a caixa de diálogo **[!UICONTROL Download]** será exibida com a caixa de seleção **[!UICONTROL Ativo(s)]** selecionada por padrão. Se a configuração do Download **** rápido estiver ativada, a caixa de seleção **[!UICONTROL Ativar aceleração]** de download estará marcada por padrão.

      ![](assets/download-dialog.png)

      >[!NOTE]
      >
      >Se os ativos de download forem arquivos de imagem e você selecionar apenas a caixa de seleção **[!UICONTROL Ativo(s)]** na caixa de diálogo **[!UICONTROL Download]** , mas não forem [autorizados pelo administrador a ter acesso às representações originais dos arquivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) de imagem, nenhum arquivo de imagem será baixado e uma notificação será exibida, informando que você foi restringido pelo administrador a acessar as representações originais.

      ![](assets/restrictaccess-note.png)

1. Para baixar as representações além dos ativos originais, marque a caixa de seleção **[!UICONTROL Representações]** . No entanto, se você quiser baixar as execuções geradas pelo sistema junto com as execuções personalizadas, desmarque a caixa de seleção **[!UICONTROL Excluir representações]** do sistema.

   ![](assets/download-system-rendition.png)

   * Para baixar apenas as representações, desmarque a caixa de seleção **[!UICONTROL Ativo(s)]** .

      >[!NOTE]
      >
      >Por padrão, somente os ativos são baixados. No entanto, as representações originais dos arquivos de imagem não serão baixadas se você não estiver [autorizado pelo administrador a ter acesso às representações originais dos arquivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)de imagem.

   * Para compartilhar os ativos selecionados com outros usuários por meio de um link, marque a caixa de seleção **[!UICONTROL Email]** . Uma notificação por email é enviada aos usuários com o link de download. Para saber como baixar ativos de links compartilhados, consulte [Download de ativos de links](../using/brand-portal-link-share.md#main-pars-header-1703469193)compartilhados.

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >O link de download na notificação por email expira após 45 dias.
      >
      >Os administradores podem personalizar mensagens de e-mail, isto é, logotipo, descrição e rodapé, usando o recurso [Marca](../using/brand-portal-branding.md) .

   * Você pode selecionar uma predefinição de imagem predefinida ou criar uma representação dinâmica personalizada na caixa de diálogo **[!UICONTROL Download]** .

      Para aplicar uma predefinição de imagem [personalizada ao ativo e suas representações](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), marque a caixa de seleção Representações **[!UICONTROL dinâmicas]** . Especifique as propriedades predefinidas da imagem (como tamanho, formato, espaço de cor, resolução e modificador de imagem) para aplicar a predefinição de imagem personalizada ao baixar o ativo e suas representações. Para baixar apenas as representações dinâmicas, desmarque a caixa de seleção **[!UICONTROL Ativo(s)]** .

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >O Brand Portal suporta a configuração de Dynamic Media em ambos os modos - Hybird e Scene 7.
      >
      >(*Se AEM instância do autor estiver em execução no modo **Híbrido do***Dynamic Media)      >Para pré-visualização ou download de representações dinâmicas de um ativo, verifique se a mídia dinâmica está ativada e se a representação temporária do ativo em Pirâmide existe na instância do autor da AEM Assets de onde os ativos foram publicados. Quando um ativo é publicado no Brand Portal, sua representação em pirâmide também é publicada.

   * Para preservar a hierarquia de pastas do Brand Portal ao baixar ativos, marque a caixa de seleção **[!UICONTROL Criar pasta separada para cada ativo]** . Por padrão, a hierarquia de pastas do Brand Portal é ignorada e todos os ativos são baixados em uma pasta no sistema local.

1. Clique em **[!UICONTROL Download]**.

   Os ativos (e as execuções, se selecionadas) são baixados como um arquivo zip para a pasta local. No entanto, nenhum arquivo zip será criado se um único ativo for baixado sem nenhuma das representações.

   Se você não estiver [autorizado pelo administrador a ter acesso às representações](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)originais, as representações originais dos ativos selecionados não serão baixadas.

   >[!NOTE]
   >
   >Os ativos que são baixados individualmente ficam visíveis no relatório de download de ativos. No entanto, se uma pasta que contém ativos for baixada, a pasta e os ativos não serão exibidos no relatório de download de ativos.


## Desempenho de download esperado {#expected-download-performance}

A experiência de download de arquivo pode variar para usuários em diferentes locais de cliente, dependendo de fatores como conectividade local à Internet e latência do servidor. O desempenho de download esperado para o arquivo de 2 GB observado em diferentes locais de clientes é o seguinte, com o servidor Brand Portal, no Oregon, Estados Unidos:

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

>[!NOTE]
>
>Os dados citados são observados em condições de teste, que podem variar para usuários em locais diferentes que testemunham latência e largura de banda variadas.

