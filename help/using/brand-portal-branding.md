---
title: Personalizar papel de parede, cabeçalho e mensagens de e-mail
seo-title: Customize wallpaper, header, and email message
description: Os administradores do Brand Portal podem fazer personalizações limitadas na interface exibida aos usuários. Você pode escolher uma imagem de fundo (wallpaper) específica para a página de logon do Brand Portal. Você também pode adicionar uma imagem de cabeçalho e personalizar os emails de compartilhamento de ativos para corresponder à marca do cliente.
seo-description: Brand Portal administrators can make limited customizations to the interface displayed to users. You can choose a specific background image (wallpaper) for the Brand Portal login page. You can also add a header image and customize asset sharing emails to match the customer’s brand.
uuid: e078d0b9-18b5-467a-ae90-7f0b9fd0d414
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 7b573a4f-2d4e-48d6-b259-436d0cfbdce9
role: Admin
exl-id: 9f5c2a6a-8844-4ca4-b0d9-8f50b6164219
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 2%

---

# Personalizar papel de parede, cabeçalho e mensagens de e-mail {#customize-wallpaper-header-and-email-message}

Os administradores do Brand Portal podem fazer personalizações limitadas na interface exibida aos usuários. Você pode escolher uma imagem de fundo (wallpaper) específica para a página de logon do Brand Portal. Você também pode adicionar uma imagem de cabeçalho e personalizar os emails de compartilhamento de ativos para corresponder à marca do cliente.

## Personalizar o papel de parede da tela de logon {#customize-the-login-screen-wallpaper}

Na ausência de uma imagem de papel de parede personalizada, um papel de parede padrão é exibido na página de logon.

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Marcas]**.


   ![](assets/admin-tools-panel-10.png)

1. No painel esquerdo do **[!UICONTROL Configurar marca]** página, **[!UICONTROL Papel de parede]** é selecionada por padrão. A imagem de fundo padrão que aparece na página de logon é exibida.

   ![](assets/default_wallpaper.png)

1. Para adicionar uma nova imagem de plano de fundo, clique no **[!UICONTROL Escolher imagem]** ícone na barra de ferramentas na parte superior.

   ![](assets/choose_wallpaperimage.png)

   Siga uma das seguintes opções:

   * Para carregar uma imagem do seu computador, clique em **[!UICONTROL Carregar]**. Navegue até a imagem desejada e faça upload dela.
   * Para usar uma imagem existente do Brand Portal, clique em **[!UICONTROL Selecionar a partir de existentes]**. Escolha uma imagem usando o seletor de ativos.

   ![](assets/asset-picker.png)

1. Especifique um texto de cabeçalho e uma descrição para a imagem do plano de fundo. Para salvar as alterações, clique **[!UICONTROL Salvar]** na barra de ferramentas na parte superior.

1. Na barra de ferramentas na parte superior, clique no botão **[!UICONTROL Visualizar]** ícone para gerar uma pré-visualização da interface do Brand Portal com a imagem.

   ![](assets/chlimage_1.png)

   ![](assets/custom-wallpaper-preview.png)

1. Para ativar ou desativar o papel de parede padrão, faça o seguinte no **[!UICONTROL Configurar marca > Papel de parede]** página:

   * Para exibir a imagem de wallpaper padrão na página de logon do Brand Portal, clique em **[!UICONTROL Desativar papel de parede]** na barra de ferramentas na parte superior. Uma mensagem confirma que a imagem personalizada está desativada.

   ![](assets/chlimage_1-1.png)

   * Para restaurar a imagem personalizada na página de logon do Brand Portal, clique em **[!UICONTROL Ativar papel de parede]** na barra de ferramentas. Uma mensagem confirma que a imagem está restaurada.

   ![](assets/chlimage_1-2.png)

   * Clique em **[!UICONTROL Salvar]** para salvar as alterações.



## Personalizar o cabeçalho {#customize-the-header}

O cabeçalho é exibido em várias páginas do Brand Portal depois de fazer logon no Brand Portal.

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Marcas]**.

   ![](assets/admin-tools-panel-11.png)

1. Para personalizar o cabeçalho da página para a interface do Brand Portal, no **[!UICONTROL Configurar marca]** selecione **[!UICONTROL Imagem do cabeçalho]** do painel esquerdo. A imagem do cabeçalho padrão é exibida.

   ![](assets/default-header.png)

1. Para fazer upload de uma imagem de cabeçalho, clique no **[!UICONTROL Escolher imagem]** e escolha **[!UICONTROL Carregar]**.

   Para usar uma imagem existente do Brand Portal, escolha **[!UICONTROL Selecionar a partir de existentes]**.

   ![](assets/choose_wallpaperimage-1.png)

   Escolha uma imagem usando o seletor de ativos.

   ![](assets/asset-picker-header.png)

1. Para incluir um URL na imagem de cabeçalho, especifique-o na tag **[!UICONTROL URL da imagem]** caixa. Você pode especificar URLs externos ou internos. Links internos também podem ser links relativos, por exemplo,
   [!UICONTROL `/mediaportal.html/content/dam/mac/tenant_id/tags`].
Esse link direciona os usuários para a pasta de tags.
Para salvar as alterações, clique **[!UICONTROL Salvar]** na barra de ferramentas na parte superior.

   ![](assets/configure_brandingheaderimageurl.png)

1. Na barra de ferramentas na parte superior, clique no botão **[!UICONTROL Visualizar]** ícone para gerar uma pré-visualização da interface do Brand Portal com a imagem do cabeçalho.

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

1. Para ativar ou desativar a imagem de cabeçalho, faça o seguinte no **[!UICONTROL Configurar marca > Imagem do cabeçalho]** página:

   * Para evitar que uma imagem de cabeçalho seja exibida em páginas do Brand Portal, clique em **[!UICONTROL Desativar cabeçalho]** na barra de ferramentas na parte superior. Uma mensagem confirma que a imagem está desativada.

   ![](assets/chlimage_1-4.png)

   * Para fazer com que a imagem de cabeçalho reapareça nas páginas do Brand Portal, clique em **[!UICONTROL Ativar cabeçalho]** na barra de ferramentas na parte superior. Uma mensagem confirma que a imagem está ativada.

   ![](assets/chlimage_1-5.png)

   * Clique em **[!UICONTROL Salvar]** para salvar as alterações.



## Personalizar as mensagens de email {#customize-the-email-messaging}

Quando os ativos são compartilhados como um link, os usuários recebem um email contendo o link. Os administradores podem personalizar as mensagens, ou seja, o logotipo, a descrição e o rodapé desses emails.

1. Na barra de ferramentas na parte superior, clique no logotipo do Experience Manager para acessar as ferramentas administrativas.

   ![](assets/aemlogo.png)

1. No painel de ferramentas administrativas, clique em **[!UICONTROL Marcas]**.

   ![](assets/admin-tools-panel-12.png)

1. Quando os ativos são compartilhados como links ou baixados por emails e quando  **[!UICONTROL coleções]** forem compartilhadas, as notificações por email serão enviadas aos usuários. Para personalizar a mensagem de email, no **[!UICONTROL Configurar marca]** selecione **[!UICONTROL Mensagem de email]** do painel esquerdo.

   ![](assets/configure-branding-page-email.png)

1. Para adicionar um logotipo a emails de saída, clique em **[!UICONTROL Carregar]** na barra de ferramentas na parte superior.

1. No **[!UICONTROL Descrição]** especifique o texto do cabeçalho e do rodapé do email. Para salvar as alterações, clique **[!UICONTROL Salvar]** na barra de ferramentas na parte superior.

   >[!NOTE]
   >
   >Se você não usar o tamanho recomendado para o logotipo ou se o texto do cabeçalho e rodapé exceder a contagem de palavras recomendada, o conteúdo da mensagem de email poderá parecer ilegível.
