---
title: Perguntas frequentes
seo-title: null
description: Saiba mais sobre as perguntas frequentes no Portal de marcas de ativos do Adobe Experience Manager.
seo-description: null
uuid: null
content-type: reference
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f8d95ab1e1c17ef2cf86d0206a36134996e4fe07

---


# Perguntas frequentes {#frequently-asked-questions}

As Perguntas frequentes do Brand Portal se concentram nas consultas e problemas que os usuários finais podem encontrar ao trabalhar com a versão mais recente do AEM Assets Brand Portal 6.4.5 ou versões anteriores.



**Ques. Qual é a grande mudança na versão 6.4.5 do Brand Portal?**

**Ans.** O AEM Assets Brand Portal 6.4.5 é uma versão de recurso que permite que os usuários do Brand Portal façam upload de conteúdo dentro da instância do Brand Portal e publiquem a pasta Contribuição de volta nos ativos AEM sem precisar de direitos de administrador.
Para obter mais informações, consulte Seleção de [recursos no Portal](brand-portal-asset-sourcing.md)da marca.



**Ques. Perderei o acesso a ativos, recursos ou configurações existentes que criei?**

**Ans.** Todos os recursos e configurações existentes permanecem intactos. Seus usuários finais não são afetados e seu conteúdo permanece intacto.



**Ques. Quando eu vou mudar para a nova versão do Brand Portal?**

**Ans.** O Brand Portal 6.4.5 foi lançado para produção em outubro de 2019. E a próxima versão do Brand Portal deverá ser lançada no terceiro trimestre de 2020.
Para atualizações e alterações de versão, é recomendável rastrear as Notas [de](brand-portal-release-notes.md) versão e [Novidades do Brand Portal](whats-new.md).



**Ques. Meus usuários serão afetados?**

**Ans.** A versão do Brand Portal 6.4.5 está exclusivamente no Brand Portal, portanto não há impacto para os usuários finais.



**Ques. Há alguma ação necessária da minha parte como usuário do Brand Portal?**

**Ans.** A versão 6.4.5 do Brand Portal vem com um novo recurso chamado Asset Sourcing. O administrador do AEM deve configurar o recurso de Seleção de ativos nos ativos AEM para ativar o recurso para os usuários do Brand Portal. Para obter mais informações, consulte [Ativar fonte](brand-portal-configure-asset-sourcing.md)de ativos.



**Ques. Quem pode criar uma pasta de contribuição?**

**Ans.** Qualquer usuário do AEM pode criar uma nova pasta nos ativos AEM e atribuir a propriedade **Asset Contribution**. A pasta recém-criada é chamada de pasta **Contribuição** .
Essa pasta é compartilhada com os usuários ativos do Brand Portal para obter contribuição.



**Ques. O que uma pasta de contribuição contém?**

**Ans.** A pasta **Contribution** contém duas subpastas **NEW** e **SHARED**. Inicialmente, a pasta NEW está em branco e a pasta SHARED contém o conteúdo de referência (ativos reutilizáveis) para os usuários do Brand Portal.
Os usuários do Brand Portal acessam a pasta **Contribution** e carregam conteúdo na pasta **NEW** .



**Ques. Quais são os requisitos de ativos com contribuição de r l'r?**

**Ans.** O documento **Breve** anexado à pasta **Contribution** e o conteúdo de referência (ativos reutilizáveis) carregado na pasta **SHARED** ajuda o usuário do Brand Portal a entender a necessidade de contribuição e expectativas como colaborador e é chamado coletivamente de requisitos de ativos.



**Ques. É possível fazer upload de ativos para qualquer pasta permitida?**

**Ans.** Nem todas as pastas permitidas. Um usuário do Brand Portal só pode carregar conteúdo para a pasta **Contribution** compartilhada pelo administrador do AEM ou do Brand Portal.



**Ques. Como obtenho acesso a uma pasta de contribuição?**

**Ans.** Você pode acessar uma pasta **de contribuição** somente se ela tiver sido compartilhada com você. Você receberá uma notificação por email/pulsação sempre que uma pasta de contribuição for compartilhada com você. Você pode acessar a pasta Contribuição por meio do link compartilhado no e-mail ou fazer logon na instância do Brand Portal e navegar até o ícone de sinalizador para obter notificações para acessar a pasta Contribuição.

>[!NOTE]
>
>Se você não for um usuário do Brand Portal, solicite ao administrador do AEM que crie seu usuário no Admin Console do AEM e adicione seu perfil ao arquivo de configuração do usuário na lista de usuários do Brand Portal. Consulte, [Adicionar usuário](brand-portal-configure-asset-sourcing.md)do Brand Portal.



**Ques. Qual é o Formato do arquivo CSV para importação de usuário?**

**Ans.** O formato é o mesmo que o Admin Console suporta para importação de usuários em massa. Email, nome e sobrenome são obrigatórios.



**Ques. O que preenche a lista de usuários (contribuidores do Brand Portal) no menu suspenso de usuários da Contribuição de ativos?**

**Ans.** Os usuários na lista suspensa são preenchidos a partir do arquivo de configuração de usuário (.csv) do Brand Portal carregado no AEM.



**Ques. Onde posso ver o status das tarefas de importação e publicação?**

**Ans.** No AEM, você pode ver o status de uma importação na página de trabalho **assíncrona** . No Brand Portal, você pode ver o status de um trabalho de publicação em **[!UICONTROL Ferramentas &gt; Status]** de contribuição de ativos.



**Ques. Qual é a frequência de um trabalho de importação executado periodicamente no AEM?**

**Ans.** No AEM, a pesquisa é executada a cada 5 minutos.



**Ques. Há algum limite no número de vezes que uma pasta pode ser publicada no Portal de marcas para os ativos AEM?**

**Ans.** Não, todos os ativos na pasta **NEW** são publicados nos ativos AEM, independentemente de terem sido publicados anteriormente. Sempre que uma pasta **Contribuição** é publicada do Portal de marcas para os ativos AEM, ela substitui o conteúdo da pasta **NOVO** .



**Ques. Como carregar novos ativos em uma pasta de contribuição?**

**Ans.** Consulte a documentação detalhada para [Fazer upload de ativos para a pasta](brand-portal-upload-assets-to-contribution-folder.md)Contribuição.



**Ques. Não vejo miniaturas/visualizações nos ativos carregados na pasta NEW por um usuário do Brand Portal?**

**Ans.** Como projetado, porque não há fluxo de trabalho sendo executado no Portal da Marca.



**Ques. O que acontece se uma pasta for publicada do AEM Assets para o Brand Portal que está em fluxo?**

**Ans.** No AEM, os registros são mantidos sempre que uma pasta é publicada no Brand Portal. No momento da publicação, todos os ativos que não são publicados no Brand Portal são colocados em uma fila de replicação. Qualquer ativo adicionado à pasta depois que o trabalho de publicação é acionado não é publicado no Brand Portal. Quando o usuário do AEM publica a pasta novamente, somente os ativos que não foram publicados anteriormente (existentes na fila de replicação) são publicados no Brand Portal.
Isso vale para qualquer pasta publicada dos ativos AEM para o Portal de marcas e para a pasta COMPARTILHADA em uma pasta de contribuição.



**Ques. Com quem eu entro em contato com as perguntas?**

**Ans.** Entre em contato com seu Gerente de conta da Adobe ou com o Suporte ao cliente.


>[!NOTE]
>
>O cronograma de liberação é provisório e está sujeito a alterações. Entre em contato com seu Gerente de contas da Adobe ou com o Suporte ao cliente para obter o cronograma atualizado.




## Acesso e suporte ao produto (sites restritos) {#product-access-and-support-restricted-sites}

Estes sites estão disponíveis somente para clientes. Se você for um cliente e precisar de acesso, entre em contato com seu gerente de contas da Adobe.

* [](https://daycare.day.com) Acesso ao [produto](https://login.marketing.adobe.com)

* [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html)
