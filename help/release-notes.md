---
title: Notas de versão do [!DNL Adobe Marketo Qualifier]
description: Saiba mais sobre as novidades do [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 633ca975d4fe58bdcc84caf633049ae1190b0f56
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 10%
---
# Notas de versão do [!DNL Adobe Marketo Qualifier]

## Próxima versão

* Descreva quem você deseja alcançar em linguagem simples e transforme-o em cliente potencial do CRM e filtros de contato, use cada filtro de Clientes potenciais e Contatos no direcionamento de Fluxo de trabalho de saída e visualize os clientes potenciais correspondentes antes de salvar. [Saiba mais](outbound-workflows.md#step-2-configure-targeting-filters).
* Filtre clientes potenciais por vários valores de uma só vez em campos de texto, como Título do trabalho e Email, com até cinco valores por filtro. [Saiba mais](prospects.md#filter-and-find-prospects).
* Revise, edite e envie respostas de rascunho de IA para respostas de prospecto diretamente de um fluxo de trabalho de saída ou rejeite rascunhos que não se encaixem. [Saiba mais](outbound-workflows.md#review-and-send-ai-draft-replies).
* Instale o [!DNL Adobe Marketo Qualifier] no Salesforce ou Microsoft Dynamics 365 e adicione prospetos a Fluxos de Trabalho de Saída ou campanhas do Marketo das exibições de lista e páginas de registro do Salesforce. [Saiba mais](crm-plugin-setup.md).
* Introdução mais rápida a Públicos inteligentes (Beta): uma apresentação guiada, opções de adição rápida ao criar um público-alvo e listas mais claras com contagens de registros, uma coluna Conta que permanece na exibição e pontuações codificadas por cores. [Saiba mais](smart-audience.md).
* Encontre e priorize as contas e os leads certos com público-alvo inteligente (Beta). Descreva as contas desejadas em linguagem simples, adicione dados de CRM e sinais de crescimento, analise clientes potenciais pontuados e adicione-os a um Fluxo de trabalho de saída. [Saiba mais](smart-audience.md).
* Filtre contatos por campos de conta, junto com campos de contato e oportunidade, para encontrar os contatos certos e direcionar workflows de saída com mais precisão. [Saiba mais](prospects.md#filter-and-find-prospects).
* Os contatos mostram sua conta associada e o nome do proprietário, e a página de um cliente potencial agora mostra 90 dias de atividade de marketing, antes 30. [Saiba mais](prospects.md#review-prospect-details).

## 10-08-2026

Esta versão inclui:

* Reutilize um workflow de saída ou altere os pontos de contato de um workflow em execução, duplique-o e edite a cópia. A cópia é iniciada como um rascunho privado sem clientes potenciais e o fluxo de trabalho original permanece inalterado. [Saiba mais](outbound-workflows.md#duplicate-an-outbound-workflow).
* Configure Workflows de saída em um layout compacto com navegação entre meta, direcionamento, pontos de contato e configurações. [Saiba mais](outbound-workflows.md#create-an-outbound-workflow).
* Limpar as solicitações de recusa em respostas de email são reconhecidas automaticamente. O cliente potencial é marcado como recusado e nenhum outro ponto de contato é enviado. [Saiba mais](outbound-workflows.md#opt-out-requests-in-replies).
* Prepare-se para reuniões com um único resumo que combina pesquisa na Web e estudos de caso de clientes específicos de produtos, com tópicos classificados por relevância e fontes identificadas. [Saiba mais](prospects.md#generate-meeting-prep).
* Os emails gerados são verificados em relação às diretrizes de qualidade e regravados quando necessário, antes de você analisá-los. Você ainda revisa, edita e aprova cada email antes que ele seja enviado. [Saiba mais](outbound-workflows.md#review-and-refine-generated-emails).

## 09-22-2026

Esta versão inclui:

* Exiba [!DNL Marketo Sales Insights] e dados de agente no plug-in do CRM inserido e adicione prospetos a [!DNL Marketo Qualifier]. [Saiba mais](admin-settings.md#crm-mcp-and-the-embedded-plugin).
* Priorize clientes potenciais do CRM com melhores opções, Minha lista de observação, atividade da Web, envolvimento de email e atividade de webinário. [Saiba mais](admin-settings.md#prioritize-leads-in-the-crm-plugin).
* Inscrever automaticamente clientes potenciais em Fluxos de Trabalho de Saída quando a atividade [!DNL Marketo] ativa corresponder aos critérios do fluxo de trabalho. [Saiba mais](home.md#automatically-enroll-prospects-from-marketing-highlights).
* Revise o contexto do cliente potencial, exporte a lista de clientes potenciais e exiba os resumos de pessoa da IA em [!DNL Marketo Optimizer] instâncias do Prime e do Ultimate. [Saiba mais](prospects.md#review-prospect-context-and-export-the-list).
* Revise e aprove emails de clientes potenciais gerados da fila de tarefas e responda com sugestões de agente durante um Fluxo de trabalho de saída. [Saiba mais](tasks.md).

## 09-08-2026

Esta versão inclui:

* Defina seu próprio estilo de rascunho de email uma vez nas configurações de Perfil, e cada email gerado o seguirá. [Saiba mais](profile-settings.md#email-drafting-context).
* Gerar preparação de reunião personalizada ou com base em metas a partir da página de um cliente potencial, em uma nova guia Pesquisa de reunião. [Saiba mais](prospects.md#generate-meeting-prep).
* Os administradores podem atribuir um Fluxo de trabalho de saída a um colega de equipe e redefinir as configurações do fluxo de trabalho para seus padrões. [Saiba mais](outbound-workflows.md#create-an-outbound-workflow).
* Mapeie campos personalizados ao importar prospetos de um CSV e use esses valores em emails gerados. [Saiba mais](prospects.md#build-your-prospect-list).
* Os emails gerados usam quaisquer dados de cliente potencial adicionais que você importar e podem ser escritos nativamente no idioma do cliente potencial. [Saiba mais](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
* Desempenho de Saída mostra a taxa de abertura e a taxa de cliques por padrão, com uma alternância para contagens brutas e total de clientes potenciais no nível da organização. [Saiba mais](performance.md).
* As Regras de Sincronização do CRM atualizam automaticamente o status do CRM à medida que um cliente potencial passa por um Fluxo de Trabalho de Saída. [Saiba mais](admin-settings.md#configure-crm-sync-rules).
* Faça perguntas sobre o Chat de IA nos dados do [!DNL Marketo Qualifier], CRM, [!DNL Marketo] e [!DNL Marketo Optimizer]. [Saiba mais](ai-assistant.md#ask-ai-chat-across-your-connected-data).

## 08-17-2026

[!DNL Marketo Qualifier] agora está disponível como um aplicativo independente. Oferece suporte a [!DNL Marketo Engage] e [!DNL Marketo Optimizer].

Esta versão inclui:

* Priorização de prospecto e conta com resumos de atividades geradas por IA e pontuação baseada em sinais. [Saiba mais](prospects.md#review-prospect-details) sobre clientes potenciais ou [contas](accounts.md#account-insights).
* Fluxos de trabalho de saída orientados por metas com cadências propostas por IA e emails rascunhados. [Saiba mais](outbound-workflows.md).
* Uma fila de tarefas unificada para chamadas telefônicas, LinkedIn InMails e revisões de email. [Saiba mais](tasks.md).
* Agendamento automático de reunião por meio da integração do calendário. [Saiba mais](outbound-workflows.md#meeting-booking).
* Um centro de conhecimento para fundamentar o alcance da IA em seus próprios materiais do manual. [Saiba mais](admin-settings.md#knowledge-center).
* Chat de IA para perguntas em linguagem natural com base em seu CRM, envolvimento e dados do Centro de conhecimento. [Saiba mais](ai-assistant.md).
* Relatórios de desempenho de email e reserva de reunião. [Saiba mais](performance.md).
* Plug-ins de navegador e email para acesso no CRM ou Outlook. [Saiba mais](admin-settings.md#crm-mcp-and-the-embedded-plugin).
* Suporte para integrações Salesforce e Microsoft Dynamics 365. [Saiba mais](integrations.md).
