---
title: Revisar a caixa de saída de email
description: Saiba como revisar os emails enviados pelo Adobe Marketo Qualifier em seu nome, incluindo respostas, na Caixa de saída de email.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: e6e1112f-735e-4244-9aeb-08972bded7e7
    internal-label: Email
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
source-git-commit: fcdc5d36cbb1500cf984e1439291aa8dbf17b72b
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%
---

# Caixa de saída de email

Use a **[!UICONTROL Caixa de Saída de Email]** para examinar emails enviados por Fluxos de Trabalho de Saída e quaisquer respostas. Você pode confirmar o que foi enviado, ler respostas no contexto e abrir o Fluxo de trabalho de saída que enviou uma mensagem.

A página tem dois painéis: uma lista de emails à esquerda e uma visualização de leitura à direita. Arraste o divisor entre elas para redimensionar a lista.

## Ler a lista de email

A lista **[!UICONTROL Todos os emails]** contém uma linha para cada email enviado, com o email mais recente primeiro. Cada linha mostra o nome, o assunto e a data de envio do recipient. Um email sem um assunto mostra _(Sem assunto)_. Role para carregar emails mais antigos.

Ao abrir a página, o Adobe Marketo Qualifier seleciona o primeiro email automaticamente para que seu conteúdo apareça à direita.

Se você não enviou nenhum email, a lista mostra _Sua caixa de saída está vazia_. Depois de enviar ou agendar um email por meio de um Fluxo de trabalho de saída, ele é exibido aqui.

## Ler um email e suas respostas

Para abrir um email à direita, selecione-o na lista. O modo de exibição de leitura tem três partes:

* **Destinatário** — O nome, o cargo e a conta do destinatário, quando disponíveis.
* **Fluxo de Trabalho de Assunto e Saída** — O assunto, o nome do [Fluxo de Trabalho de Saída](outbound-workflows.md) que enviou o email e o status do Fluxo de Trabalho de Saída. Para abrir o Fluxo de trabalho de saída, selecione o nome dele.
* **Conversação** — O email enviado e todas as respostas em um thread. Cada entrada identifica se a mensagem foi enviada ou recebida e inclui um carimbo de data e hora.

Os emails são renderizados conforme são enviados, incluindo o conteúdo personalizado. Se o corpo da mensagem não estiver disponível, o Marketo Qualifier mostrará uma breve observação _Conteúdo de email não disponível_ em seu lugar.

>[!NOTE]
>
>A caixa de saída de email é somente leitura. Para acompanhar um cliente potencial que respondeu, abra o Fluxo de Trabalho de Saída ou o cliente potencial. Para analisar o desempenho do email e da resposta, consulte [Desempenho de saída](performance.md).

>[!MORELIKETHIS]
>
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Desempenho de saída](performance.md)
>* [Tarefas](tasks.md)
