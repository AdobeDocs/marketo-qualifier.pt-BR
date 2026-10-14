---
title: Configurações de administração
description: Saiba como gerenciar campos do CRM, sincronização de atividades, recusa de email e outras configurações de administração do [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
internal-label: Administration
autotag-review: '2026-10-08T17:58:28.029Z'
TQID: 'https://experienceleague.adobe.com/2eccZWj1XY7qP20n6GcnBe6PZwNkp0ALhZfOhljwZF8'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Sales Qualifier
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
    internal-label: Customer profiles
source-git-commit: 3b50b4d3000696cb25ef747fefd579cfd3b3ba0f
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%
---

# Configurações de administração

Use as **[!UICONTROL Configurações de Administração]** para configurar as integrações de CRM, gerenciar o Centro de Conhecimento e configurar a recusa de email.

[!DNL Adobe Marketo Qualifier] conecta-se ao Salesforce ou Microsoft Dynamics 365. A conexão fornece à Account Qualification Agent (AQA) uma visualização consistente de clientes potenciais, contas, contatos, atividades e proprietários. O Marketo Qualifier também pode gravar atividades de alcance geral e status de recusa no CRM e sincronizar atividades de alcance geral com o Marketo.

Para configurar conexões do CRM, mapeamento de campos e sincronização de atividades, vá para **[!UICONTROL Administração]** > **[!UICONTROL Configurações de Administração]** > **[!UICONTROL Conexões do CRM]**. Os usuários padrão podem usar os dados e filtros do CRM configurados, mas não podem alterar essas configurações. Para conectar um CRM pela primeira vez, consulte [Introdução](getting-started.md#connect-your-crm).

>[!IMPORTANT]
>
>O acesso a **[!UICONTROL Configurações de Administrador]** requer associação aos grupos de usuários `Marketo Qualifier` e `Marketo Qualifier Admins`.

## MCP do CRM e o plug-in incorporado

O Marketo Qualifier funciona com seu CRM das seguintes maneiras:

* **Consultas do MCP do CRM** — O Account Qualification Agent consulta dados do CRM ao vivo para que as respostas e os insights reflitam o estado atual de seus registros.
* **Plug-in incorporado** — o plug-in do CRM exibe [!DNL Marketo Sales Insights] insights e dados de agente no seu CRM. Use o plug-in para adicionar um cliente potencial a [!DNL Marketo Qualifier].
* **Sincronização de atividade** — Quando um administrador ativa a **[!UICONTROL Sincronização de atividade]**, as atividades de alcance externo são sincronizadas com o CRM e o Marketo.

### Priorizar clientes em potencial no plug-in do CRM

O plug-in CRM fornece uma página inicial padrão, em que os representantes podem priorizar clientes em potencial sem sair do CRM. As guias disponíveis organizam o trabalho por origem e por intenção:

* **[!UICONTROL Melhores Opções]** — Recomendações de clientes potenciais prontas para ação.
* **[!UICONTROL Minha Lista de Interesse]** — Clientes potenciais que você está rastreando.
* **[!UICONTROL Atividade da Web]** — Visitas recentes ao site de clientes potenciais conhecidos.
* **[!UICONTROL Atividade da Web Anônima]** — Visitas de visitantes não identificados.
* **[!UICONTROL Meu Email]** — Engajamento no email associado aos seus clientes potenciais.
* **[!UICONTROL Webinar]** — atividade de registro e participação no webinário.

Cada lead pode incluir uma pré-visualização de email [!DNL Marketo], um link para os detalhes do lead e uma pesquisa no LinkedIn. As guias e os dados que você pode acessar dependem da configuração do plug-in do CRM.

## Escopo de acesso do CRM

O Marketo Qualifier lê usuários, contatos, mapeamentos de proprietários, clientes potenciais, contas, oportunidades e atividades do CRM. Ele grava no CRM somente atividades de alcance reportadas e status de recusa, e sincroniza atividades de alcance reportadas ao Marketo. Seu administrador de CRM prepara o acesso à API no Salesforce ou Dynamics. Em seguida, um administrador do Marketo Qualifier conecta o CRM, mapeia campos de entrada e escolhe se deseja sincronizar atividades.

>[!NOTE]
>
>As etapas de credencial em [Introdução](getting-started.md#connect-your-crm) descrevem o acesso de leitura a objetos do CRM. Se você ativar a sincronização de atividades ou o cancelamento da gravação, peça ao administrador do CRM para conceder o acesso de gravação correspondente exigido pela configuração do CRM.

## Mapear campos do CRM (mapeamento de entrada)

Depois que o CRM estiver conectado, selecione **[!UICONTROL Gerenciar]** para a conexão e abra o **[!UICONTROL Mapeamento de entrada]**. O mapeamento de entrada controla quais campos do CRM o Marketo Qualifier extrai para o aplicativo.

1. Selecione **[!UICONTROL Adicionar seção]**.
1. Insira um nome e uma descrição de seção.
1. Selecione um tipo de entidade. **[!UICONTROL Clientes potenciais]** está selecionado por padrão. **[!UICONTROL Contatos]**, **[!UICONTROL Contas]** e **[!UICONTROL Oportunidades]** também estão disponíveis.
1. Para importar campos do CRM, selecione os campos.

   Cada linha de campo exibe seu **[!UICONTROL Nome de exibição]**, **[!UICONTROL Nome do campo]** e **[!UICONTROL Tipo de dados]**.

1. Ative **[!UICONTROL Filtrável]** para cada campo de cliente potencial, contato ou oportunidade que você deseja disponibilizar como filtro na lista **[!UICONTROL Clientes Potenciais]**.
1. Visualize a seção e selecione **[!UICONTROL Adicionar]**.

Os campos mapeados aparecem nas áreas correspondentes do Marketo Qualifier:

* Os campos de cliente potencial aparecem na guia **[!UICONTROL Pessoa]**.
* Os campos de conta aparecem na guia **[!UICONTROL Conta]**.
* Os campos de oportunidade aparecem na seção **[!UICONTROL Oportunidade de conta]**. Os campos de oportunidade filtráveis também aparecem como suas próprias colunas em **[!UICONTROL Meus Contatos de Oportunidade]**, com rótulos como **[!UICONTROL Preparo (Oportunidade)]** para diferenciá-los dos campos de contato.

## Configurar a sincronização de atividades (mapeamento de saída)

1. Em **[!UICONTROL Conexões do CRM]**, selecione **[!UICONTROL Gerenciar]** para o CRM conectado.
1. Abra **[!UICONTROL Mapeamento de saída]**.
1. Ative a **[!UICONTROL Sincronização de atividade]** para sincronizar as atividades de alcance da Marketo Qualifier com o CRM e a Marketo.

Quando a sincronização de atividades está desativada, o Marketo Qualifier continua a usar dados de entrada do CRM, mas não sincroniza atividades de alcance para seu CRM ou Marketo.

## Configurar Regras de Sincronização do CRM

O Marketo Qualifier pode enviar atualizações de status de clientes potenciais de volta para o Salesforce e o Microsoft Dynamics automaticamente à medida que um cliente potencial passa por um fluxo de trabalho de saída, para que os representantes não atualizem mais o CRM manualmente.

### O que as Regras de Sincronização do CRM fazem

Uma atualização pode direcionar o registro de **[!UICONTROL Lead]**, **[!UICONTROL Contato]**, **[!UICONTROL Conta]** ou **[!UICONTROL Oportunidade]**, não apenas o lead.

As atualizações são acionadas nestes momentos do Fluxo de trabalho de saída:

* Adicionado a um fluxo de trabalho, respondido ou reunião registrada
* Removido por um representante ou fluxo de trabalho concluído sem resposta
* Recusa ou email rejeitado

Os valores de campo podem ser personalizados com tokens dinâmicos para que a atualização do CRM reflita a jornada real do cliente potencial em vez de um valor estático. Os tokens estão disponíveis para detalhes como o nome do representante, o nome do Fluxo de trabalho de saída e a data e hora da reunião.

Somente valores compatíveis com o CRM são gravados, um campo com falha não bloqueia os outros e problemas temporários são repetidos automaticamente. Cada atualização é rastreada para que você possa ver o que está sincronizado e o que precisa de atenção.

### Configurar Regras de Sincronização do CRM

Para configurar Regras de Sincronização do CRM:

1. Na navegação à esquerda, expanda **[!UICONTROL Administração]** e selecione **[!UICONTROL Configurações de Administração]** > **[!UICONTROL Conexões do CRM]**.
1. Selecione **[!UICONTROL Gerenciar]** para o CRM conectado e selecione **[!UICONTROL Regras de sincronização]**.
1. Escolha a entidade CRM de destino e os campos, mapeie-os para os momentos do fluxo de trabalho acima e ative o botão de alternância.

Com as Regras de sincronização do CRM configuradas, as equipes de vendas veem o status preciso, personalizado e atualizado em clientes potenciais, contatos, contas e oportunidades em cada estágio, com menos atraso de dados e trabalho manual.

## Criar um manual da Central de conhecimento {#knowledge-center}

O **[!UICONTROL Centro de Conhecimento]** dá à Account Qualification Agent (AQA) acesso aos seus materiais de vendas. A Marketo Qualifier usa esses materiais para gerar pesquisas, insights de qualificação e alcance que refletem como sua organização vende. Somente administradores podem criar e gerenciar o manual.

![Centro de conhecimento](assets/knowledge-center.png){width="800" zoomable="yes"}

1. Na navegação à esquerda, expanda **[!UICONTROL Administração]**, selecione **[!UICONTROL Configurações de Administração]** e selecione **[!UICONTROL Centro de Conhecimento]**.
1. Defina o **[!UICONTROL Nome da empresa]** e a **[!UICONTROL URL da empresa]** que a Marketo Qualifier usa para pesquisar sua empresa e rascunhar emails.
1. Faça upload das ações de vendas, perfis de clientes ideais (ICPs), guias de posicionamento e outros materiais de apoio de vendas nos formatos PDF, PPTX ou DOCX.
1. Selecione **[!UICONTROL Criar Manual]**.

A página mostra o status do manual criado mais recentemente e fornece a próxima ação depois de fazer upload do conteúdo. Para recuperar o status mais recente após uma compilação, selecione **[!UICONTROL Atualizar]**.

Cada documento carregado também exibe seu status de processamento, como **[!UICONTROL Pronto]**, e quando foi atualizado pela última vez.

>[!NOTE]
>
>Um manual pode levar até 24 horas para ser processado.

Quando o manual estiver pronto, os representantes poderão usá-lo em dois lugares:

* **Prompts de email de saída** — Em um prompt de ponto de contato, nomeie o documento e descreva o contexto a ser usado. Por exemplo, digite `Use the ABC positioning guide from the Knowledge Center and focus on the security value proposition`. Consulte [Configurar pontos de contato](outbound-workflows.md#step-3-generate-and-review-touchpoints).
* **Chat de IA**: consulte o Centro de Conhecimento em sua pergunta. Por exemplo, digite `From the Knowledge Center, help me position our security solution for ABC Corp before tomorrow's call`. Consulte [Chat de IA](ai-assistant.md).

Em ambos os casos, o conteúdo gerado reflete a mensagem no seu manual em vez da pesquisa genérica.

## Configurar opção de não participação de email global

1. Na navegação à esquerda, expanda **[!UICONTROL Administração]** e selecione **[!UICONTROL Configurações de Administração]**.
1. Selecione as **[!UICONTROL Configurações de email]** em **[!UICONTROL Conformidade]**.
1. Ative **[!UICONTROL Incluir link para opção de não participação em todos os emails]** para anexar um rodapé de cancelamento de inscrição a emails de saída.
1. Em **[!UICONTROL Modelo de mensagem de recusa]**, digite o texto do rodapé. Inclua o token `{opt_out_link}` no qual o link para cancelar inscrição deve aparecer.

As configurações são salvas automaticamente.

Quando um cliente potencial seleciona o link, o Marketo Qualifier interrompe o envio de emails para esse cliente potencial e sincroniza o status de recusa para o CRM conectado. A Marketo Qualifier também reconhece solicitações claras de recusa na resposta por email de um cliente potencial, como &quot;pare de me enviar por email&quot; ou &quot;cancelar inscrição&quot;, e marca o cliente potencial como recusa automática. O mesmo status e selo **[!UICONTROL Opted out]** se aplicam e nenhum outro ponto de contato é enviado. Nenhuma configuração adicional é necessária. Respostas que não pedem claramente para parar, como &quot;não no momento&quot;, não são tratadas como recusas. Consulte [Solicitações de recusa em respostas](outbound-workflows.md#opt-out-requests-in-replies).

## Referência: amostra de parâmetros da API

Sua equipe de CRM pode usar esses exemplos para confirmar os retornos de acesso de leitura dos campos de cliente potencial esperados.

### Exemplo de OData do Dynamics

```text
$select=fullname,_ownerid_value,leadid,emailaddress1,jobtitle,statuscode,createdon,modifiedon,statecode
$filter=_ownerid_value eq '<crmUserId>' [AND additional filters]
$expand=Lead_ActivityPointers(...),parentaccountid(...)
$orderby=modifiedon desc
```

### Exemplo de Salesforce SOQL

```sql
SELECT Id, Salutation, FirstName, LastName, Name, Title, Company, Email,
  LeadSource, Status, OwnerId, LastModifiedDate, LastActivityDate, CreatedDate,
  (SELECT Id, Subject, ActivityDate, Status FROM Tasks ORDER BY ActivityDate DESC LIMIT 1),
  (SELECT Id, Subject, ActivityDateTime FROM Events ORDER BY ActivityDateTime DESC LIMIT 1)
FROM Lead
WHERE OwnerId = '<crmUserId>' AND IsDeleted = false
ORDER BY LastModifiedDate DESC
```

>[!MORELIKETHIS]
>
>* [Introdução](getting-started.md)
>* [Clientes Potenciais](prospects.md)
