---
title: Acelerar os downloads do Brand Portal
seo-title: Acelerar os downloads do Brand Portal
description: Aprimore o desempenho do download do Portal da marca e dos links compartilhados.
seo-description: Aprimore o desempenho do download do Portal da marca e dos links compartilhados.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: download-instalação
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 alimentado 0 c 0
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Acelerar os downloads do Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

O Brand Portal permite aprimorar o desempenho do download de arquivos de ativos grandes por meio da integração com IBM Aspera Connect, que é um aplicativo de demanda de instalação. O aplicativo usa tecnologia proprietária para remover overloads TCP e ajuda a melhorar a velocidade de transferência dos arquivos do ativo. Essa integração garante uma experiência aprimorada de download.

>[!NOTE]
>
>A velocidade de download varia para os usuários, pois depende de fatores como largura de banda de rede, latência do servidor e localização geográfica dos clientes.

Se ativado, os usuários do Brand Portal podem reduzir significativamente o tempo gasto para baixar os arquivos de ativos desejados do Brand Portal ou por meio do link Compartilhado instalando o cliente Aspera Connect.

![](assets/enable-fast-file-download.png)

## Pré-requisitos para acelerar o download do arquivo {#prerequisites-to-accelerate-file-download}

Para baixar os arquivos mais rapidamente, verifique o seguinte:

* **[!UICONTROL Ative a Aceleração de download]** (desabilitada por padrão) das [!UICONTROL Configurações gerais] no painel de ferramentas administrativas.
* A porta 33001 (TCP e UDP) está aberta no firewall. Para obter mais informações sobre os pré-requisitos, consulte [a documentação do Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).
* Instale o Aspera Connect usando privilégios de administrador.
* Para suporte à plataforma de cliente de transferência Aspera, consulte [matriz de suporte à plataforma Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## Baixar domínios {#download-domains}

Veja a seguir os domínios de download para diferentes localidades geográficas:

| Código da região | Domínio |
|---|---|
| NA OR 1 | downloads-na1.brand-portal.adobe.com |
| NA VA 5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON 5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN 2 | downloads-apac1.brand-portal.adobe.com |

## Amostra do desempenho do download usando acelerador de arquivo {#expected-download-performance-using-file-accelerator}

A tabela a seguir mostra o desempenho de download de arquivo 2 GB usando acelerador de download de arquivo Aspera Connect:

**Os resultados observados variam devido a fatores como largura de banda de rede, latência do servidor e localização do cliente, considerando que o servidor Brand Portal está no Oregon (Estados Unidos).*

| Localização do cliente | Latência entre cliente e servidor (milissegundos) | Velocidade com o Acelerador de transferência de arquivo Aspera Connect (mbps) | Tempo decorrido para baixar o arquivo de 2 GB com o Acelerador de transferência de arquivo Aspera (segundos) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Oeste dos EUA (N. Califórnia) | 18 | 36 | 57 |
| Oeste dos EUA (Oregon) | 42 | 36 | 57 |
| Leste dos EUA (N. Virgínia) | 85 | 35 | 58 |
| APAC (Tóquio) | 124 | 36 | 57 |
| Noida (Índia) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| Londres | 179 | 35 | 58 |
| Cingapura | 196 | 34 | 60 |

## Baixar o fluxo de trabalho usando acelerador de arquivo {#download-workflow-using-file-accelerator}

Para baixar ativos mais rapidamente do Portal da marca:

1. Faça logon no Brand Portal usando um navegador compatível.
2. Procure e selecione o arquivo, pasta ou coleção de ativos desejado para baixar. Toque/clique na opção de download.
A caixa de diálogo Download é exibida com [a opção Ativar aceleração] de download selecionada.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >A funcionalidade para enviar uma notificação por email com o link para fazer download de ativos não é suportada enquanto os downloads mais rápidos estão ativados.

   ![](assets/fast-download-emailchk.png)

3. Toque/clique na **[!UICONTROL opção Download]** .
Para acelerar a experiência de download na conta de locatário do Brand Portal, você precisa ter o aplicativo de cliente Aspera Connect instalado no sistema.

4. **Baixar o cliente Aspera Connect se**
o cliente Aspera Connect não estiver instalado no sistema ou o cliente Aspera Connect existente estiver desatualizado, um prompt será exibido na página do navegador onde você poderá baixar o cliente Aspera Connect específico do sistema selecionando **[!UICONTROL Baixar versão mais recente]**.

   ![](assets/aspera-not-launched.png)

   Para baixar a versão mais recente do Acrobat Connect de [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), selecione **[!UICONTROL Download agora]** e siga as instruções.

5. **Instale o Aspera Connect Client**
para instalar a configuração de cliente IBM Aspera Connect, execute a configuração do arquivo. msi do aplicativo cliente IBM Aspera Connect e siga o assistente de instalação.

6. Depois que o cliente for instalado com êxito, atualize a página do navegador e inicie as etapas de download novamente ou selecione **[!UICONTROL Reiniciar]** na caixa de diálogo **[!UICONTROL Download]** do ativo (Etapa n º 2).
Ao usar o Aspera Connect pela primeira vez, o navegador solicita abrir o link usando **[!UICONTROL IBM Aspera Connect]**. Para ignorar essa caixa de diálogo no futuro, ative **[!UICONTROL Lembrar minha escolha para links FASP]**.

   >[!NOTE]
   >
   >Essa mensagem é diferente em navegadores diferentes.

7. Uma caixa de diálogo confirma se deseja ou não executar a transferência. Selecione **[!UICONTROL Permitir]** para começar.
Para ignorar essa caixa de diálogo no futuro, ative **[!UICONTROL Usar minha escolha para todas as conexões com esse host]**.
O download começa. Uma caixa de diálogo mostra o progresso do download. Use a caixa de diálogo para **[!UICONTROL pausar]**, **[!UICONTROL retomar]** ou **[!UICONTROL cancelar]** o download.
O aplicativo Aspera Connect fornece uma Janela de atividade no sistema em que o usuário pode visualizar e gerenciar todas as sessões de transferência. Para obter mais informações, consulte [a documentação do Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Após a conclusão do download, uma caixa de diálogo mostra o local onde os ativos são baixados para o sistema do usuário. Se houver uma falha, mostra o erro.

>[!NOTE]
>
>Há uma limitação conhecida no aplicativo cliente Aspera Connect que nenhum prompt para selecionar o local de download aparece se **[!UICONTROL sempre perguntar onde salvar arquivos]** baixados é ativado nas [!UICONTROL Transferências de guia] nas [!UICONTROL Preferências]. Antes de iniciar qualquer download, forneça o local na caixa de texto **[!UICONTROL Salvar arquivos baixados.]**

## Usar acelerador de arquivo no navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

O Microsoft Edge é executado no modo Protegido aprimorado (EPM), evitando a comunicação com o servidor Aspera Connect, enquanto na mesma rede privada ou com um Site confiável. Portanto, uma pop-up aparece sempre que uma conexão com o servidor está sendo estabelecida.

![](assets/switchapps-msedge.png)

Para usar a funcionalidade de download acelerada no Microsoft Edge, remova o site do Brand Portal da lista de site confiável.

1. Abra o Painel de controle (pressione **[!UICONTROL a tecla Window + X]** e selecione **[!UICONTROL Painel de controle]**).
2. Vá para **[!UICONTROL Rede e Internet &gt; Opções da Internet]**. Clique na **[!UICONTROL guia Segurança]** .
3. Clique na **[!UICONTROL zona de sites confiáveis]** e clique **[!UICONTROL em Sites]**.
4. Remova o site do Brand Portal da lista.

## Preferências do cliente Aspera Connect {#aspera-connect-client-preferences}

Há algumas preferências úteis que podem ser definidas na preferência IBM Aspera Connect Client clicando com o botão direito do mouse no ícone e selecionando **[!UICONTROL Preferências]**.

![](assets/download_assets_frombrandportalimg19.png)

Você pode definir o local padrão de download.

![](assets/aspera-preferences.png)

Além disso, o cliente Aspera Connect pode ser marcado para iniciar automaticamente na inicialização do sistema para que o cliente Connect esteja em execução e disponível para que o download comece mais rápido.

![](assets/aspera-automaticallylaunch.png)

## Solucionar problemas com a aceleração de download {#troubleshoot-issues-with-download-acceleration}

Se a aceleração de download não estiver funcionando para você, siga estas etapas para solucionar o problema:

1. Verifique se as portas não estão bloqueadas ao visitar [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) de sua máquina.

   Se as portas não estiverem OK, entre em contato com a equipe de rede e certifique-se de que as Portas 33001 (TCP &amp; UDP) não estejam bloqueadas no firewall.

2. Se as portas estiverem OK, verifique se a rede não é lenta, ao medir a largura de banda disponível usando [https://www.speedtest.net/](https://www.speedtest.net/).

   Se a largura de banda tiver alguns (1-10 Mbps) ou em Kbps, use Preferências Aspera e tente limitar a largura de banda igual à largura de banda disponível.

3. Para confirmar se os downloads do servidor de demonstração Aspera estão funcionando, use [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (logon: asperaweb, senha: demoaspera)

4. Se nenhuma das etapas de solução de problemas acima funcionar, desmarque a opção Ativar aceleração de download e use o download normal.
