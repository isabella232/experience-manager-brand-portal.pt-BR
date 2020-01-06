---
title: Gerenciar direitos digitais dos ativos
seo-title: Gerenciar direitos digitais dos ativos
description: O licenciamento de ativos e a definição da expiração de ativos e links compartilhados garantem o uso controlado desses ativos e os protegem.
seo-description: O licenciamento de ativos e a definição da expiração de ativos e links compartilhados garantem o uso controlado desses ativos e os protegem.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Gerenciar direitos digitais dos ativos {#manage-digital-rights-of-assets}

Garantir a distribuição e uso seguros dos ativos criativos e do material da marca é vital para proteger sua marca. Isso pode ser aplicado dentro e fora da organização, associando uma data de expiração (e hora) aos ativos aprovados publicados do AEM para o Brand Portal, ou licenciando esses ativos para uso condicional. Além disso, o Brand Portal permite que você especifique uma data de expiração para os links para os ativos compartilhados do Brand Portal.

Leia para saber como os ativos estão protegidos no Brand Portal e entender as permissões de uso associadas.

## Expiração do ativo {#asset-expiration}

A expiração do ativo é uma forma eficaz de controlar o uso dos ativos aprovados no Brand Portal em uma organização. Todos os ativos publicados dos ativos AEM para o Brand Portal podem ter uma data de expiração, o que restringe o uso desses ativos por diferentes funções de usuário.

### Permissões de uso relacionadas a ativos expirados {#usage-permissions-expired-assets}

No Brand Portal, os administradores podem exibir, baixar e adicionar ativos expirados às coleções. Enquanto isso, os editores e visualizadores só podem exibir e adicionar ativos expirados às coleções.

Os administradores podem publicar ativos expirados dos ativos AEM para o Portal de marcas. No entanto, os ativos expirados não podem ser compartilhados via tinta do Brand Portal. Se você selecionar qualquer ativo expirado em uma pasta que contenha ativos expirados e não expirados, a ação **[!UICONTROL Compartilhar link]**não estará disponível. Mas, se você selecionar uma pasta que contenha ativos expirados e não expirados, as ações[!UICONTROL Compartilhar]e**[!UICONTROL  Compartilhar link]** estarão disponíveis.

>[!NOTE]
>
>Uma pasta ainda pode ser compartilhada como um link, mesmo que contenha ativos expirados. Nesse caso, o link não lista ativos expirados e somente os ativos não expirados são compartilhados.

A tabela a seguir exibe as permissões de uso dos ativos expirados:

|  | **[!UICONTROL Compartilhamento de links]** | **[!UICONTROL Download]** | **[!UICONTROL Propriedades]** | **[!UICONTROL Adicionar à coleção]** | **[!UICONTROL Excluir]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrador]** | Indisponível | Disponível | Disponível | Disponível | Disponível |
| **[!UICONTROL Editor]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |
| **[!UICONTROL Visualizador]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |
| **[!UICONTROL Usuário convidado]** | Indisponível | Indisponível | Disponível | Disponível | Indisponível |

>[!NOTE]
>
>Se os visualizadores e editores baixarem uma pasta contendo ativos expirados e não expirados, somente os ativos não expirados serão baixados. Se uma pasta contiver apenas ativos expirados, uma pasta vazia será baixada.

### Estado de vencimento dos ativos {#expiration-status-of-assets}

Você pode exibir o status de expiração dos ativos em sua Visualização **[!UICONTROL de]**cartão. Um sinalizador vermelho no cartão indica que o ativo expirou.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>As exibições de Lista e Coluna não exibem o status de expiração dos ativos.

## Expiração do link do ativo {#asset-link-expiration}

Ao compartilhar ativos por meio de links, os administradores e editores podem definir uma data e hora de expiração usando o campo **[!UICONTROL Expiração]**na caixa de diálogo Compartilhamento**[!UICONTROL  de]** links. A expiração padrão do link é de sete dias a partir da data em que o link é compartilhado.

![](assets/asset-link-sharing.png)

Ela garante que os ativos compartilhados como links expirem na data e hora definidas pelos administradores e editores do Brand Portal, e não poderão mais ser visualizados e baixados além da data de expiração. Como os ativos compartilhados por meio de links também podem ser exibidos por usuários externos que não fazem parte da organização, ao especificar a expiração, você pode garantir que seus ativos aprovados estejam protegidos e não sejam expostos a entidades desconhecidas além de um tempo especificado.

Para obter mais informações sobre o compartilhamento de links, consulte [Compartilhar ativos como um link](../using/brand-portal-link-share.md).

## Ativos licenciados {#licensed-assets}

Os ativos licenciados estão sujeitos à aceitação de um contrato de licença antes do download do Brand Portal. Este contrato para os ativos licenciados vem quando você baixa diretamente o ativo do Brand Portal ou por meio de um link compartilhado. Independentemente de expirar ou não, os ativos protegidos por licença podem ser exibidos por todos os usuários. No entanto, o download e o uso de ativos licenciados expirados são limitados. Para saber mais sobre o comportamento dos ativos licenciados expirados e das atividades permitidas com base nas funções do usuário, consulte as permissões de [uso dos ativos](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)expirados.

Os ativos protegidos por licença têm o contrato de [licença anexado](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) a eles, o que é feito ao configurar a propriedade [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadados do ativo nos ativos AEM.

Se optar por baixar ativos protegidos por licença, você será redirecionado para a página Gerenciamento **[!UICONTROL de]**direitos autorais.

![](assets/asset-copyright-mgmt.png)

Aqui, você precisa selecionar o ativo para baixar e aceitar o contrato de licença associado. Se você não aceitar o contrato de licença, o botão **[!UICONTROL Download]**não estará ativado.

![](assets/licensed-asset-download-2.png)

Se a seleção contiver vários ativos protegidos, selecione um ativo de cada vez, aceite o contrato de licença e continue com o download do ativo.

## Gerar relatório sobre ativos expirados {#generate-report-about-expired-assets}

Os administradores podem gerar e baixar um relatório que lista todos os ativos expirados em um período de tempo específico. Este relatório inclui informação pormenorizada— como tamanho, tipo, caminho que especifica a localização do ativo na hierarquia do ativo, quando o ativo venceu e quando o ativo foi publicado— sobre os ativos expirados. As colunas deste relatório podem ser personalizadas para exibir mais dados com base nos requisitos do usuário.

![](assets/assets-expired.png)

Para obter mais informações sobre o recurso de relatórios, consulte [Trabalhar com relatórios](../using/brand-portal-reports.md#work-with-reports).
