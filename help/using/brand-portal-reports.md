---
title: Trabalhar com relatórios
seo-title: Trabalhar com relatórios
description: Os administradores do AEM Assets Brand Portal podem visualizar o relatório sobre uso do Brand Portal e criar, gerenciar e exibir relatórios nos ativos baixados, expirados, publicados e compartilhados por meio do Brand Portal.
seo-description: Os administradores do AEM Assets Brand Portal podem visualizar o relatório sobre uso do Brand Portal e criar, gerenciar e exibir relatórios nos ativos baixados, expirados, publicados e compartilhados por meio do Brand Portal.
uuid: dc 4 e 5275-a 614-4 b 95-8 c 70-2 b 7 e 470 c 50 a 7
content-type: referência
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 7683074 f-b 6 ea -42 e 0-a 411-3 b 13 eb 88 d 1 f 2
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Trabalhar com relatórios {#work-with-reports}

O recurso de relatório é instrumente na avaliação [!DNL Brand Portal] de uso e sabendo como os usuários internos e externos interagem com ativos aprovados. Os administradores podem exibir [!DNL Brand Portal] o Relatório de uso, que está sempre disponível na página Relatórios de ativos. No entanto, os relatórios de logons de usuário e ativos baixados, expirados, publicados e ativos compartilhados por links podem ser gerados e exibidos a partir da página de Relatórios de ativo. Esses relatórios são úteis na análise da implantação de ativos, que permite que você derive métricas-chave de sucesso para medir a adoção de ativos aprovados dentro e fora da organização.

A interface de gerenciamento de relatórios é intuitiva e inclui opções e controles refinados para acessar relatórios salvos. Você pode exibir, baixar ou excluir relatórios da página Relatórios de ativos, onde todos os relatórios gerados anteriormente são listados.

## Exibir relatórios {#view-reports}

Para exibir um relatório, siga estas etapas:

1. Na barra de ferramentas na parte superior, toque/clique no [!DNL AEM] logotipo para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, clique **em Criar/gerenciar relatórios** para abrir a página** Relatórios de ativo**.

   ![](assets/access-asset-reports.png)

3. Acesso **de** acesso e outros relatórios gerados a partir da página Relatórios de ativos.

   >[!NOTE]
   >
   >O relatório de uso está presente por padrão [!DNL Brand Portal]. Ele não pode ser criado ou excluído. No entanto, você pode criar, baixar e excluir os relatórios Download, Expiração, Publicação, Compartilhamento de links e Logons de usuário.

   Para exibir um relatório, toque/clique no link do relatório. Como alternativa, selecione o relatório e toque/clique no ícone Exibir na barra de ferramentas.

   **O Relatório** de uso exibe informações sobre o número de [!DNL Brand Portal] usuários atuais, o espaço de armazenamento ocupado por todos os ativos e o total de ativos em [!DNL Brand Portal]. O relatório também exibe a capacidade permitida para cada uma dessas métricas de informações.

   ![](assets/usage-report.png)

   **O relatório de logons** de usuário fornece informações sobre os usuários aos quais [!DNL Brand Portal]fizeram logon. O relatório mostra nomes de exibição, IDs de e-mail, personalizados (administrador, visualizador, editor, convidado), grupos, último logon, status da atividade e contagem de login de cada usuário da [!DNL Brand Portal] implantação 6.4.2 até o momento da geração do relatório.

   ![](assets/user-logins.png)

   **Baixe** listas de relatórios e detalhes sobre todos os ativos baixados em uma data e hora específicas.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >O relatório de ativos** Download** exibe somente os ativos que foram individualmente selecionados e baixados [!DNL Brand Portal]. Se um usuário tiver baixado uma pasta que contém ativos, o relatório não exibirá a pasta ou os ativos dentro dela.

   **O relatório de expiração** lista e detalha todos os ativos que expiram em um intervalo de tempo específico.

   ![](assets/expiration-report.png)

   **Publicar** relatório lista e fornece informações sobre todos os ativos publicados em [!DNL AEM] um intervalo [!DNL Brand Portal] de tempo especificado.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publicar relatório não exibe informações sobre fragmentos do conteúdo, já que os fragmentos do conteúdo não podem ser publicados no [!DNL Brand Portal].

   **O relatório** de compartilhamento de link lista todos os ativos compartilhados pelos links da [!DNL Brand Portal] interface em um período específico. O relatório também informa quando foi o ativo compartilhado por link, por qual usuário, quando o link expira e o número de links compartilhados para o inquilino (e usuários com os quais o link de ativo foi compartilhado). As colunas do Relatório de compartilhamento de link não são personalizáveis.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >O Relatório de compartilhamento de links não exibe os usuários que têm acesso ao ativo compartilhado por meio do link ou baixaram o ativo por meio do link.
   >
   >
   >Para rastrear downloads por meio do link compartilhado, é necessário gerar o relatório de download depois de selecionar **Somente a opção Downloads** de compartilhamento de links na **página Criar relatório** . No entanto, o usuário (Baixado por) é anônimo nesse caso.

## Gerar relatórios {#generate-reports}

Os administradores podem gerar e gerenciar os seguintes relatórios padrão, após serem gerados, eles serão salvos para [serem acessados](../using/brand-portal-reports.md#main-pars-header) posteriormente:

* Logons de usuário
* Download
* Expiração
* Publicação
* Compartilhamento de link

As colunas no relatório Download, Expiração e Publicação podem ser personalizadas para exibição. Para gerar um relatório, siga estas etapas:

1. Na barra de ferramentas na parte superior, toque/clique no [!DNL AEM] logotipo para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

2. No painel de ferramentas administrativas, toque/clique **em Criar/gerenciar relatórios** para abrir a página** Relatórios de ativo**.

   ![](assets/asset-reports.png)

3. Na página Relatórios de ativos, toque/clique **em Criar**.
4. Na página **Criar relatório** , selecione um relatório a ser criado e toque/clique **em Avançar**.

   ![](assets/crete-report.png)

5. Configure os detalhes do relatório. Especifique título, descrição, estrutura de pastas (onde o relatório precisa executar e gerar estatísticas) e o intervalo de datas para **relatórios de Download**, **Expiração** e **Publicação** .

   ![](assets/create-report-page.png)

   Considerando que o **Relatório** de compartilhamento de link precisa apenas do título, descrição e parâmetros de intervalo de datas.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Caracteres especiais # e % no título do relatório são substituídos por um hífen (-) na geração do relatório.

6. Toque/clique **em Avançar**, para configurar as colunas de relatórios de Download, Expiração e Publicação.
7. Marque ou desmarque as caixas de seleção apropriadas conforme necessário. Por exemplo, para exibir nomes de usuários (que baixaram ativos) no **Relatório Download** , selecione **Baixado por**. A imagem a seguir ilustra a seleção de colunas padrão no Relatório de download.

   ![](assets/createdownloadreport.png)

   Você também pode adicionar colunas personalizadas a esses relatórios para exibir mais dados para seus requisitos personalizados.

   Para adicionar colunas personalizadas a Download, publicação ou expiração do relatório, siga estas etapas:

   1. Para exibir uma coluna personalizada, toque/clique **em Adicionar** em **Colunas personalizadas**.
   2. Especifique o nome da coluna no **campo Nome** da coluna.
   3. Selecione a propriedade à qual a coluna precisa mapear, usando o seletor de propriedades.

      ![](assets/property-picker.png)Como alternativa, digite o caminho no campo caminho da propriedade.

      ![](assets/property-path.png)

      Para adicionar mais colunas personalizadas, toque/clique **em Adicionar** e repita as etapas 2 e 3.

8. Toque/clique em **Criar**. Uma mensagem notifica que a geração de relatórios foi iniciada.

## Download de relatórios {#download-reports}

Para salvar e baixar um relatório como arquivo. csv, execute um dos seguintes procedimentos:

* Selecione um relatório na página Relatórios de ativos e toque/clique **em Download** na barra de ferramentas na parte superior.

![](assets/download-asset-report.png)

* Na página Relatórios de ativos, abra um relatório. Selecione **a opção Download** na parte superior da página do relatório.

![](assets/download-report-fromwithin.png)

## Excluir relatórios {#delete-reports}

Para excluir um relatório existente, selecione o relatório da **página Relatórios** de ativos e toque/clique **em Excluir** na barra de ferramentas na parte superior.

>[!NOTE]
>
>**O relatório de uso** não pode ser excluído.
