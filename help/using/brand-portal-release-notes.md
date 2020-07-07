---
title: Notas de versão
seo-title: Notas de versão
description: Saiba mais sobre os recursos, melhorias, problemas críticos corrigidos e problemas conhecidos no Adobe Experience Manager Assets Brand Portal 6.4.6.2.
seo-description: Saiba mais sobre os aprimoramentos, problemas críticos corrigidos e problemas conhecidos no Adobe Experience Manager Assets Brand Portal 6.4.6.2.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 8%

---


# Notas de versão {#release-notes}

Saiba mais sobre os novos recursos, aprimoramentos, problemas críticos corrigidos e problemas conhecidos no Adobe Experience Manager Assets Brand Portal 6.4.6.2.

## Informações da versão {#release-information}

| Produto | Portal de marcas dos ativos Adobe Experience Manager |
|---|---|
| Versão | 6.4.6.2 |
| Data | Junho de 2020 |

## Visão geral {#overview}

O Portal de marcas de ativos Adobe Experience Manager (AEM) ajuda você a adquirir, controlar e distribuir com facilidade ativos criativos aprovados para terceiros externos e usuários empresariais internos em dispositivos. Ajuda a melhorar a eficiência do compartilhamento de ativos, acelera o tempo de comercialização dos ativos e reduz o risco de não conformidade e acesso não autorizado. O Brand Portal permite que os usuários naveguem, pesquisem, pré-visualizações, baixem e exportem ativos em formatos corporativos aprovados, a qualquer momento e em qualquer lugar.

## Novidades da versão 6.4.6.2 {#what-s-new-in-6462}

### Problemas críticos corrigidos {#critical-issues-fixed-6462}

Esta versão inclui correções para os seguintes problemas críticos:

* Remover um schema de metadados publicado do Brand Portal resulta em um erro.

* Se o administrador configurar o Experience Manager Assets 6.5.4 com o Brand Portal por meio do Adobe Developer Console, o usuário do Brand Portal não poderá publicar os ativos da pasta de contribuição do Brand Portal para o Experience Manager.

* Replicação de Duplicado das pastas pai que causam conflitos.

* O usuário não consegue gerar o relatório de compartilhamento de link.

* O usuário pode copiar segredos MAC para um terminal do Brand Portal usando o comando copyPage.

* cqTags que causam reindexação no clone VA5.


### Problemas conhecidos {#known-issues-6462}

Esta versão inclui os seguintes problemas conhecidos:

* Se uma pasta na hierarquia for renomeada de AEM Assets e a pasta aninhada que contém um ativo for publicada no Brand Portal, o título da pasta não será atualizado no Brand Portal até que a pasta raiz seja publicada novamente.


## Novidades da versão 6.4.6 {#what-s-new-in-646}

### New Features {#new-feature}

Esta versão inclui os seguintes novos recursos:

* Captcha para logon de convidado no Brand Portal. See, [Brand Portal guest access](../using/guest-access.md) for more information.

* O Brand Portal agora é compatível com o serviço em nuvem do AEM Assets. Você pode configurar que os AEM Assets podem trabalhar com o Brand Portal para compartilhar e distribuir ativos com os usuários do Brand Portal.
Para obter mais informações, consulte [Configurar o serviço em nuvem do AEM Assets com o Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html).

### Aprimoramentos {#enhancements-646}

Esta versão do Brand Portal inclui os seguintes aprimoramentos:

* No AEM 6.3 e superior, o canal de autorização entre o AEM Assets e o Portal de marcas é alterado. O AEM Assets agora está configurado com o Brand Portal por meio do Adobe Developer Console, que obtém um token IMS para autorização do locatário do Brand Portal.

>[!NOTE]
>
>A configuração por meio do Legacy OAuth não é mais compatível a partir de 6 de abril de 2020 e é alterada para configuração por meio do Adobe Developer Console.

>[!TIP]
>
>***Somente para clientes existentes***
>
>A configuração antiga do OAuth Gateway continuará funcionando para os clientes existentes.
>
>Caso encontre problemas com a configuração herdada do OAuth Gateway, exclua a configuração existente e crie uma nova configuração por meio do Adobe Developer Console.

For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

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

* Os usuários do Brand Portal não conseguem publicar ativos da pasta de contribuição em AEM Assets ao atualizar para o Adobe Developer Console no AEM 6.5.4.

   Esse problema será corrigido no próximo service pack 6.5.5.

   Para corrigir imediatamente o AEM 6.5.4, é recomendável [baixar a correção](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalá-la na instância do autor.

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
* [Documentação do Portal de marcas de ativos](https://helpx.adobe.com/br/experience-manager/brand-portal/user-guide.html)

## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente e precisar de acesso, entre em contato com seu gerente de contas da Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Acesso ao produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html)
