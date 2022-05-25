---
title: Faça upload de ativos e publique a pasta Contribuição do Brand Portal para o Experience Manager Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: Obtenha informações sobre como fazer upload de novos ativos e publicar a pasta de contribuição do Brand Portal para o Experience Manager Assets.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 606f4389780025f5cf92b11bf8cac464e36be44a
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Publicar a pasta de contribuição no Experience Manager Assets {#using-asset-souring-in-bp}

Os usuários da Brand Portal com permissões apropriadas podem fazer upload de vários ativos ou pastas contendo vários ativos para a pasta de contribuição. No entanto, os usuários do Brand Portal só podem fazer upload de ativos para o **NOVO** pasta. O **COMPARTILHADO** destina-se à distribuição de ativos da linha de base (conteúdo de referência) que podem ser usados pelos usuários da Brand Portal ao criar novos ativos para contribuição.

O usuário do Brand Portal com permissão para acessar a pasta de contribuição pode executar as seguintes atividades:

* [Baixar requisitos de ativos](#download-asset-requirements)
* [Fazer upload de novos ativos para a pasta de contribuição](#uplad-new-assets-to-contribution-folder)
* [Publicar a pasta de contribuição no Experience Manager Assets](#publish-contribution-folder-to-aem)

## Baixar requisitos de ativos {#download-asset-requirements}

Os usuários do Brand Portal recebem automaticamente notificações por e-mail/pulso sempre que uma pasta de contribuição é compartilhada pelo usuário do Experience Manager Assets, permitindo que baixem o documento resumido (requisito de ativo), bem como baixar os ativos da linha de base (conteúdo de referência) da **COMPARTILHADO** para garantir que entenda os requisitos do ativo.

O usuário do Brand Portal realiza as seguintes atividades para baixar os requisitos de ativos:

* **Resumo do download**: Baixe o resumo (documento de requisito de ativo) anexado à pasta de contribuição que contém informações relacionadas ao ativo, como tipo de ativos, finalidade, formatos compatíveis, tamanho máximo do ativo etc.
* **Baixar ativos da linha de base**: Baixe os ativos da linha de base que podem ser usados para entender os tipos de ativos necessários. Os usuários da Brand Portal podem usar esses ativos como referência para criar novos ativos para contribuição.

O painel do Brand Portal reflete todas as pastas existentes permitidas para o usuário do Brand Portal junto com a pasta de contribuição compartilhada recentemente. Neste exemplo, o usuário do Brand Portal só tem acesso à pasta de contribuição recém-criada, nenhuma outra pasta existente é compartilhada com o usuário.

**Para baixar os requisitos de ativos:**

1. Faça logon na instância do Brand Portal.
1. Selecione a pasta de contribuição no painel da Brand Portal.
1. Clique em **[!UICONTROL Propriedades]**. A janela Propriedade que contém os detalhes da pasta de contribuição é aberta.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Clique no botão **[!UICONTROL Download breve]** para baixar o documento de requisito de ativo em sua máquina local.

   ![](assets/download.png)

1. Volte para o painel do Brand Portal.
1. Clique para abrir a pasta de contribuição, você pode ver duas subpastas -**[!UICONTROL COMPARTILHADO]** e **[!UICONTROL NOVO]** na pasta de contribuição. A pasta COMPARTILHADA contém todos os ativos de linha de base (conteúdo de referência) compartilhados pelos administradores.
1. Você pode baixar o **[!UICONTROL COMPARTILHADO]** pasta contendo todos os ativos da linha de base em sua máquina local.
Ou você pode abrir o **[!UICONTROL COMPARTILHADO]** e clique no botão **Baixar** ícone para baixar arquivos/pastas individuais.

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

Analise o resumo (documento de requisito de ativo) e consulte os ativos da linha de base para entender os requisitos de ativos. Agora, você pode criar novos ativos para contribuição e carregá-los na pasta de contribuição.


## Fazer upload de ativos para a pasta de contribuição {#upload-new-assets-to-contribution-folder}

Após verificar os requisitos de ativos, os usuários do Brand Portal podem criar novos ativos para contribuição e carregá-los na pasta NOVA na pasta de contribuição. Um usuário pode fazer upload de vários ativos para uma pasta de contribuição de ativos. No entanto, apenas uma pasta pode ser criada de cada vez.

>[!NOTE]
>
>Os usuários do Brand Portal podem fazer upload de ativos (máximo de **2** GB por tamanho de arquivo) para a pasta NEW.
>
>O limite máximo de upload para qualquer locatário do Brand Portal é **10º** GB que é aplicado cumulativamente a todas as pastas de contribuição.
>
>Os ativos carregados no Brand Portal não são processados para representações e não contêm visualizações.

>[!NOTE]
>
>É recomendável liberar o espaço de upload após a publicação da pasta de contribuição no Experience Manager Assets para que ele fique disponível para contribuição dos outros usuários do Brand Portal.
>
>Se houver a necessidade de estender o limite de upload do seu locatário do Brand Portal além de **10º** GB, entre em contato com o Suporte ao cliente especificando o requisito.


**Para fazer upload de novos ativos:**

1. Faça logon na instância do Brand Portal.
O painel do Brand Portal reflete todas as pastas existentes permitidas para o usuário do Brand Portal junto com a pasta de contribuição compartilhada recentemente.

1. Selecione a pasta de contribuição e clique em para abri-la. A pasta de contribuição contém duas subpastas - **[!UICONTROL COMPARTILHADO]** e **[!UICONTROL NOVO]**.

1. Clique no botão **[!UICONTROL NOVO]** pasta.

   ![](assets/upload-new-assets4.png)

1. Clique em **[!UICONTROL Criar]** > **[!UICONTROL Arquivos]** para carregar arquivos individuais ou pastas (.zip) contendo vários ativos.

   ![](assets/upload-new-assets5.png)

1. Procure e faça upload de ativos (arquivos ou pastas) no **[!UICONTROL NOVO]** pasta.

   ![](assets/upload-asset4.png)

Após fazer upload de todos os ativos ou pastas para a pasta NEW , publique a pasta de contribuição na Experience Manager Assets.


## Publicar a pasta de contribuição no Experience Manager Assets {#publish-contribution-folder-to-aem}

Os usuários do Brand Portal podem publicar a pasta de contribuição no Experience Manager Assets sem precisar acessar a instância do autor do Experience Manager.

Certifique-se de ter passado pelos requisitos do ativo e feito upload dos ativos recém-criados em **NOVO** na pasta de contribuição.

**Para publicar a pasta de contribuição:**

1. Faça logon na instância do Brand Portal.

1. Selecione a pasta de contribuição no painel da Brand Portal.
1. Clique em **[!UICONTROL Publicar no AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

Uma notificação por email/pulso é enviada ao usuário e administradores do Brand Portal em diferentes estágios do fluxo de trabalho de publicação:

1. **Em fila** - Uma notificação é enviada ao usuário do Brand Portal e aos administradores do Brand Portal quando um fluxo de trabalho de publicação é acionado no Brand Portal.

1. **Concluído** - Uma notificação é enviada ao usuário do Brand Portal e aos administradores do Brand Portal quando a pasta de contribuição é publicada com êxito no Experience Manager Assets.

Após publicar os ativos recém-criados no Experience Manager Assets, os usuários do Brand Portal podem excluí-los da NOVA pasta. Enquanto isso, o administrador do Brand Portal pode excluir os ativos das pastas NOVO e COMPARTILHADO.

Quando o objetivo de criar a pasta de contribuição for atingido, o administrador do Brand Portal poderá excluir a pasta de contribuição para liberar o espaço de upload para outros usuários.

## Publicar o status do trabalho {#publishing-job-status}

Há dois relatórios que os administradores podem utilizar para visualizar o status das pastas de contribuição de ativos publicadas do Brand Portal para o Experience Manager Assets.

* No Brand Portal, navegue até **[!UICONTROL Ferramentas]** > **[!UICONTROL Status da contribuição de ativos]**. Este relatório reflete o status de todos os trabalhos de publicação em estágios diferentes do fluxo de trabalho de publicação.

   ![](assets/contribution-folder-status-v2.png)

* No Experience Manager Assets (no local ou serviço gerenciado), navegue até **[!UICONTROL Ativos]** > **[!UICONTROL Tarefas]**. Este relatório reflete o estado final (Sucesso ou Erro) de todos os trabalhos de publicação.

   ![](assets/publishing-status.png)

* No Experience Manager Assets as a Cloud Service, navegue até **[!UICONTROL Ativos]** > **[!UICONTROL Tarefas]**.

   Ou você pode navegar diretamente para **[!UICONTROL Tarefas]** da navegação global.

   Este relatório reflete o estado final (Sucesso ou Erro) de todos os trabalhos de publicação, incluindo a importação de ativos do Brand Portal para o Experience Manager Assets as a Cloud Service.

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## Exclusão automática de ativos publicados na Experience Manager Assets na pasta Contribuição {#automatically-delete-published-assets-from-contribution-folder}

A Brand Portal agora executa trabalhos automáticos a cada doze horas para verificar todas as pastas de Contribuição e excluir todos os ativos publicados no AEM. Como resultado, não é necessário excluir os ativos na pasta Contribuição manualmente para manter o tamanho da pasta abaixo do [limite](#upload-new-assets-to-contribution-folder). Você também pode monitorar o status dos trabalhos de exclusão executados automaticamente nos últimos sete dias. O relatório de uma tarefa fornece os seguintes detalhes:

* Hora de início da tarefa
* Hora de término da tarefa
* Status da tarefa
* Total dos ativos incluídos numa tarefa
* Total de ativos excluídos com êxito em uma tarefa
* Armazenamento total disponibilizado como resultado da execução do trabalho

   ![Relatório de exclusão](assets/deletion-reports.png)

Também é possível fazer uma busca detalhada para exibir os detalhes de cada ativo incluído em um job de exclusão. Detalhes como título do ativo, tamanho, autor, status de exclusão e tempo de exclusão são incluídos no relatório.

![Relatório de Exclusão Detalhado](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * Os clientes podem solicitar que o Suporte ao cliente do Adobe desative e reative o recurso de exclusão automática de trabalho ou altere a frequência de execução.
> * Este recurso está disponível com o Experience Manager 6.5.13.0 e versões posteriores.


### Exibir e baixar relatórios de exclusão {#view-delete-jobs}

Para exibir e baixar relatórios para um trabalho de exclusão:

1. No Brand Portal, navegue até **[!UICONTROL Ferramentas]**>**[!UICONTROL Status da contribuição de ativos]**>**[!UICONTROL Relatórios de exclusão]** opção.

1. Selecione um trabalho e clique em **[!UICONTROL Exibir]** para visualizar o relatório.

   Exibir os detalhes de cada ativo incluído em um job de exclusão. Detalhes como título do ativo, tamanho, autor, status de exclusão e tempo de exclusão são incluídos no relatório. Clique em **[!UICONTROL Baixar]** para baixar o relatório da tarefa no formato CSV.

   O status de exclusão de um ativo no relatório pode ter os seguintes valores possíveis:

   * **Excluído** - O ativo é excluído da pasta Contribuição com êxito.

   * **Não encontrado** - A Brand Portal não pôde localizar o ativo na pasta Contribuição. O ativo já é excluído da pasta manualmente.

   * **Ignorado** - A Brand Portal ignorou a exclusão do ativo, pois há uma nova versão disponível para o ativo na pasta Contribuição, que ainda não foi publicada no Experience Manager.

   * **Falha** - O Brand Portal não pôde excluir o ativo. Há três tentativas de excluir um ativo com um `Failed` excluir status. Se o ativo falhar na terceira tentativa de exclusão, será necessário excluir o ativo manualmente.

### Excluir um relatório

O Brand Portal também permite selecionar um ou vários relatórios e excluí-los manualmente.

Para excluir um relatório:

1. Navegar para **[!UICONTROL Ferramentas]**>**[!UICONTROL Status da contribuição de ativos]**>**[!UICONTROL Relatórios de exclusão]** opção.

1. Selecione um ou mais relatórios e clique em **[!UICONTROL Excluir]**.


