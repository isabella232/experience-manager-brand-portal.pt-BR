---
title: Configurar propriedades da pasta Contribuição
seo-title: Configurar propriedades da pasta Contribuição
description: 'Obtenha informações sobre como configurar as propriedades de uma pasta de contribuição no AEM Assets. '
seo-description: 'Obtenha informações sobre como configurar as propriedades de uma pasta de contribuição no AEM Assets. '
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
version: 6.5
discoiquuid: null
translation-type: tm+mt
source-git-commit: d0c5adad47fdc83adfad79bae4119cb6d38caf5e
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Configurar as propriedades da pasta de contribuição {#configure-contribution-folder-properties}

O administrador do AEM executa as seguintes atividades ao configurar as propriedades de uma pasta de contribuição.

* **Adicionar descrição**: Forneça uma descrição de alto nível da pasta de contribuição.
* **Resumo** do upload:  Faça upload do documento de requisito de ativo que contém informações relacionadas ao ativo.
* **Adicionar colaboradores**: Adicione usuários ou grupos do Brand Portal para conceder acesso à pasta de contribuição.

O requisito de ativo se refere aos detalhes fornecidos pelos administradores para ajudar os contribuidores (usuários do Brand Portal) a entender a necessidade e os requisitos da pasta de contribuição. O administrador carrega um documento de requisito de ativo que contém um resumo sobre o tipo de ativos que devem ser adicionados à pasta de contribuição e às informações relacionadas ao ativo, por exemplo, finalidade, tipo de imagens, tamanho máximo etc.

O administrador pode conceder acesso aos usuários/grupos do Brand Portal à pasta de contribuição antes de publicar a pasta de contribuição recém-criada no Brand Portal.

**Para configurar as propriedades da pasta de contribuição:**
1. Faça logon na instância do autor de AEMURL padrão: http:// localhost:4502/aem/start.html
1. Navegue até **[!UICONTROL Ativos > Arquivos]** e localize a pasta de contribuição.
1. Selecione a pasta de contribuição e clique em **[!UICONTROL Propriedades]** ![](assets/properties.png). A janela de propriedades da pasta é aberta.
   ![](assets/contribution-folder-property1.png)
1. Navegue até a guia Contribuição **[!UICONTROL do]** ativo.
1. Digite a **[!UICONTROL Descrição]** de alto nível da pasta de contribuição.
1. Clique em **[!UICONTROL Carregar resumo]** ![](assets/upload.png) para navegar pelo computador local e fazer upload de um Documento **de requisitos de** ativos.
1. Em **[!UICONTROL Adicionar usuário ou grupo]**, pesquise e **[!UICONTROL adicione]** usuários do Brand Portal com os quais você deseja compartilhar a pasta de contribuição. Uma pasta de contribuição não pode ser atribuída a grupos.
Esses usuários do Brand Portal terão permissão para acessar a pasta de contribuição e fazer upload do conteúdo da interface do Brand Portal sem precisar acessar a instância do autor do AEM.

1. Clique em **[!UICONTROL Salvar]**.
   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>Os resultados da pesquisa são baseados na lista de usuário do Brand Portal configurada no AEM Assets. Verifique se você tem a lista atualizada do usuário do Brand Portal. Consulte [Fazer upload da lista](brand-portal-configure-asset-sourcing.md)do usuário do Brand Portal.

