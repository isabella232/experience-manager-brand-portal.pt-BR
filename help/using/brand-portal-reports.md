---
title: Trabalhar com relatórios
seo-title: Trabalhar com relatórios
description: Os administradores do Portal de marcas do AEM Assets podem visualização relatórios sobre o uso do Portal de marcas e criar, gerenciar e visualização relatórios sobre os ativos baixados, expirados, publicados e compartilhados por meio do Portal de marcas.
seo-description: Os administradores do Portal de marcas do AEM Assets podem visualização relatórios sobre o uso do Portal de marcas e criar, gerenciar e visualização relatórios sobre os ativos baixados, expirados, publicados e compartilhados por meio do Portal de marcas.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---


# Trabalhar com relatórios {#work-with-reports}

A capacidade do relatórios é fundamental para avaliar o uso do Brand Portal e saber como os usuários internos e externos interagem com os ativos aprovados. Os administradores podem visualização o relatório de uso do portal de marcas, que está sempre disponível na página Relatórios de ativos. No entanto, relatórios de logons de usuário e ativos baixados, expirados, publicados e ativos compartilhados por links podem ser gerados e exibidos na página Relatórios de ativos. Esses relatórios são úteis na análise da implantação de ativos, o que permite que você obtenha métricas principais de sucesso para medir a adoção de ativos aprovados dentro e fora da organização.

A interface de gerenciamento de relatórios é intuitiva e inclui opções e controles aprimorados para acessar relatórios salvos. Você pode visualização, baixar ou excluir relatórios da página Relatórios de ativos, onde todos os relatórios gerados anteriormente são listados.

## Relatórios de Visualização {#view-reports}

Para visualização de um relatório, siga estas etapas:

1. Na barra de ferramentas na parte superior, toque/clique no logotipo do AEM para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Criar/gerenciar relatórios]** para abrir a página Relatórios **[!UICONTROL de]** ativos.

   ![](assets/access-asset-reports.png)

1. Acesse o relatório **[!UICONTROL de uso]** e outros relatórios gerados na página Relatórios de ativos.

   >[!NOTE]
   >
   >O relatório de uso está presente por padrão no Brand Portal. Não pode ser criado ou excluído. Entretanto, você pode criar, baixar e excluir os relatórios Download, Expiração, Publicar, Compartilhamento de links e Logons de usuário.

   Para visualização de um relatório, toque/clique no link do relatório. Como alternativa, selecione o relatório e toque/clique no ícone de Visualização na barra de ferramentas.

   **[!UICONTROL O Relatório]** de uso exibe informações sobre o número de usuários atuais do Brand Portal, o espaço de armazenamento ocupado por todos os ativos e a contagem total de ativos no Brand Portal. O relatório também exibe a capacidade permitida para cada uma dessas métricas de informação.

   ![](assets/usage-report.png)

   **[!UICONTROL O relatório Logons]** de usuário fornece informações sobre os usuários que fizeram logon no Brand Portal. O relatório mostra nomes para exibição, IDs de email, personas (administrador, visualizador, editor, convidado), grupos, último logon, status de atividade e contagem de logon de cada usuário da implantação do Brand Portal 6.4.2 até o momento da geração do relatório.

   ![](assets/user-logins.png)

   **[!UICONTROL Baixe]** listas de relatório e detalhes sobre todos os ativos baixados em um intervalo de data e hora específico.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >O relatório de **[!UICONTROL Download]** de ativos exibe apenas os ativos que foram individualmente selecionados e baixados do Brand Portal. Se um usuário tiver baixado uma pasta que contém ativos, o relatório não exibirá a pasta nem os ativos dentro da pasta.

   **[!UICONTROL O relatório de expiração]** lista e detalha todos os ativos que expiraram em um período de tempo específico.

   ![](assets/expiration-report.png)

   **[!UICONTROL Publique]** listas de relatório e forneça informações sobre todos os ativos publicados do AEM para o Brand Portal em um período de tempo especificado.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publicar relatório não exibe informações sobre fragmentos de conteúdo, pois os fragmentos de conteúdo não podem ser publicados no Brand Portal.

   **[!UICONTROL Relatório]** de compartilhamento de link lista todos os ativos compartilhados por meio de links da interface do Brand Portal em um período específico. O relatório também informa quando o ativo foi compartilhado via link, por meio do qual o usuário, quando o link expira e o número de links compartilhados para o locatário (e os usuários com os quais o link do ativo foi compartilhado). As colunas do Relatório de compartilhamento de links não são personalizáveis.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >O Relatório de compartilhamento de link não exibe os usuários que têm acesso ao ativo compartilhado pelo link ou que baixaram o ativo pelo link.
   >
   >
   >Para rastrear downloads pelo link compartilhado, é necessário gerar um relatório de download depois de selecionar a opção **[!UICONTROL Somente downloads]** de compartilhamento de link na página **[!UICONTROL Criar relatório]** . Entretanto, o usuário (baixado por) é anônimo nesse caso.

## Gerar relatórios {#generate-reports}

Os administradores podem gerar e gerenciar os seguintes relatórios padrão, depois de gerados, eles são salvos para serem [acessados](../using/brand-portal-reports.md#main-pars-header) posteriormente:

* Logons de usuário
* Download
* Expiração
* Publicação
* Compartilhamento de link

As colunas no relatório Download, Expiração e Publicação podem ser personalizadas para exibição. Para gerar um relatório, siga estas etapas:

1. Na barra de ferramentas na parte superior, toque/clique no logotipo do AEM para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, toque/clique em **[!UICONTROL Criar/gerenciar relatórios]** para abrir a página Relatórios **[!UICONTROL de]** ativos.

   ![](assets/asset-reports.png)

1. Na página Relatórios de ativos, toque/clique em **[!UICONTROL Criar]**.
1. Na página **[!UICONTROL Criar relatório]** , selecione um relatório a ser criado e toque/clique em **[!UICONTROL Avançar]**.

   ![](assets/crete-report.png)

1. Configure os detalhes do relatório. Especifique o título, a descrição, a estrutura da pasta (onde o relatório precisa executar e gerar estatísticas) e o intervalo de datas para os relatórios de **[!UICONTROL Download]**, **[!UICONTROL Expiração]** e **[!UICONTROL Publicação]** .

   ![](assets/create-report-page.png)

   Enquanto isso, o Relatório **[!UICONTROL de compartilhamento de]** links precisa apenas dos parâmetros título, descrição e intervalo de datas.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Os caracteres especiais # e % no título do relatório são substituídos por um hífen (-) na geração do relatório.

1. Toque/clique em **[!UICONTROL Avançar]** para configurar as colunas dos relatórios de Download, Expiração e Publicação.
1. Marque ou desmarque as caixas de seleção apropriadas, conforme necessário. Por exemplo, para nomes de visualização de usuários (que baixaram ativos) no relatório **[!UICONTROL Download]** , selecione **[!UICONTROL Baixado por]**. A imagem a seguir ilustra a seleção de colunas padrão no Relatório de download.

   ![](assets/createdownloadreport.png)

   Você também pode adicionar colunas personalizadas a esses relatórios para exibir mais dados para seus requisitos personalizados.

   Para adicionar colunas personalizadas ao Relatório de download, publicação ou expiração, siga estas etapas:

   1. Para exibir uma coluna personalizada, toque/clique em **[!UICONTROL Adicionar]** em Colunas personalizadas.
   1. Especifique o nome da coluna no campo Nome **[!UICONTROL da]** coluna.
   1. Selecione a propriedade para a qual a coluna precisa ser mapeada, usando o seletor de propriedades.

      ![](assets/property-picker.png)
Como alternativa, digite o caminho no campo de caminho da propriedade.

      ![](assets/property-path.png)

      Para adicionar mais colunas personalizadas, toque/clique em **Adicionar** e repita as etapas 2 e 3.

1. Toque/clique em **[!UICONTROL Criar]**. Uma mensagem notifica que a geração de relatórios foi iniciada.

## Download de relatórios {#download-reports}

Para salvar e baixar um relatório como arquivo .csv, execute um dos procedimentos a seguir:

* Selecione um relatório na página Relatórios de ativos e toque/clique em **[!UICONTROL Download]** na barra de ferramentas na parte superior.

![](assets/download-asset-report.png)

* Na página Relatórios de ativos, abra um relatório. Selecione a opção **[!UICONTROL Download]** na parte superior da página do relatório.

![](assets/download-report-fromwithin.png)

## Excluir relatórios {#delete-reports}

Para excluir um relatório existente, selecione o relatório na página Relatórios **[!UICONTROL de]** ativos e toque/clique em **[!UICONTROL Excluir]** na barra de ferramentas na parte superior.

>[!NOTE]
>
>**[!UICONTROL O relatório de uso]** não pode ser excluído.
