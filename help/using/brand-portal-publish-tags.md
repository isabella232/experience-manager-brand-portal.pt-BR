---
title: Publicar tags no Brand Portal
seo-title: Publicar tags no Brand Portal
description: Saiba como publicar tags dos ativos AEM no Portal da marca.
seo-description: Saiba como publicar tags dos ativos AEM no Portal da marca.
uuid: 4167367 e -1 af 8-476 b -97 a 5-730 c 43 bd 0816
topic-tags: publicação
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referência
discoiquuid: 3 c 8 e 9251-195 d -4 c 56-a 9 a 9-27 bc 8 b 2 a 82 a 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Saiba como publicar tags dos ativos AEM no Portal da marca.

As tags são úteis na organização de ativos e aprimoramento da análise dos ativos aos quais estão associados. As tags podem ser pensadas como palavras-chave ou rótulos (metadados) anexados aos ativos e permitem que os ativos sejam rapidamente encontrados em resultado de uma pesquisa. Para saber como atribuir tags a ativos nos ativos AEM, consulte [Tags para organizar ativos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (associadas a ativos e coleções no AEM) são publicadas automaticamente no Brand Portal quando os ativos (e coleções) com tags associadas são publicados no Brand Portal. As tags publicadas são úteis para ativar as pesquisas para encontrar os ativos associados.

>[!NOTE]
>
>No entanto, é recomendado publicar tags exclusivamente no Brand Portal antes de publicar os ativos (e coleções) com os quais as tags estão associadas. Isso garante uma publicação mais rápida dos ativos (e coleções) no Portal da marca.

## Manage tags {#manage-tags}

Você pode usar as tags pré-existentes para anexar a um ativo ou criar novas tags do console de Tags AEM (**[!UICONTROL Ferramentas | Marcação | Tags AEM]**). Em ambos os cenários, primeiro você deve publicar as tags no Brand Portal e associá-las a ativos apropriados.

Para criar tags no AEM, publique as tags no Brand Portal e associe as tags com os ativos adequados (ou coleções), siga estas etapas:

1. **Criar tags**
Faça logon na instância Autor de AEM com privilégios administrativos e acesse **[!UICONTROL o console de Tags]** do AEM a partir da navegação global:

   1. Selecionar **[!UICONTROL ferramentas]**

   2. Selecionar **[!UICONTROL geral]**

   3. Selecione **[!UICONTROL Marcação]**

2. Selecione **[!UICONTROL Criar]** e selecione **[!UICONTROL Criar tag.]**
3. Especificar:

   * **[!UICONTROL Título]**
      *(obrigatório)* Um título de exibição para a tag.
   * **[!UICONTROL Nome]**
      *(obrigatório)* Um nome para a tag. Se não for especificado, um nome de nó válido será criado a partir do Título. Consulte [tagid](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descrição**
      *(opcional)* Uma descrição da tag.
   * **Caminho**JCR do caminho
de tag da tag.

4. Selecione **[!UICONTROL Enviar]** para criar a tag.

   Após criar uma tag na instância do AEM, a tag estará disponível para ser anexada a um ativo (usando a seção Propriedades ou a seção Gerenciar tags desse ativo).

5. **Publique a tag no Brand Portal**.

   Ir para **[!UICONTROL o console de Tags]** AEM ([!UICONTROL Ferramentas | Marcação | Tags AEM], selecione a tag desejada e publique no Portal da marca.

6. **Anexe a tag a um ativo (ou coleção)**.

   Selecione um ativo (ou coleção) e anexe a tag desejada usando a seção Propriedades ou a seção Gerenciar tags desse ativo. Para saber mais sobre como atribuir tags a ativos nos ativos AEM, consulte [Tags para organizar ativos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publicar ativos (ou coleções) no Portal da marca**.\
   Quando você publica um ativo (ou coleção) no Portal da marca, a tag anexada também está disponível no Brand Portal.

   Para ver a tag anexada no respectivo ativo (ou coleção) no Brand Portal, faça logon no Brand Portal e selecione o ativo, na seção Propriedades, que será visualizado na tag anexada.

## Pesquisar Promover {#search-promote}

O AEM Assets Brand Portal permite que você faça ativos específicos como os principais resultados para pesquisas baseadas em uma tag de palavra-chave.

Para elevar um ativo para uma palavra-chave de pesquisa, siga estas etapas:

1. Abra a página **[!UICONTROL Propriedades]** de um ativo na instância do autor de AEM.
2. Vá até a guia **[!UICONTROL Avançado]** .
3. Na **[!UICONTROL seção Pesquisar promoção]** em **[!UICONTROL Elevar para palavras-chave]** de pesquisa, selecione **[!UICONTROL Adicionar]** para adicionar as palavras-chave de pesquisa ou tags.

   ![](assets/search-promote.png)

4. Salve as alterações.
5. Publicar o ativo no Brand Portal.
6. Faça logon no Brand Portal. Exibir **[!UICONTROL a guia Avançado]** na **[!UICONTROL seção Propriedades]** do ativo.
Observe que a **[!UICONTROL palavra-chave do Search Promote]** também está visível nas Propriedades desse ativo.
