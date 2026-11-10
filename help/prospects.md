---
title: Clientes potenciais em [!DNL Adobe Marketo Qualifier]
description: Saiba como criar sua lista de clientes potenciais a partir do CRM, de fontes importadas e adicionadas manualmente, filtrar clientes potenciais e revisar detalhes de clientes potenciais no [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/zf2H5rq1JlIT26LqLPMrm2Mq3tSIrLOiTEw6BXb1w2U'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: da87d43a-78d4-4b1e-bb4a-743cbd343472
    internal-label: Prospects
subfeature_v2:
  - id: 6aa13f53-6e49-5228-b98a-64c9ebe5af74
    internal-label: Contacts
  - id: 4143255e-1853-5eb6-a189-dece7126669f
    internal-label: Leads
  - id: 78e1f6f5-7122-5e4d-81c3-d3a90e954414
    internal-label: People lists
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
    internal-label: Customer profiles
source-git-commit: 633ca975d4fe58bdcc84caf633049ae1190b0f56
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 1%
---

# Clientes potenciais

Para exibir os clientes em potencial e os contatos que você pode acessar, selecione **[!UICONTROL Clientes potenciais]** na navegação à esquerda. Use a lista para examinar o status de cada cliente potencial e a atividade mais recente.

![Tabela de clientes potenciais exibindo o status do cliente potencial e a última atividade para gerenciamento de clientes potenciais](./assets/prospects.png){width="800" zoomable="yes"}

* **[!UICONTROL Clientes potenciais]** clientes potenciais atribuídos a você no CRM conectado.
* **[!UICONTROL Contatos]** Contatos atribuídos a você no CRM conectado, com sua conta associada. Os detalhes de contato também incluem o nome do proprietário. Esses detalhes estão disponíveis para o Salesforce e o Microsoft Dynamics 365.
* **[!UICONTROL Destaques de marketing]** clientes potenciais com atividade de Marketo ao vivo, como aberturas ou cliques de email.
* **[!UICONTROL Lista de pessoas]** Clientes potenciais que você importa ou adiciona manualmente.

## Revisar contexto de cliente potencial e exportar a lista

A lista de clientes potenciais resume se o contexto adicional está disponível para alcance personalizado. Um resumo acima da lista mostra o número de clientes potenciais em cada estado, e a coluna de contexto exibe o estado de cada cliente potencial:

* **[!UICONTROL Aplicado]** O contexto disponível foi aplicado ao cliente potencial.
* **[!UICONTROL Parcial]** Apenas parte do contexto disponível foi aplicada.
* **[!UICONTROL Ausente]** Nenhum contexto adicional está disponível.

Para baixar a lista de clientes potenciais atual como um arquivo CSV, selecione **[!UICONTROL Exportar CSV]**.

## Criar sua lista de clientes potenciais

A lista de clientes potenciais combina pessoas de mais de uma fonte:

* **Clientes potenciais do CRM**—[!DNL Adobe Marketo Qualifier] importa automaticamente clientes potenciais e contatos atribuídos ao usuário conectado. Consulte [Integrações](integrations.md).
* **Prospetos importados** — Prospetos importados de um arquivo CSV.
* **Prospetos adicionados manualmente** — Prospetos individuais adicionados ao Marketo Qualifier.

Para adicionar prospetos que não vêm do seu CRM:

1. Na página **[!UICONTROL Clientes potenciais]**, selecione **[!UICONTROL Lista de pessoas]**.

   ![Lista de pessoas](assets/prospects-people-list.png){width="800" zoomable="yes"}

1. Selecione **[!UICONTROL + Adicionar pessoas]** e **[!UICONTROL Importar CSV]** ou **[!UICONTROL Adicionar pessoa]**.

   * Para uma importação de CSV, carregue um CSV no formato `firstname,email`.
     O nome e o email são obrigatórios. O sobrenome é opcional. O modelo CSV não inclui a coluna de ID de cliente potencial do CRM, mas você pode adicionar a coluna e seus valores ao arquivo antes da importação. Se a importação falhar, revise a mensagem de erro para os campos ou valores a serem corrigidos e, em seguida, faça upload do arquivo novamente.
     Mapeie campos CSV personalizados ou adicionais, não apenas os campos padrão. A Marketo Qualifier salva esses valores em cada cliente potencial e os disponibiliza posteriormente, inclusive para [geração de email](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
   * Para adicionar uma pessoa manualmente, insira seus detalhes no formulário.

1. Selecione **[!UICONTROL Salvar]**.

## Filtrar e localizar clientes potenciais

Para restringir a lista, selecione **[!UICONTROL Filtro]**. Você pode filtrar por:

* Status do fluxo de trabalho de saída
* Criado por
* Nome do cargo
* Conta
* Fonte
* Última atualização

Nas listas **[!UICONTROL Clientes Potenciais]** e **[!UICONTROL Contatos]**, filtros de texto como **[!UICONTROL Cargo]** e **[!UICONTROL Email]** aceitam até cinco valores com o operador contains. Digite um valor e pressione Enter, depois adicione o próximo valor. Os resultados incluem clientes potenciais que correspondem a qualquer um dos valores. Por exemplo, um filtro de título de trabalho que contém `manager` e `director` retorna clientes potenciais cujo título contém qualquer uma das palavras. Esta filtragem está disponível para Salesforce e Microsoft Dynamics 365, e os mesmos filtros podem ser usados em [Direcionamento do Fluxo de Trabalho de Saída](outbound-workflows.md#step-2-configure-targeting-filters).

Os administradores também podem disponibilizar campos do CRM mapeados como filtros. Em **[!UICONTROL Configurações de Administração]**, ative **[!UICONTROL Filtrável]** para cada campo que os usuários usam para localizar prospetos. Consulte [Mapear campos do CRM](integrations.md#map-crm-fields-inbound-mapping).

Em **[!UICONTROL Meus Contatos da Oportunidade]**, você também pode filtrar contatos por campos de suas oportunidades associadas, como estágio, tipo e data de fechamento. Os campos de oportunidade têm rótulos como **[!UICONTROL Estágio (Oportunidade)]**, que os distingue dos campos de contato. O administrador controla quais campos de oportunidade estão disponíveis como filtros.

Também é possível filtrar contatos por campos da conta associada, como setor, região ou tipo de conta. O administrador escolhe quais campos de conta podem ser filtrados. Combine filtros de conta, contato e oportunidade para localizar, por exemplo, contatos com uma função específica em contas de um setor específico. A filtragem de campo de conta está disponível para Salesforce e Microsoft Dynamics 365, e os mesmos campos podem ser usados em [Direcionamento de Fluxo de Trabalho de Saída](outbound-workflows.md#step-2-configure-targeting-filters).

### Filtrar por destaques de marketing

Revise e priorize clientes potenciais pelo envolvimento ativo de [!DNL Marketo], como atividade de email, visitas da Web e preenchimentos de formulário. O engajamento aparece em tempo quase real, à medida que acontece.

Para filtrar clientes potenciais por Realces de marketing:

1. Selecione **[!UICONTROL Filtro]**.
1. Adicione um filtro de Destaques de marketing e defina o tipo de atividade, a campanha ou outros atributos para se concentrar no envolvimento importante.

Cada cliente potencial mostra sua atividade [!DNL Marketo] mais recente junto com o histórico recente.

Os destaques de marketing estão disponíveis em todas as regiões de produção. Um administrador conclui uma instalação única que conecta o [!DNL Marketo] ao Marketo Qualifier. Consulte [Configurar destaques de marketing](integrations.md#turn-on-marketo-engagement-filtering).

## Revisar detalhes do cliente potencial

Para abrir o perfil de um cliente potencial, selecione-o. Revise os sinais importantes antes de entrar em contato com:

* **Resumo da pessoa de IA** — um instantâneo escrito por IA do cliente potencial ou contato e seu envolvimento recente. Use o resumo para entender a pessoa rapidamente antes de revisar atividades individuais. Os resumos da pessoa de IA estão disponíveis em instâncias que executam o [!DNL Marketo Optimizer] Prime ou o Ultimate.
* **Lista de atividades** — Uma lista cronológica que mostra os últimos 90 dias de atividade de marketing.
* **Modo de exibição de Linha do Tempo** — uma linha do tempo visual que mostra os últimos 90 dias de envolvimento de marketing entre canais.
* **Conteúdo exibido** — páginas da Web e ativos que o cliente potencial visualizou. Para abrir um item, selecione-o

### Gerar preparação da reunião

Além do resumo da pessoa de IA permanente, você pode gerar uma reunião preparada sob medida para uma chamada futura específica a partir da guia **[!UICONTROL Pesquisa de reunião]**, ao lado de **[!UICONTROL Pesquisa de conta]**.

O Meeting Prep combina pesquisas na Web sobre o cliente potencial e sua empresa com evidências de estudos de caso sobre clientes de mesmo nível que usam o produto que você está vendendo. Os pontos de discussão do estudo de caso podem incluir resultados mensuráveis do cliente. As fontes são combinadas em um resumo, com os pontos de discussão classificados por relevância. Cada ponto de discussão identifica se vem de estudos de caso, pesquisa na web ou ambos. Se nenhuma evidência de estudo de caso relevante estiver disponível, o preparo da reunião usa pesquisa na Web.

* **Baseado em meta** — Se o cliente potencial estiver inscrito em um Fluxo de Trabalho de Saída em execução, selecione-o. O preparo se alinha à meta do Fluxo de trabalho de saída, como reservar uma reunião ou reengajar o cliente potencial.
* **Personalizar prompt**—Digite o que você deseja preparar, por exemplo `Focus on renewal risk` ou `Prepare for a technical deep dive with their IT lead`. O preparo corresponde ao seu prompt. A opção de prompt personalizado está disponível sempre que o cliente potencial não está em um Fluxo de trabalho de saída em execução.

O resumo continua seguindo a meta do Fluxo de trabalho de saída ou o prompt personalizado que você escolher. A forma como você gera o preparo da reunião não é alterada.

>[!MORELIKETHIS]
>
>* [Contas](accounts.md)
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Bate-papo de IA](ai-assistant.md)
