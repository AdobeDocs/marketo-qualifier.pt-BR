---
title: Público-alvo inteligente (Beta)
description: Saiba como usar o Público-alvo inteligente (Beta) para criar listas de contas, adicionar dados de CRM e sinais de crescimento, priorizar leads e adicioná-los a um Fluxo de trabalho de saída.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
badgeBeta: label="Beta" type="Informative"
source-git-commit: 633ca975d4fe58bdcc84caf633049ae1190b0f56
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%
---

# Público-alvo inteligente (Beta)

O Smart Audience (Beta) ajuda você a encontrar as contas e as pessoas que trabalharão em seguida no [!DNL Adobe Marketo Qualifier]. Descreva seu público-alvo em linguagem simples, refine a lista de contas com dados de CRM e sinais de crescimento, encontre leads relevantes e adicione leads selecionados a um fluxo de trabalho de saída.

Trabalhe na exibição de lista com sua grade, filtros e botões ou use o chat para descrever o que deseja. Ambos trabalham na mesma lista: as alterações em um aparecem no outro. Se uma alteração não aparecer imediatamente, selecione **[!UICONTROL Atualizar]**.

O rastreador de progresso na parte superior de cada lista mostra três estágios: **[!UICONTROL Criar lista de público-alvo inteligente]**, **[!UICONTROL Priorizar clientes em potencial]** e **[!UICONTROL Adicionar ao fluxo de trabalho de saída]**.

A página de aterrissagem inclui um exemplo de reprodução automática do fluxo completo de cinco etapas, desde a descrição das contas até a adição de leads para um fluxo de trabalho de saída. Uma apresentação **[!UICONTROL Como funciona]** explica a jornada passo a passo e abre automaticamente quando você não tem listas. Você pode ignorar a apresentação e reabri-la a qualquer momento selecionando **[!UICONTROL Como funciona]**.

## Antes de começar

O público-alvo inteligente requer um Salesforce conectado ou um Microsoft Dynamics 365 CRM. Ele lê os dados do CRM e não grava no CRM. Para obter instruções de conexão, consulte [Introdução](getting-started.md#connect-your-crm).

É possível criar até 100 listas. Cada lista contém até 500 contas e 2.000 leads. Contas ou clientes potenciais acima desses limites não são adicionados. Restrinja seus critérios ou divida o público em várias listas, por exemplo, por região ou segmento.

## Descrever e visualizar contas

Comece com uma descrição das contas que deseja acessar. A visualização não salva uma lista.

1. Abra **[!UICONTROL Público-alvo inteligente]** e selecione **[!UICONTROL Novo público-alvo inteligente]** ou **[!UICONTROL Criar lista]**.
1. Use as opções de adição rápida e os prompts de exemplo na página de criação de público-alvo para iniciar sua solicitação ou descreva as contas desejadas no chat.

   Por exemplo, digite `Find healthcare accounts with revenue over $50M`.

1. Revise o número de contas correspondentes e a amostra na visualização.

Sua solicitação pode incluir estes critérios:

| Critérios | Exemplos |
| --- | --- |
| Perfil da empresa | Setor, contagem de funcionários, receita anual, tipo de conta e classificação |
| Localização | Região, país, estado ou cidade |
| Propriedade | Suas contas atribuídas a um proprietário nomeado |
| Canal de processamento | Contas com ou sem uma oportunidade aberta, sujeitas aos [limites da Salesforce](#current-scope-and-limits) |
| Detalhes da conta | Nome, site ou domínio e número da conta |

Outros exemplos de solicitações incluem:

* `Accounts in the US with more than 1000 employees`
* `My accounts in Germany or France`
* `Accounts with no open opportunity`

Se parte de uma solicitação não puder ser aplicada aos seus dados do CRM, o chat identificará a condição ignorada. A visualização reflete somente as condições que foram aplicadas. Revise essas omissões antes de salvar.

## Salvar ou refinar a visualização

Salve a visualização quando ela corresponder ao público-alvo desejado.

1. Para alterar a visualização, envie uma nova solicitação com as condições desejadas. Nada é salvo até que você confirme.
1. Quando a visualização estiver pronta, peça ao chat para salvá-la como uma lista e dar um nome a ela.
1. Revise as contas salvas na guia **[!UICONTROL Contas]**.

As listas salvas são exibidas como cartões com detalhes de conta, lead e enriquecimento para ajudá-lo a escolher qual lista abrir.

É possível renomear uma lista a partir de sua página. Para excluir uma lista, abra-a e selecione **[!UICONTROL Excluir lista de público-alvo inteligente]**.

>[!CAUTION]
>
>Excluir uma lista remove permanentemente suas contas, clientes potenciais e colunas do Público-alvo inteligente. Ela não exclui registros do CRM.

## Enriquecer e selecionar contas

Adicione colunas de informações para ajudar a decidir quais contas trabalhar. Solicite uma coluna ou um sinal por solicitação.

Para adicionar informações do CRM, insira uma solicitação como `Add a column showing which accounts have an open opportunity`. Consulte [Escopo atual e limites](#current-scope-and-limits) para restrições de Salesforce.

Para adicionar sinais de crescimento, selecione **[!UICONTROL Enriquecer contas]** na exibição de lista ou perguntar no chat. Os sinais disponíveis incluem:

| Sinal | O que ele mostra |
| --- | --- |
| Financiamento | Eventos recentes de financiamento e financiamento |
| Contratação | Aberturas de emprego recentes e demanda de contratação |
| Sinais de expansão | Novos escritórios, novos mercados e anúncios de expansão |
| Mudanças tecnológicas | Adições e alterações na pilha de tecnologia de uma empresa |
| Desistências | Informações de layout solicitadas pelo chat |

Por exemplo, digite `Which of these accounts have raised funding recently?` ou `Which of these accounts have had layoffs?`.

Em listas grandes, a adição de um sinal pode levar alguns minutos. Siga o progresso mostrado na lista, revise cada nova coluna e mantenha-a ou descarte-a. Depois de adicionar uma coluna de enriquecimento, selecione **[!UICONTROL Mostrar coluna]** para exibi-la. A coluna é destacada brevemente para que você possa encontrá-la sem alterar a ordem da coluna.

As guias **[!UICONTROL Contas]** e **[!UICONTROL Clientes potenciais]** mostram suas contagens de registro. A coluna **[!UICONTROL Conta]** permanece na exibição enquanto você rola horizontalmente pela lista.

Para refinar e priorizar as contas:

1. Na guia **[!UICONTROL Contas]**, abra **[!UICONTROL Filtros]**.
1. Filtre por conta, domínio, setor, proprietário, funcionários mínimos ou máximos, receita mínima ou máxima ou colunas personalizadas. Colunas personalizadas são as colunas CRM e de sinal que você adicionou. Por exemplo, filtre por contas em que a coluna de contratação está definida como `Yes`.
1. Opcionalmente, selecione **[!UICONTROL Priorizar contas]** para classificar as contas por pontuação.
1. Remova todas as contas que você não deseja que funcionem.

Os filtros são salvos com a lista. Clientes potenciais são encontrados somente para as contas filtradas, portanto, defina filtros de conta antes de priorizar clientes potenciais.

## Localizar e priorizar clientes em potencial

Encontre pessoas relevantes nas contas que você selecionou. Em **[!UICONTROL Priorizar clientes em potencial]**, escolha uma predefinição ou descreva as pessoas que você deseja no chat.

| Predefinição | Contatos encontrados |
| --- | --- |
| **[!UICONTROL Contatos de vendas]** | Contatos do Diretor de Vendas e do Gerente de Vendas |
| **[!UICONTROL Contatos de marketing]** | VP de contatos do gerente de marketing e marketing |
| **[!UICONTROL Contatos de produtos]** | SVP de Contatos de Gerente de Produto e Produto |
| **[!UICONTROL Contatos de tecnologia]** | Diretor de TI e vice-presidente de contatos de engenharia |
| **[!UICONTROL Todos os contatos do CRM]** | Cada contato disponível nas contas, até o limite de 2.000 clientes potenciais |

Para uma solicitação de chat, digite `Find VP and Director level people at these accounts`, `Find C-level executives (CEO, CTO, CFO) at these accounts` ou `Find managers at these accounts`.

Revise os resultados na guia **[!UICONTROL Clientes potenciais]**. Cada lead mostra o nome, cargo, conta, email, proprietário e pontuação. Filtre por prioridade, se um endereço de email está disponível, pontuação mínima ou máxima ou se o lead está em um fluxo de trabalho. A coluna **[!UICONTROL Raciocínio]** explica por que cada lead é classificado onde está.

Se a guia **[!UICONTROL Clientes Potenciais]** estiver vazia, siga suas orientações para encontrar clientes em potencial para suas contas selecionadas.

### Como as pontuações funcionam

As pontuações variam de 0 a 100. Uma pontuação mais alta indica melhor ajuste e mais disponibilidade para engajamento. Os mesmos dados produzem a mesma pontuação.

As pontuações são codificadas por cores para ajudar as correspondências mais fortes a se destacarem. Analise a pontuação numérica e o raciocínio ao comparar contas ou leads em vez de depender apenas da cor.

Uma pontuação combina:

* **Adequação**: se a conta corresponde ao seu perfil de cliente ideal, como setor e tamanho.
* **Sinais de compra e crescimento**: sinais como contratações, financiamento e alterações de liderança. Os sinais recentes contam mais.
* **Contexto de vendas**: um contexto como um cliente existente com uma oportunidade de expansão.

Revise o raciocínio e os dados disponíveis antes de decidir com quem entrar em contato.

## Adicionar leads a um workflow de saída

Depois de revisar os clientes potenciais, adicione aqueles que deseja a um Fluxo de trabalho de saída existente.

1. Na guia **[!UICONTROL Clientes potenciais]**, filtre e selecione os clientes potenciais desejados. Por exemplo, selecione leads com um endereço de email e uma pontuação mínima de 70.
1. Selecione **[!UICONTROL Adicionar ao fluxo de trabalho de saída]**.
1. Escolha o workflow e confirme.
1. Revise a confirmação. A coluna **[!UICONTROL Fluxo de trabalho]** mostra **[!UICONTROL Atribuído]** para os clientes potenciais adicionados.

Você também pode pedir ao chat para adicionar os leads a um workflow por nome. Se você não souber o nome, peça ao chat para listar os workflows disponíveis. Verifique o nome do workflow e o número de leads na resposta.

A adição de clientes em potencial não substitui a análise e a aprovação de email. Siga as etapas para [revisar emails gerados](outbound-workflows.md#review-and-refine-generated-emails) e [aprovar e inscrever prospetos](outbound-workflows.md#approve-and-enroll-prospects) antes do envio do alcance externo.

## Escopo e limites atuais

Durante a Beta, lembre-se dos seguintes limites:

* Solicite uma coluna ou um sinal por solicitação.
* O público-alvo inteligente usa campos de conta padrão do CRM. Não há suporte para campos personalizados do CRM.
* Não há suporte para a filtragem por produtos de uma conta.
* Para o Salesforce, não está disponível encontrar contas que tenham uma oportunidade aberta. Encontrar contas sem oportunidade em aberto funciona com ambos os CRMs.
* Para o Salesforce, as solicitações sobre contratação para uma função específica, como representantes de vendas, não estão disponíveis.

>[!MORELIKETHIS]
>
>* [Contas](accounts.md)
>* [Clientes Potenciais](prospects.md)
>* [Fluxos de Trabalho de Saída](outbound-workflows.md)
>* [Bate-papo de IA](ai-assistant.md)
