---
title: Gerenciar direitos digitais de ativos
seo-title: Gerenciar direitos digitais de ativos
description: Ativos de licenciamento e configuração de expiração para ativos e links compartilhados garantem o uso controlado desses ativos e protegem-os.
seo-description: Ativos de licenciamento e configuração de expiração para ativos e links compartilhados garantem o uso controlado desses ativos e protegem-os.
uuid: ce 30 e 398-0109-41 bf-a 4 d 2-2 fcca 476 f 499
contentOwner: bdhar
topic-tags: download-instalação
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
discoiquuid: f 77003 ba -31 fe -4 a 9 e -96 c 8-dbc 4 c 2 eba 79 e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Gerenciar direitos digitais de ativos {#manage-digital-rights-of-assets}

Garantir a distribuição e o uso seguros de ativos criativos e o material da marca é vital para proteger sua marca. Isso pode ser aplicado em toda a organização e fora dele ao associar uma data de expiração (e hora) com os ativos aprovados publicados do AEM para o Brand Portal ou ao licenciar esses ativos para uso condicional. Além disso, o Brand Portal permite especificar uma data de expiração para os links para os ativos compartilhados do Brand Portal.

Faça a leitura para saber como os ativos são protegidos no Brand Portal e compreender as permissões de uso associadas.

## Expiração do ativo {#asset-expiration}

A expiração do ativo é uma forma eficaz de controlar o uso de ativos aprovados no Brand Portal em uma organização. Todos os ativos publicados no AEM Assets para o Brand Portal podem ter uma data de expiração, que restringe o uso desses ativos por diferentes funções de usuário.

### Permissões de uso relacionadas aos ativos expirados {#usage-permissions-expired-assets}

No Brand Portal, os administradores podem visualizar, baixar e adicionar ativos expirados às coleções. Enquanto os Editores e Visualizadores podem apenas visualizar e adicionar ativos expirados às coleções.

Os administradores podem publicar ativos expirados do AEM Assets no Portal da marca. No entanto, os ativos expirados não podem ser compartilhados por tinta do Brand Portal. Se você selecionar qualquer ativo expirado de uma pasta contendo ativos expirados ou não expirados, a ação **[!UICONTROL Compartilhar link]** não estará disponível. Mas, se você selecionar uma pasta que contém ativos expirados e não expirados, as ações [!UICONTROL Compartilhar] e **[!UICONTROL Compartilhar link]** estarão disponíveis.

>[!NOTE]
>
>Uma pasta ainda pode ser compartilhada como um link, mesmo que contenha ativos expirados. Nesse caso, o link não lista ativos expirados e somente os ativos não expirados são compartilhados.

A tabela a seguir exibe as permissões de uso dos ativos expirados:

|  | **[!UICONTROL Compartilhar compartilhamento]** | **[!UICONTROL Download]** | **[!UICONTROL Propriedades]** | **[!UICONTROL Adicionar à coleção]** | **[!UICONTROL Excluir]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrador]** | Indisponível | Disponível | Disponível | Disponível | Disponível |
| **[!UICONTROL Editor]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |
| **[!UICONTROL Visualizador]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |
| **[!UICONTROL Usuário convidado]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |

>[!NOTE]
>
>Se os Visualizadores e editores baixarem uma pasta contendo ativos expirados e não expirados, somente os ativos não expirados serão baixados. Se uma pasta contiver apenas ativos expirados, será baixada uma pasta vazia.

### Status de expiração dos ativos {#expiration-status-of-assets}

É possível exibir o status de expiração dos ativos na exibição [!UICONTROL de cartão]. Um sinalizador vermelho no cartão indica que o ativo expirou.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>As exibições de lista e coluna não exibem o status de expiração dos ativos.

## Expiração do link de ativos {#asset-link-expiration}

Ao compartilhar ativos por meio de links, os administradores e editores podem definir uma data e hora de expiração usando o campo **[!UICONTROL Expiração]** na caixa de diálogo **[!UICONTROL Compartilhamento]** de links. A expiração padrão do link é sete dias a partir da data em que o link é compartilhado.

![](assets/asset-link-sharing.png)

Isso garante que os ativos compartilhados como links expiram na data e hora definidos pelos Administradores e Editores do Brand Portal, e não podem mais ser visualizados e baixados além da data de expiração. Como os ativos compartilhados por links também podem ser exibidos por usuários externos que não fazem parte da organização, ao especificar a expiração, você pode garantir que os ativos aprovados sejam protegidos e não expostos a entidades desconhecidas além de um tempo especificado.

Para obter mais informações sobre compartilhamento de links, consulte [Compartilhar ativos como um link](../using/brand-portal-link-share.md).

## Ativos licenciados {#licensed-assets}

Os ativos licenciados estão sujeitos à aceitação de um contrato de licença antes do download do Portal da marca. Esse contrato para ativos licenciados ocorre quando você baixa diretamente o ativo do Portal da marca ou por um link compartilhado. Se expirar ou não expirar, os ativos protegidos por licença podem ser exibidos por todos os usuários. No entanto, o download e o uso dos ativos licenciados expirados são limitados. Para saber sobre o comportamento dos ativos licenciados e atividades permissíveis expirados com base nas funções do usuário, consulte as permissões [de uso dos ativos expirados](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Os ativos protegidos por licença possuem [contrato de licença anexado](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) a eles, o que é feito pela definição da propriedade [de metadados do ativo](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) nos ativos AEM.

Se você optar por baixar ativos protegidos por licença, será redirecionado para [!UICONTROL a página Gerenciamento] de direitos autorais.

![](assets/asset-copyright-mgmt.png)

Aqui, você precisa selecionar o ativo para baixar e aceitar o contrato de licença associado. Se você não aceitar o contrato de licença, o botão [!UICONTROL Download] não estará ativado.

![](assets/licensed-asset-download-2.png)

Se a seleção contiver vários ativos protegidos, selecione um ativo por vez, aceite o contrato de licença e prossiga para baixar o ativo.

## Gerar relatório sobre ativos expirados {#generate-report-about-expired-assets}

Os administradores podem gerar e baixar um relatório que lista todos os ativos expirados em um período específico. Este relatório inclui informações detalhadas, como tamanho, tipo, caminho especificando o local do ativo na hierarquia do ativo, quando o ativo expira e quando foi o ativo publicado— sobre os ativos expirados. As colunas deste relatório podem ser personalizadas para exibir mais dados com base nos requisitos do usuário.

![](assets/assets-expired.png)

Para obter mais informações sobre o recurso de relatórios, consulte [Trabalhar com relatórios](../using/brand-portal-reports.md#work-with-reports).
