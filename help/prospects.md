---
title: Clientes potenciais em [!DNL Adobe Marketo Qualifier]
description: Saiba como criar sua lista de clientes potenciais a partir do CRM, de fontes importadas e adicionadas manualmente, filtrar clientes potenciais e revisar detalhes de clientes potenciais no [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/zf2H5rq1JlIT26LqLPMrm2Mq3tSIrLOiTEw6BXb1w2U'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
    internal-label: Integrations
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 2124387555f5fb08ea19eaf121fc87aa66d66de2
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 1%
---

# Clientes potenciais

Para exibir os clientes em potencial e os contatos que você pode acessar, selecione **[!UICONTROL Clientes potenciais]** na navegação à esquerda. Use a lista para examinar o status de cada cliente potencial e a atividade mais recente.

![Tabela de clientes potenciais exibindo o status do cliente potencial e a última atividade para gerenciamento de clientes potenciais](./assets/prospects.png){width="800" zoomable="yes"}

* **[!UICONTROL Clientes potenciais]** clientes potenciais atribuídos a você no CRM conectado.
* **[!UICONTROL Contatos]** Contatos atribuídos a você no CRM conectado.
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
* **Prospetos adicionados manualmente** — Prospetos individuais adicionados ao Qualificador do Marketo.

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

Os administradores também podem disponibilizar campos do CRM mapeados como filtros. Em **[!UICONTROL Configurações de Administração]**, ative **[!UICONTROL Filtrável]** para cada campo que os usuários usam para localizar prospetos. Consulte [Mapear campos do CRM](integrations.md#map-crm-fields-inbound-mapping).

Em **[!UICONTROL Meus Contatos da Oportunidade]**, você também pode filtrar contatos por campos de suas oportunidades associadas, como estágio, tipo e data de fechamento. Os campos de oportunidade têm rótulos como **[!UICONTROL Estágio (Oportunidade)]**, que os distingue dos campos de contato. O administrador controla quais campos de oportunidade estão disponíveis como filtros.

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
* **Lista de atividades** — Uma lista cronológica de atividades e comportamentos recentes.
* **Modo de exibição de Linha do Tempo** — uma linha do tempo visual do envolvimento entre canais.
* **Conteúdo exibido** — páginas da Web e ativos que o cliente potencial visualizou. Para abrir um item, selecione-o

### Gerar preparação da reunião

Além do resumo da pessoa de IA permanente, você pode gerar uma reunião preparada sob medida para uma chamada futura específica a partir da guia **[!UICONTROL Pesquisa de reunião]**, ao lado de **[!UICONTROL Pesquisa de conta]**.

* **Baseado em meta** — Se o cliente potencial estiver inscrito em um Fluxo de Trabalho de Saída em execução, selecione-o. O preparo se alinha à meta do Fluxo de trabalho de saída, como reservar uma reunião ou reengajar o cliente potencial.
* **Personalizar prompt**—Digite o que você deseja preparar, por exemplo `Focus on renewal risk` ou `Prepare for a technical deep dive with their IT lead`. O preparo corresponde ao seu prompt. A opção de prompt personalizado está disponível sempre que o cliente potencial não está em um Fluxo de trabalho de saída em execução.

>[!MORELIKETHIS]
>
>* [Contas](accounts.md)
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Bate-papo de IA](ai-assistant.md)
