---
title: Guia para acelerar downloads do portal da marca
seo-title: Guia para acelerar downloads do portal da marca
description: Aprimore o desempenho do download do Portal da marca e dos links compartilhados.
seo-description: Aprimore o desempenho do download do Portal da marca e dos links compartilhados.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: download-instalação
content-type: referência
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 alimentado 0 c 0
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Guia para acelerar downloads do portal da marca {#guide-to-accelerate-downloads-from-brand-portal}

O Brand Portal é compatível com o download acelerado de arquivos de ativos grandes por meio da integração com IBM Aspera Connect, que é um aplicativo de demanda de instalação. O aplicativo usa tecnologia proprietária para remover overloads TCP e ajuda a melhorar a velocidade de transferência de arquivos, dessa forma, garantindo uma experiência aprimorada de download. Os usuários distribuídos por localidades, com latência alta, também podem se beneficiar desse recurso.

>[!NOTE]
>
>O IBM Aspera Connect permite o download rápido de arquivos de ativos grandes do Brand Portal e links compartilhados, mas a velocidade de download pode variar dependendo de fatores, como largura de banda de rede, latência do servidor e localização geográfica dos clientes.

Para configurar os locatários específicos para download de arquivo acelerado, os administradores **[!UICONTROL ativam a Aceleração de download]** (que é desativada por padrão) das **Configurações gerais** no painel de ferramentas administrativas.

Se ativado, os usuários do Brand Portal podem reduzir significativamente o tempo gasto para baixar os arquivos de ativos desejados do Brand Portal ou por meio do link Compartilhado instalando o cliente Aspera Connect.

![](assets/enable-fast-file-download.png)

## Pré-requisitos para acelerar o download do arquivo {#prerequisites-to-accelerate-file-download}

Para usar a funcionalidade mais rápida de download de arquivo, verifique se:

* As portas 33001 (TCP &amp; UDP) são abertas no firewall por administradores. Para obter mais informações sobre os pré-requisitos para usar o IBM Aspera Connect, consulte [a documentação do Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).

   Veja a seguir os domínios de download para diferentes localidades geográficas:

   | Região | Domínio |
   |---|---|
   | NA OR 1 | downloads-na1.brand-portal.adobe.com |
   | NA VA 5 | downloads-na2.brand-portal.adobe.com |
   | EMEA LON 5 | downloads-emea1.brand-portal.adobe.com |
   | APAC SIN 2 | downloads-apac1.brand-portal.adobe.com |

* Os privilégios de administrador são usados para baixar o pacote do instalador do IBM Aspera, pois não é possível instalar o Aspera Connect na conta Convidado.

### Requisitos do sistema e do navegador {#system-and-browser-requirements}

Requisitos do sistema e do navegador para o Aspera Connect 3.8.0 são os seguintes:

| ﻿OS | Versão do SO | Navegador |  | Bibliotecas necessárias |
|----------------|----------------------------------------|-------------------|-------|--------------------------|
| Windows | Windows 7, 8, 10 | Chrome | 64-66 |  |
|  | Windows Server 2008, R 2, 2012 R 2, 2016 | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Internet Explorer | 11 |  |
|  |  | Microsoft Edge | 39-42 |  |
| Macos | 10.11 - 10.13 | Chrome | 64-66 |  |
|  |  | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Safari | 11 |  |
| Linux (64 bits) | RHEL 6 - 7 | Chrome | 64-66 | Openssl 1.0.2 g ou superior |
|  | Centos 6 - 7 |  |  | Mesa EGL |
|  | Debian 7 - 9 |  |  | glib 2 2.28 ou superior |
|  | SLES 11 - 12 |  |  |  |
|  | Fedora 26 - 27 |  |  |  |
|  | Opensuse 42.3 | Firefox | 57-60 |  |
|  | Ubuntu 14 - 17 | Firefox ESR | 52 |  |

Para obter a plataforma de suporte a matrizes diferentes de cliente de transferência Aspera, consulte [matriz de suporte à plataforma Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## O desempenho do download esperado usando acelerador de arquivo {#expected-download-performance-using-file-accelerator}

O desempenho de download esperado para o arquivo 2 GB usando o acelerador de download de arquivo Aspera Connect em locais cliente diferentes é o seguinte, considerando o servidor do Brand Portal em Oregon nos Estados Unidos:

| Localização do cliente | Latência entre cliente e servidor | Velocidade com o Acelerador de transferência de arquivo Aspera | Tempo decorrido para baixar o arquivo de 2 GB com o Acelerador de transferência de arquivo Aspera |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Oeste dos EUA (N. Califórnia) | 18 milissegundos | 36 MB/s | 57 segundos |
| Oeste dos EUA (Oregon) | 42 milissegundos | 36 MB/s | 57 segundos |
| Leste dos EUA (N. Virgínia) | 85 milissegundos | 35 MB/s | 58 segundos |
| APAC (Tóquio) | 124 milissegundos | 36 MB/s | 57 segundos |
| Noida | 275 milissegundos | 13.36 MB/s | 153 segundos |
| Sydney | 175 milissegundos | 29 MB/s | 70 segundos |
| Londres | 179 milissegundos | 35 MB/s | 58 segundos |
| Cingapura | 196 milissegundos | 34 MB/s | 60 segundos |

>[!NOTE]
>
>Os dados citados são os de acordo com os testes realizados no laboratório e são apenas indicativos. Os resultados observados variam devido a fatores como largura de banda de rede, latência do servidor e localização do cliente.

## Baixar o fluxo de trabalho usando acelerador de arquivo {#download-workflow-using-file-accelerator}

Para baixar ativos mais rapidamente do Portal da marca:

1. Faça logon no Brand Portal por meio de um navegador preferencial.
2. Procure e selecione o arquivo, pasta ou coleção de ativos desejado para baixar. Toque/clique na opção de download.
A caixa de diálogo Download é exibida com [a opção Ativar aceleração] de download selecionada.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >A funcionalidade para enviar uma notificação por email com o link para fazer download de ativos não é suportada enquanto os downloads mais rápidos estão ativados.

   ![](assets/fast-download-emailchk.png)

3. Toque/clique **em Download**.
Para acelerar a experiência de download na conta de locatário do Brand Portal, você precisa ter o aplicativo de cliente Aspera Connect instalado no sistema.

4. **Baixar o cliente Aspera Connect se**
o cliente Aspera Connect não estiver instalado no sistema ou o cliente Aspera Connect existente estiver desatualizado, um prompt será exibido na página do navegador onde você poderá baixar o cliente Aspera Connect específico do sistema selecionando **Baixar versão mais recente**.

   ![](assets/aspera-not-launched.png)

   Para baixar a versão mais recente do Acrobat Connect de [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), selecione **Download agora** e siga as instruções.

5. **Instale o Aspera Connect Client**
para instalar a configuração de cliente IBM Aspera Connect, execute a configuração do arquivo. msi do aplicativo cliente IBM Aspera Connect e siga o assistente de instalação.

6. Depois que o cliente for instalado com êxito, atualize a página do navegador e inicie as etapas de download novamente ou selecione **Reiniciar** na caixa de diálogo **Download** do ativo (Etapa n º 2).
Ao usar o Aspera Connect pela primeira vez, o navegador solicita abrir o link usando **IBM Aspera Connect**. Para ignorar essa caixa de diálogo no futuro, ative **Lembrar minha escolha para links FASP**.

   >[!NOTE]
   >
   >Essa mensagem é diferente em navegadores diferentes.

7. Uma caixa de diálogo confirma se deseja ou não executar a transferência. Selecione **Permitir** para começar.
Para ignorar essa caixa de diálogo no futuro, ative **Usar minha escolha para todas as conexões com esse host**.
O download começa. Uma caixa de diálogo mostra o progresso do download. Use a caixa de diálogo para **pausar**, **retomar** ou **cancelar** o download.
O aplicativo Aspera Connect fornece uma Janela de atividade no sistema em que o usuário pode visualizar e gerenciar todas as sessões de transferência. Para obter mais informações, consulte [a documentação do Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Após a conclusão do download, uma caixa de diálogo mostra o local onde os ativos são baixados para o sistema do usuário. Se houver uma falha, mostra o erro.

>[!NOTE]
>
>Há uma limitação conhecida no aplicativo cliente Aspera Connect que nenhum prompt para selecionar o local de download aparece se **sempre perguntar onde salvar arquivos** baixados na guia** Transferências** em **Preferências**. Antes de iniciar qualquer download, forneça o local na caixa de texto **Salvar arquivos baixados.**

## Usar acelerador de arquivo no navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

O Microsoft Edge é executado no modo Protegido aprimorado (EPM), evitando a comunicação com o servidor Aspera Connect, enquanto na mesma rede privada ou com um Site confiável. Portanto, uma pop-up aparece sempre que uma conexão com o servidor está sendo estabelecida.

![](assets/switchapps-msedge.png)

Para usar a funcionalidade de download acelerada no Microsoft Edge, remova o site do Brand Portal da lista de site confiável.

1. Abra o Painel de controle (pressione **a tecla Window + X** e selecione **Painel de controle**).
2. Vá para **Rede e Internet &gt; Opções da Internet**. Click the **Security** tab.
3. Clique na **zona de sites confiáveis** e clique **em Sites**.
4. Remova o site do Brand Portal da lista.

## Preferências do cliente Aspera Connect {#aspera-connect-client-preferences}

Há algumas preferências úteis que podem ser definidas na preferência IBM Aspera Connect Client clicando com o botão direito do mouse no ícone e selecionando **Preferências**.

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
