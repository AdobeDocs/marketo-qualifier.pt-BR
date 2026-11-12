---
title: Configurar o plug-in do CRM
description: Saiba como instalar o plug-in do Marketo Qualifier CRM no Salesforce ou no Microsoft Dynamics 365. Configure ações do Salesforce para workflows e campanhas do Marketo.
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: da701e37-3227-4187-b68a-914277252a79
    internal-label: Integrations
  - id: f8f8b877-7295-5853-989f-e21f73bc94c4
    internal-label: Administration
subfeature_v2:
  - id: d2fe5f36-5653-5902-937c-9d3026104284
    internal-label: CRM integrations
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: df256cf271296b82fab2ed10725a0d6bd165e05b
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%
---

# Configurar o plug-in do CRM

Instale o plug-in do CRM [!DNL Adobe Marketo Qualifier] para que os representantes possam usar [!DNL Marketo Sales Insights] e insights gerados pela IA nas páginas de registro de cliente potencial, contato e conta sem sair do Salesforce ou Microsoft Dynamics 365. O plug-in também fornece uma exibição inicial para [priorizar clientes em potencial no seu CRM](admin-settings.md#prioritize-leads-in-the-crm-plugin).

No Salesforce, os representantes também podem adicionar prospetos a fluxos de trabalho de saída ou campanhas do Marketo de exibições de leads e listas de contatos e páginas de registros individuais.

## Antes de começar

Certifique-se de que as pessoas que instalam e usam o plug-in tenham o acesso necessário:

* **Administrador do Salesforce**: permissão para instalar pacotes e editar layouts de página.
* **Administrador do Microsoft Dynamics 365**: permissão para importar soluções para o ambiente de destino no Power Apps.
* **Representantes**: acesso ao Marketo Qualifier e aos registros relevantes do CRM.

A instalação do plug-in é separada de [conectar seu CRM ao Marketo Qualifier](getting-started.md#connect-your-crm).

## Instalar no Salesforce

Instale o pacote e, em seguida, adicione seus componentes às páginas de registro que os representantes usam.

1. Abra a [página de instalação do Salesforce](https://experience.adobe.com/solutions/OneAdobe-sales-workflow-optimizer-sales-insight-ui/install/sales-insight?crm=salesforce) e entre no Salesforce como administrador.
1. Na página de instalação do pacote, selecione **[!UICONTROL Instalar para Todos os Usuários]** e **[!UICONTROL Instalar]**.

   Você ainda pode controlar o acesso de usuários individuais por meio de permissões do Salesforce.

1. Quando for solicitado a aprovar o acesso de terceiros, marque a caixa de seleção de aprovação e selecione **[!UICONTROL Continuar]**.
1. Quando a instalação terminar, selecione **[!UICONTROL Concluído]**.

   A instalação leva alguns minutos. Confirme se o pacote aparece na página **[!UICONTROL Pacotes Instalados]**.

1. No Lightning App Builder, edite as páginas de registro de lead, contato e conta e adicione os componentes do Marketo Qualifier.

### Adicionar ações às exibições de lista

Configure **[!UICONTROL Adicionar ao Fluxo de Trabalho de Saída]** e **[!UICONTROL Adicionar ao Marketo Campaign]** separadamente para exibições das listas de Clientes Potenciais e de Contatos. Use os botões incluídos no pacote para evitar duplicatas.

1. Vá para **[!UICONTROL Configuração]** > **[!UICONTROL Gerenciador de Objetos]** e selecione **[!UICONTROL Cliente Potencial]** ou **[!UICONTROL Contato]**.
1. Abra **[!UICONTROL Botões, Links e Ações]** e localize os botões da lista **[!UICONTROL Adicionar AMQ ao Fluxo de Trabalho de Saída]** e **[!UICONTROL Adicionar AMQ ao Marketo Campaign]**.
1. Abra o **[!UICONTROL Layout do Botão de Exibição de Lista]** do objeto e selecione **[!UICONTROL Editar]**.

   Dependendo da configuração do Salesforce, o layout de exibição de lista pode estar em **[!UICONTROL Layouts de Pesquisa]** > **[!UICONTROL Exibição de Lista]**.

1. Mova ambos os botões da lista para **[!UICONTROL Botões Selecionados]** e salve.
1. Repita para o outro objeto.

Os representantes selecionam um ou mais registros em uma exibição de lista e, em seguida, selecionam a ação.

### Adicionar ações para gravar páginas

As ações de página de registro devem ser configuradas separadamente dos botões de exibição de lista. Adicionar ambas as ações a cada layout de página de cliente potencial e contato em uso.

1. Vá para **[!UICONTROL Configuração]** > **[!UICONTROL Gerenciador de Objetos]** e selecione **[!UICONTROL Cliente Potencial]** ou **[!UICONTROL Contato]**.
1. Abra **[!UICONTROL Botões, Links e Ações]** e localize os botões de detalhes **[!UICONTROL Adicionar AMQ ao Fluxo de Trabalho de Saída]** e **[!UICONTROL Adicionar AMQ ao Marketo Campaign]**.
1. Abra **[!UICONTROL Layouts de Página]** e edite um layout atribuído a seus representantes.
1. Adicione ambos os botões de detalhes às **[!UICONTROL Ações do Salesforce Mobile e Lightning Experience]** e salve.
1. Repita o procedimento para cada layout aplicável e para o outro objeto.

As ações são exibidas na barra de ação do registro ou em seu menu e se aplicam ao registro que está sendo exibido.

>[!NOTE]
>
>Essas ações funcionam no desktop Salesforce Lightning Experience, não no aplicativo móvel do Salesforce. A seção de layout chamada **[!UICONTROL Ações do Salesforce Mobile e Lightning Experience]** também é usada para ações de desktop.

### Substituir um botão ausente

Se um botão empacotado estiver ausente, crie uma substituição nos **[!UICONTROL Botões, Links e Ações]** do objeto.

1. Selecione **[!UICONTROL Novo Botão ou Link]**.
1. Insira um rótulo para a ação, como `Add to Outbound Workflow` ou `Add to Marketo Campaign`.
1. Escolha o **[!UICONTROL Botão de Lista]** para uma exibição de lista ou o **[!UICONTROL Botão de Página de Detalhes]** para uma página de registro.
1. Defina **[!UICONTROL Source de Conteúdo]** como **[!UICONTROL Página do Visualforce]** e escolha a página de ação do pacote que corresponda à ação, objeto e posicionamento.

   A lista de clientes potenciais, os detalhes do cliente potencial, a lista de contatos e os posicionamentos de detalhes do contato usam páginas diferentes. Confirme se a página selecionada corresponde ao posicionamento que você está configurando.

1. Para um botão de lista, selecione **[!UICONTROL Exigir Seleção de Linha]**.
1. Salve o botão e adicione-o ao layout de botão de exibição de lista ou às ações de página de registro apropriadas, conforme descrito acima.

### Verificar ações do Salesforce

Depois de salvar os layouts, confirme se ambas as ações aparecem nas exibições de listas de clientes potenciais e de contatos e nas páginas de registro. Teste cada ação de lista com registros selecionados e cada ação de página de registro de um registro individual.

Se uma ação não estiver disponível ou não abrir, use estas verificações:

| Problema | O que verificar |
| --- | --- |
| Botão ausente em uma exibição de lista | Confirme se o botão de lista está em **[!UICONTROL Botões Selecionados]** no **[!UICONTROL Layout do Botão de Exibição de Lista]** do objeto correto e salve o layout. |
| Botão ausente em uma página de registro | Confirme se o botão de detalhes está em **[!UICONTROL Ações do Salesforce Mobile e da Experiência do Lightning]** no layout atribuído ao usuário. Se sua organização usar Ações dinâmicas, verifique também a visibilidade da ação da página de registro. |
| Opção de página esperada indisponível ao criar um botão | Verifique se o tipo de exibição é **[!UICONTROL Botão de Lista]** para uma exibição de lista ou **[!UICONTROL Botão de Página de Detalhes]** para uma página de registro. |
| A ação não abre ou mostra um erro de acesso | Confirme se o usuário tem acesso ao Marketo Qualifier e aos registros selecionados. |

## Instalar no Microsoft Dynamics 365

Importe o pacote de plug-in para o ambiente em que seus representantes trabalham.

1. Abra a [página de instalação do Microsoft Dynamics 365](https://experience.adobe.com/solutions/OneAdobe-sales-workflow-optimizer-sales-insight-ui/install/sales-insight?crm=dynamics) e baixe o arquivo ZIP do pacote.
1. Entre no [Power Apps](https://make.powerapps.com/) como administrador e selecione o ambiente de destino.
1. Abra **[!UICONTROL Soluções]** e selecione **[!UICONTROL Importar solução]**.
1. Selecione **[!UICONTROL Procurar]**, escolha o arquivo ZIP baixado e selecione **[!UICONTROL Avançar]**.
1. Revise os detalhes do pacote e selecione **[!UICONTROL Próximo]**.
1. Mantenha o valor da variável de ambiente preenchido previamente e selecione **[!UICONTROL Importar]**.
1. Aguarde a mensagem de confirmação na parte superior da página de que a solução foi importada com êxito.

A importação leva alguns minutos.

>[!MORELIKETHIS]
>
>* [Priorizar clientes em potencial no plug-in do CRM](admin-settings.md#prioritize-leads-in-the-crm-plugin)
>* [Integrações](integrations.md)
>* [Introdução](getting-started.md)
