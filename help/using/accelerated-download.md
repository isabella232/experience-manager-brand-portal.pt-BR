---
title: Acelere os downloads da Brand Portal
seo-title: Speed up the Brand Portal downloads
description: Melhore o desempenho de download do Brand Portal e dos links compartilhados.
seo-description: Enhance download performance from Brand Portal and the shared links.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: Vishabh Gupta
topic-tags: download-install, download assets
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
exl-id: cf28df58-c6dd-4b12-8279-01351892009f
source-git-commit: 63b7bdd34ff185a96ea69560d2b94c2dc04129de
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 3%

---

# Acelere os downloads da Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

A Adobe Experience Manager Assets Brand Portal permite melhorar o desempenho de download de arquivos de ativos grandes integrando-se ao IBM Aspera Connect, que é um aplicativo de instalação sob demanda. O aplicativo usa tecnologia proprietária para remover custos indiretos de TCP e ajuda a melhorar a velocidade de transferência dos arquivos de ativos. Essa integração garante uma melhor experiência de download.

>[!NOTE]
>
>A velocidade de download varia para os usuários, pois depende de fatores como largura de banda da rede, latência do servidor e localização geográfica dos clientes.

O **[!UICONTROL Download rápido]** por padrão, a configuração é ativada, o que reduz significativamente o tempo gasto para baixar os arquivos de ativos desejados do Brand Portal.

![](assets/download-settings-new.png)

## Pré-requisitos para acelerar o download de arquivos {#prerequisites-to-accelerate-file-download}

Para baixar os arquivos mais rápido, verifique o seguinte:

* Navegar para **[!UICONTROL Ferramentas]** > **[!UICONTROL Baixar]** e verificar se a **[!UICONTROL Download rápido]** está habilitada em **[!UICONTROL Configurações de download]**.
* Certifique-se de que a porta 33001 (TCP e UDP) esteja aberta no firewall. Para obter mais informações sobre os pré-requisitos, consulte [Documentação do IBM Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).
* **Instalar o IBM Aspera Connect 3.9.9** na extensão do navegador usando privilégios de administrador (`https://www.ibm.com/docs/en/aspera-connect/3.9.9`).
* Para obter o suporte da plataforma do cliente de transferência Aspera, consulte [Matriz de suporte da plataforma IBM Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

>[!NOTE]
>
>Há um problema conhecido com o IBM Aspera Connect. O download rápido não funciona com o IBM Aspera Connect versão 3.10 e superior.

## Baixar domínios {#download-domains}

A seguir estão os domínios de download para diferentes regiões:

| Código de região | Domínio |
|---|---|
| NA OU1 | downloads-na1.brand-portal.adobe.com |
| VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Exemplo de desempenho de download usando o acelerador de arquivo {#expected-download-performance-using-file-accelerator}

A tabela a seguir mostra o desempenho de download para arquivos de 2 GB usando o Acelerador de download de arquivo Aspera Connect:

*Os resultados observados variam devido a fatores como largura de banda de rede, latência de servidor e localização do cliente, considerando que o servidor Brand Portal está em Oregon (Estados Unidos).*

| Local do cliente | Latência entre o cliente e o servidor (milissegundos) | Velocidade com o Acelerador de Transferência de Arquivos Assimilar Connect (MBps) | Tempo gasto para fazer o download de um arquivo de 2 GB com o Acelerador de transferência de arquivo Aspera (segundos) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Oeste dos EUA (N. Califórnia) | 18º | 36º | 57º |
| U.S. West (Oregon) | 42º | 36º | 57º |
| Leste dos EUA (Virgínia) | 85 | 35º | 58º |
| APAC (Tóquio) | 124 | 36º | 57º |
| Noida (Índia) | 275 | 13,36 | 153º |
| Sydney | 175 | 29º | 70 |
| Londres | 179 | 35º | 58º |
| Cingapura | 196º | 34º | 60 |

## Baixar ativos {#download-assets}

Para baixar ativos mais rapidamente da Brand Portal:

1. Faça logon no locatário do Brand Portal. Por padrão, a variável **[!UICONTROL Arquivos]** é aberta uma visualização que contém todos os ativos e pastas publicados.

   Faça uma das seguintes opções:

   * Selecione os ativos ou pastas que deseja baixar. Na barra de ferramentas na parte superior, clique no botão **[!UICONTROL Baixar]** ícone .

      ![selecionar vários ativos](assets/select-assets-new.png)

   * Para baixar representações de ativos específicos de um ativo, passe o ponteiro do mouse sobre ele e clique no botão **[!UICONTROL Baixar]** ícone disponível nas miniaturas de ação rápida.

      ![select-asset](assets/select-asset.png)

1. O **[!UICONTROL Baixar]** será exibida a lista de todos os ativos selecionados.

   Para preservar a hierarquia de pastas do Brand Portal ao baixar ativos, selecione a variável **[!UICONTROL Criar uma pasta separada para cada ativo]** caixa de seleção.

   O botão de download reflete a contagem dos itens selecionados. Depois de concluir a aplicação das regras, clique em **[!UICONTROL Baixar itens]**. Para saber mais sobre como aplicar regras, consulte [baixar ativos](../using/download-assets.md#download-assets).

   ![caixa de diálogo de download](assets/download-dialog-box-new.png)

1. Por padrão, a variável **[!UICONTROL Download rápido]** está ativada na variável **[!UICONTROL Configurações de download]**. Portanto, uma caixa de confirmação é exibida para baixar ativos usando o IBM Aspera Connect.

   Se você estiver baixando os ativos pela primeira vez e não tiver o IBM Aspera Connect instalado em seu navegador ou a versão existente estiver desatualizada, ele solicitará a instalação do Acelerador de download Aspera (`https://www.ibm.com/docs/en/aspera-connect/3.9.9`).

   ![](assets/aspera-not-launched.png)

1. **Instalar Cliente do Aspera Connect**

   Para instalar a configuração de cliente do IBM Aspera Connect, execute a configuração a partir do arquivo .msi do aplicativo cliente IBM Aspera Connect e siga o assistente de instalação.

   ![](assets/aspera-download-1.png)

1. Depois que o cliente for instalado com êxito, atualize a página do navegador e inicie as etapas de download novamente.

1. Para continuar usando **[!UICONTROL Download rápido]**, clique em **[!UICONTROL Permitir]**. Todas as representações selecionadas são baixadas em uma pasta zip usando o IBM Aspera Connect.

   Ao concluir com sucesso o download, uma caixa de diálogo mostra o local onde os ativos são baixados no sistema do usuário.

   ![](assets/aspera-download-2.png)

   Se não quiser usar o IBM Assimilar Connect, clique em **[!UICONTROL Negar]**. If **[!UICONTROL Download rápido]** for negado ou falhar, o sistema preencherá uma mensagem de erro. Clique no botão **[!UICONTROL Download normal]** para continuar baixando os ativos.

>[!NOTE]
>
>Se a variável **[!UICONTROL Download rápido]** for desativada pelo administrador, as representações selecionadas serão baixadas diretamente em uma pasta zip sem usar o IBM Aspera Connect.

<!-- 
On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.


1. Log in to Brand Portal using a supported browser.
1. Browse and select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon. the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** and **[!UICONTROL Enable download acceleration]** check boxes selected by default. 

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >The functionality to send email notification with the link to download assets is presently not supported while faster downloads are enabled.

   ![](assets/fast-download-emailchk.png)

1. Click **[!UICONTROL Download]**.

   To speed up the download experience on your Brand Portal tenant account, you need to have Aspera Connect client application installed in your browser's extension.

1. **Download Aspera Connect Client**

   If Aspera Connect client is not installed on your system or the existing Aspera Connect client is out of date, a prompt is displayed on the browser page from where you can download the system-specific Aspera Connect client by selecting **[!UICONTROL Download Latest Version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

1. **Install Aspera Connect Client**

   To install IBM Aspera Connect client setup, run the setup from  .msi  file of IBM Aspera Connect client application and follow the installation wizard.

1. Once the client is successfully installed, refresh the browser page and initiate the download steps again.

   When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >This message is different on the different browsers.

1. A dialog box confirms whether to proceed the transfer or not. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. For more information, refer [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.
-->

## Uso do acelerador de arquivo no navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

O Microsoft Edge é executado no EPM (Enhanced Protected Mode), impedindo a comunicação com o servidor Aspera Connect, na mesma rede privada ou com um Site Confiável. Portanto, um pop-up é exibido sempre que uma conexão com o servidor é estabelecida.

![](assets/switchapps-msedge.png)

Para usar a funcionalidade de download acelerado no Microsoft Edge, remova o site do Brand Portal da lista de sites confiáveis.

1. Abra o Painel de controle (**[!UICONTROL Tecla Window + X]**, em seguida selecione **[!UICONTROL Painel de controle do Campaign]**).
1. Ir para **[!UICONTROL Rede e Internet]** > **[!UICONTROL Opções da Internet]**. Clique no botão **[!UICONTROL Segurança]** guia .
1. Clique no botão **[!UICONTROL Zona de sites confiáveis]**, depois clique em **[!UICONTROL Sites]**.
1. Remova o site do Brand Portal da lista.

## Assimilar preferências do cliente Connect {#aspera-connect-client-preferences}

Há algumas preferências úteis que podem ser definidas na preferência de cliente do IBM Aspera Connect clicando com o botão direito do mouse e selecionando **[!UICONTROL Preferências]**.

![](assets/download_assets_frombrandportalimg19.png)

Você pode definir o local de download padrão.

![](assets/aspera-preferences.png)

Além disso, o cliente Aspera Connect pode ser marcado para iniciar automaticamente na inicialização do sistema para que o cliente connect esteja em execução e disponível para que o download comece mais rápido.

![](assets/aspera-automaticallylaunch.png)

## Solucionar problemas com a aceleração de download {#troubleshoot-issues-with-download-acceleration}

Se a aceleração de download não estiver funcionando para você, siga estas etapas para solucionar o problema:

1. Verifique se as portas não estão bloqueadas, visitando [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) da sua máquina.

   Se as portas não estiverem OK, entre em contato com a equipe de rede e verifique se as portas 33001 (TCP e UDP) não estão bloqueadas no firewall.

1. Se as portas estiverem OK, verifique se a rede não está lenta, medindo a largura de banda disponível usando [https://www.speedtest.net/](https://www.speedtest.net/).

   Se a largura de banda for de alguns (1-10 Mbps) ou em Kbps, use Aspera Preferences e tente limitar a largura de banda igual à largura de banda disponível.

1. Para confirmar se os downloads do servidor de demonstração Aspera estão funcionando, use [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (login: asperaweb , senha: demoaspera )

1. Se nenhuma das etapas de solução de problemas acima funcionar, desmarque a opção Habilitar aceleração de download e use o download normal.
