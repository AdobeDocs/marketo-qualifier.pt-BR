---
title: Tarefas em [!DNL Adobe Marketo Qualifier]
description: Saiba como processar tarefas de alcance manual e revisar clientes em potencial sugeridos por agente na fila de tarefas do [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/MbTN1r-ARrW-XYtdIS-KZT7K1Lk-B3GihT8iXL60GrQ'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Sales Qualifier
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 3b50b4d3000696cb25ef747fefd579cfd3b3ba0f
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%
---

# Tarefas

Use **[!UICONTROL Tarefas]** para concluir as ações geradas por Fluxos de Trabalho de Saída. Selecione uma tarefa, execute uma ação, marque a tarefa como concluída e continue para a próxima tarefa sem sair da página.

Na navegação à esquerda, vá para **[!UICONTROL Atividades]** > **[!UICONTROL Tarefas]**.

![Painel de tarefas](assets/tasks.png)

## Exibições de tarefa

A página tem duas guias:

* **[!UICONTROL Tarefas manuais]**—Telefonemas, LinkedIn InMails e revisões de email para clientes potenciais inscritos em um Fluxo de Trabalho de Saída.
* **[!UICONTROL Sugestões de agente]** — Clientes potenciais que correspondem a um critério de direcionamento do Fluxo de Trabalho de Saída e são recomendados para inscrição.

Cada guia tem seus próprios filtros, opções de classificação e layout de dois painéis. A lista de tarefas aparece à esquerda e o painel de trabalho aparece à direita. Selecionar uma tarefa carrega seus detalhes no painel de trabalho. Quando você conclui uma tarefa, a próxima tarefa é selecionada automaticamente.

## Tarefas manuais

### Tipos de tarefa

As tarefas manuais estão vinculadas às etapas do Fluxo de trabalho de saída e têm três tipos:

* **[!UICONTROL Telefonema]** — Criado quando uma cadência atinge uma etapa de telefonema. O painel de trabalho mostra o número de telefone do cliente potencial e, quando disponível, um script de chamada gerado por IA.

* **[!UICONTROL LinkedIn InMail]** — Criado quando uma cadência atinge uma etapa do LinkedIn InMail. O painel de trabalho mostra o conteúdo a ser copiado e enviado do LinkedIn. Expanda **[!UICONTROL Razão da IA]** para analisar a razão.

* **[!UICONTROL Revisão de Email]**—Criada depois de [!DNL Adobe Marketo Qualifier] gerar emails personalizados de um cliente potencial. Para revisar e aprovar os rascunhos antes do início do alcance, selecione **[!UICONTROL Revisar emails]**. Consulte [Revisar e refinar emails gerados](outbound-workflows.md#review-and-refine-generated-emails).

![Revisão de email](assets/tasks-review.png)

### O painel de trabalho

Para uma tarefa **[!UICONTROL Telefonema]** ou **[!UICONTROL LinkedIn InMail]**, o painel de trabalho contém:

* **[!UICONTROL Prospecto]** — O nome, o link de email e o número de telefone do cliente potencial, quando aplicável.
* **[!UICONTROL Fluxo de Trabalho de Saída]** — O nome do Fluxo de Trabalho de Saída vinculado, a data de vencimento e o indicador de salto automático, quando aplicável.
* **Conteúdo da tarefa** — O script de chamada ou o conteúdo do InMail.
* **[!UICONTROL Notas]** — As notas são salvas automaticamente quando outra tarefa é selecionada. Não é possível editar notas depois que uma tarefa é concluída, ignorada ou cancelada.

### Gerar um script de chamada

Para uma tarefa **[!UICONTROL Telefonema]**, selecione **[!UICONTROL Gerar script de chamada]**. Quando a geração terminar, selecione **[!UICONTROL Exibir Script de Chamada Detalhada]**. Se a geração falhar, tente novamente no painel.

### Ações da tarefa

Duas ações estão disponíveis no cabeçalho do painel de trabalho:

* **[!UICONTROL Marcar como concluído]**—Use esta ação depois de fazer a chamada, enviar o InMail ou revisar os emails. A fila avança para a próxima tarefa.
* **[!UICONTROL Ignorar]** — Use esta ação quando não puder concluir a etapa, mas quiser manter o cliente potencial no Fluxo de Trabalho de Saída. O cliente potencial avança para a próxima etapa de cadência.

As tarefas de Telefonema e InMail do LinkedIn podem ser ignoradas automaticamente se permanecerem abertas além do limite configurado. Um salto automático avança o cliente potencial pela cadência e não afeta os pontos de contato de email agendados.

### Filtrar, pesquisar e classificar

A barra de ferramentas acima da lista controla quais tarefas são exibidas e em que ordem. Suas opções de filtro e classificação são salvas e reaplicadas na próxima vez que você abrir a página.

* **[!UICONTROL Filtro]**—Abra o painel de filtro:
  * **[!UICONTROL Status]**—**[!UICONTROL Atual]**, **[!UICONTROL Futuro]**, **[!UICONTROL Vencido]**, **[!UICONTROL Concluído]**, **[!UICONTROL Cancelado]**, **[!UICONTROL Ignorado]**.
  * **[!UICONTROL Tipo de tarefa]**—**[!UICONTROL Email Review]**, **[!UICONTROL LinkedIn InMail]**, **[!UICONTROL Telefonema]**.
  * **[!UICONTROL Data de vencimento]**.
  * **[!UICONTROL Fluxo de Trabalho de Saída]** — Uma lista pesquisável de seus Fluxos de Trabalho de Saída.
* **[!UICONTROL Classificar]** — Classificar por data de vencimento ou data de criação. A ordem de classificação também determina a ordem em que a fila avança.
* **[!UICONTROL Pesquisar tarefas]** — Localize tarefas por nome de cliente potencial, nome de empresa ou Fluxo de Trabalho de Saída. A pesquisa se aplica com filtros ativos.

Filtros ativos aparecem como chips abaixo da barra de ferramentas. Para redefini-los, selecione **[!UICONTROL Limpar tudo]**.

### Status da tarefa

Cada tarefa mostra seu status atual:

| Status | Descrição |
| --- | --- |
| **[!UICONTROL Atual]** | Com prazo e pronto para agir. As tarefas atuais não mostram nenhuma medalha. |
| **[!UICONTROL Próximos]** | A etapa anterior está concluída, mas a data de vencimento está no futuro. Você pode agir cedo se o momento estiver certo. |
| **[!UICONTROL Vencido]** | Ultrapassou a data de vencimento e ainda não foi concluído. A tarefa está sinalizada para atenção. |
| **[!UICONTROL Concluído]** | Você concluiu a ação e marcou a tarefa como concluída. |
| **[!UICONTROL Ignorado]** | Você ignorou a etapa ou ela ignorou automaticamente. O cliente potencial avança no Fluxo de trabalho de saída. |
| **[!UICONTROL Cancelado]** | O sistema cancelou a tarefa devido a uma alteração no Fluxo de trabalho de saída. |

As tarefas concluídas, ignoradas e canceladas são finais. Suas ações não estão mais disponíveis e suas notas são somente leitura.

## Sugestões do agente

A guia **[!UICONTROL Sugestões do agente]** lista os clientes potenciais que correspondem aos critérios de direcionamento de um Fluxo de Trabalho de Saída e são recomendados para inscrição. Para ativar as recomendações, consulte [Fluxos de Trabalho de Saída](outbound-workflows.md).

Para revisar uma sugestão no painel de trabalho, selecione-a:

* Um selo de recenticidade marca cada sugestão como **[!UICONTROL Nova]** ou **[!UICONTROL Anterior]**.
* A tabela **[!UICONTROL Clientes potenciais recomendados]** ou **[!UICONTROL Contatos recomendados]** lista os clientes potenciais propostos com colunas para **[!UICONTROL Nome]**, **[!UICONTROL Título]**, **[!UICONTROL Conta]**, **[!UICONTROL Status]**, **[!UICONTROL Email]** e **[!UICONTROL Última atualização]**.

Duas ações estão disponíveis:

* **[!UICONTROL Revisar prospetos]**—Abra o Fluxo de Trabalho de Saída para revisar e inscrever prospetos recomendados. Consulte [Adicionar clientes potenciais e iniciar geração de email](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
* **[!UICONTROL Marcar como concluída]**—Descarte a sugestão depois de revisá-la.

A guia **[!UICONTROL Sugestões do agente]** inclui os filtros de status **[!UICONTROL Atual]**, **[!UICONTROL Concluído]** e **[!UICONTROL Cancelado]**, um filtro de Fluxo de Trabalho de Saída e a classificação por data de criação.

### Responder a um cliente potencial com uma sugestão de agente

Quando um cliente potencial responde a um email, [!DNL Marketo Qualifier] pode rascunhar uma resposta na thread e adicioná-la como uma tarefa em **[!UICONTROL Sugestões do agente]**. O rascunho usa o contexto relevante de:

* O thread de email completo, não apenas a mensagem mais recente.
* Material adicional e pesquisa de produto do Centro de conhecimento.
* Sinais da conta, como notícias recentes, envolvimento de marketing e atividade de CRM.
* Seu [contexto de rascunho de email](profile-settings.md#email-drafting-context) foi salvo.

O assistente adapta a resposta à intenção do cliente potencial. Por exemplo, ele pode oferecer horários por meio do link de reserva para uma solicitação de reunião, reforçar o valor quando o cliente potencial estiver interessado, responder a uma pergunta sobre o produto em seu material de apoio, compartilhar um ativo relevante, solucionar uma objeção com um diferencial ou usar uma resposta de baixa pressão quando o cliente potencial quiser adiar.

Mensagens sobre preços, requisitos legais ou de segurança, respostas hostis e solicitações pouco claras permanecem com o representante para uma resposta pessoal.

1. Abra a sugestão de resposta e revise o thread completo e a resposta de rascunho.
1. Para criar outro rascunho, edite a resposta ou selecione **[!UICONTROL Gerar com IA]**.
1. Para enviar a resposta e continuar o Fluxo de Trabalho de Saída do cliente potencial, selecione **[!UICONTROL Aprovar e enviar]**.

## Concluir tarefas de um fluxo de trabalho de saída

Na exibição **[!UICONTROL Clientes Potenciais Envolvidos]** de um Fluxo de Trabalho de Saída, um ponto de contato manual fornece as mesmas opções de **[!UICONTROL Marcar como concluído]**, **[!UICONTROL Ignorar]** e anotações. Concluir uma tarefa lá também atualiza seu status na página **[!UICONTROL Tarefas]**. Consulte [Fluxos de Trabalho de Saída](outbound-workflows.md).

## Estados vazios

* Quando você não tem nenhuma tarefa para desempenhar, a lista mostra uma mensagem de _Você está no auge hoje_.
* Quando os filtros não correspondem a nenhuma tarefa, a lista relata que nenhuma tarefa corresponde aos seus filtros.
* Quando nenhuma tarefa é selecionada, o painel de trabalho solicita que você selecione uma tarefa. Para exibir seus detalhes, selecione uma tarefa.

>[!MORELIKETHIS]
>
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Desempenho de saída](performance.md)
>* [Clientes Potenciais](prospects.md)
