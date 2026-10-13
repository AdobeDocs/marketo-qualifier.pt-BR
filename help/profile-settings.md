---
title: Definir configurações de perfil
description: Saiba como configurar sua conexão de email, assinatura e disponibilidade de calendário nas configurações de perfil do Adobe Marketo Qualifier.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/YsrBduYA7jKhgxttexqMBBpgDIq23s6wUb4Wp6y6h3g'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Sales Qualifier
feature_v2:
  - id: 1e0ea71a-a210-5748-9b0f-c02c2ef6a746
    internal-label: Workflows
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
    internal-label: Integrations
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 3b50b4d3000696cb25ef747fefd579cfd3b3ba0f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%
---

# Configurações do perfil

Na navegação à esquerda, expanda **[!UICONTROL Configuração]** e selecione **[!UICONTROL Configurações de perfil]**. Use essas configurações para gerenciar seus detalhes pessoais, conexão de email, calendário e disponibilidade de chat.

![Configurações de perfil](assets/profile-email-config.png)

## Configurações de email

Na guia **[!UICONTROL Configurações de email]**, configure suas conexões de email.

* **[!UICONTROL Conexões de email]** — Selecione Microsoft Outlook ou Google e siga o processo de entrada. Consulte [Conectar-se ao Outlook](integrations.md#connect-outlook) para obter o acesso que você aprova e o caminho de aprovação do administrador, se necessário.
* **[!UICONTROL Assinatura de email]** — Adicione ou atualize a assinatura usada nos emails gerados. Inclua o link da sua [reserva de reunião](outbound-workflows.md#meeting-booking) para que os clientes potenciais possam agendar horários com você.
* **[!UICONTROL Link de reserva da reunião]** - Envie um convite de reunião dentro de seus emails. Obtém a URL da reunião.

### Contexto de redação do email

![Contexto do email](assets/profile-email-instructions.png)

Use o **[!UICONTROL Contexto de rascunho de email]** para definir o tom, a estrutura e o estilo do email, de forma que os emails sejam consistentes.

Escreva seu contexto em marcação simples na área **[!UICONTROL Contexto de rascunho de email]**.
Use-a para definir:

* Tom e voz
* Estrutura e comprimento
* Personalization e regras de saudação
* Estilo da linha de assunto
* Como os sinais de engajamento são usados
* Como métricas, pontos de prova e histórias de clientes são enquadradas

Por padrão, os rascunhos usam um contexto de estilo doméstico, de modo que os rascunhos existentes não são alterados até que você adicione seu próprio contexto.

## Configuração do calendário

Na guia **[!UICONTROL Configuração do calendário]**, defina o fuso horário e a disponibilidade.

* **[!UICONTROL Conexão do calendário]**—Selecione **[!UICONTROL Conectar]** e siga o processo de entrada da Microsoft.
* **[!UICONTROL Email de confirmação da reunião]** — Defina o assunto e o corpo do email de confirmação que um cliente potencial recebe após reservar uma reunião.
* **[!UICONTROL Preferências]** — Defina a duração padrão da reunião e o buffer entre reuniões.

Se você desconectar seu calendário:

* Os links de reserva ativos param de funcionar.
* A página de reserva mostra uma mensagem de indisponibilidade temporária.
* Suas configurações são preservadas quando você se reconecta.

## Disponibilidade do calendário

A disponibilidade de seu calendário no Adobe Marketo Qualifier é baseada em duas entradas:

* Seu calendário de trabalho conectado, como Outlook ou Gmail
* As regras de disponibilidade e intervalo de tempo na **[!UICONTROL Configuração do calendário]**

O Marketo Qualifier lê o status de disponibilidade, não os detalhes do evento, do calendário conectado. Ele combina esse status com suas regras para determinar os intervalos de tempo que os clientes potenciais podem reservar.

Você pode configurar:

* Horas de trabalho por dia da semana
* Vários blocos por dia, por exemplo, das 9h às 13h e das 13h às 17h.
* Seu fuso horário
* Duração da reunião
* Buffer antes e depois de reuniões
* Aviso mínimo
* Janela de reserva

>[!MORELIKETHIS]
>
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Integrações](integrations.md)
>* [Tarefas](tasks.md)
