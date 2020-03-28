---
title: Notas de versão
seo-title: Notas de versão
description: Saiba mais sobre os recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos no portal de marcas dos ativos Adobe Experience Manager versão 6.4.6.
seo-description: Saiba mais sobre os aprimoramentos, os problemas críticos corrigidos e os problemas conhecidos no Adobe Experience Manager Assets Brand Portal 6.4.6.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 6b03229b72a1912be57c2bc1b7e47a017d3dca7e

---


# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos no portal de marcas dos ativos Adobe Experience Manager versão 6.4.6.

## Informações da versão {#release-information}

| Produto | Portal de marcas de ativos do Adobe Experience Manager |
|---|---|
| Versão | 6.4.6 |
| Data | Março de 2020 |

## Visão geral {#overview}

O portal de marcas dos ativos Adobe Experience Manager (AEM) ajuda você a adquirir, controlar e distribuir com segurança ativos criativos aprovados para terceiros e usuários empresariais internos em dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, pré-visualizações, baixem e exportem ativos em formatos corporativos aprovados, a qualquer momento e em qualquer lugar.

## Novidades da versão 6.4.6 {#what-s-new-in-646}

### Novos recursos {#new-feature}

Esta versão inclui os seguintes novos recursos:

* Captcha para logon de convidado no Brand Portal. Consulte Acesso [de convidados do Portal de](../using/guest-access.md) marcas para obter mais informações.

### Aprimoramentos {#enhancements-646}

Esta versão do Brand Portal inclui os seguintes aprimoramentos:

* Os ativos AEM agora estão configurados com o Portal de marcas por meio da E/S da Adobe, que obtém um token IMS para autorização do locatário do Portal de marcas.

   >[!NOTE]
   >
   >A configuração por meio do Legacy OAuth não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio da E/S da Adobe.


   >[!TIP]
   >
   >***Somente clientes existentes***
   >
   >É recomendável continuar usando a configuração existente do gateway OAuth. Caso tenha problemas com a configuração antiga do OAuth Gateway, exclua a configuração existente e crie uma nova configuração via E/S da Adobe.


Para obter mais informações, consulte [Configurar ativos AEM com o Portal de marcas](configure-aem-assets-with-brand-portal.md)


### Problemas críticos corrigidos {#critical-issues-fixed}

Esta versão inclui correções para os seguintes problemas críticos:

* Os valores suspensos do schema de metadados não estão visíveis nas propriedades do ativo.

* O subesquema de metadados não exibe guias com base no tipo de mimetype nas propriedades do ativo.

* Cancelar a publicação do schema de metadados preenche uma mensagem de erro, embora o schema seja removido do backend.

* A imagem de Pré-visualização não é exibida para um ativo publicado.

* O usuário não pode publicar ou cancelar a publicação de ativos que contêm aspas simples no nome.

* Os termos e condições não são exibidos durante o download de vários ativos.

* Pequenas vulnerabilidades de segurança abordadas.

### Problemas conhecidos {#known-issues}

Esta versão inclui os seguintes problemas conhecidos:

* Os usuários do Brand Portal não conseguem publicar ativos da pasta de contribuição nos ativos AEM ao atualizar para a E/S da Adobe.

* A opção Excluir representações do sistema não está funcionando corretamente ao baixar um ativo.

## Idiomas {#languages}

A interface de usuário do Brand Portal está disponível nos seguintes idiomas:

* Inglês
* Alemão
* Francês
* Espanhol
* Italiano
* Português do Brasil
* Japonês
* Chinês simplificado
* Coreano

## Plataformas certificadas {#certified-platforms}

Para determinar quais plataformas são certificadas para execução com esta versão do Brand Portal, consulte a coluna **Suporte para interface otimizada para toque na tabela na seção Navegadores** suportados para criação da interface **do usuário dos requisitos** [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)técnicos.

## Links {#links}

* [Página do produto Adobe Experience Manager em adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentação do Portal de marcas de ativos](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente e precisar de acesso, entre em contato com seu gerente de contas da Adobe.

* [](https://daycare.day.com) Acesso ao [produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html)
