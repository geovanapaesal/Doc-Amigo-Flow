# Botões de Ação nos Templates do Amigo Flow (WhatsApp API)

Agora sua clínica pode adicionar botões interativos aos templates de mensagem que executam ações diretamente no sistema — sem que o atendente precise interpretar a resposta do paciente e fazer nada manualmente.

Essa nova funcionalidade permite:

* adicionar botões de ação ao criar ou editar um template,
* escolher o tipo de botão e a ação que ele executa,
* personalizar o texto exibido para o paciente,
* e registrar automaticamente cada ação no histórico da conversa.

Tudo isso dentro do próprio construtor de mensagens do Amigo Flow.<br>

### Tutorial — Como adicionar botões de ação a um template

### 1️⃣ Acessando o Criador de Templates

No menu de Mensagens / Modelos do Amigo Flow, selecione "Criar modelo" (ou edite um modelo já existente).

Você verá a área de edição do template com:

* Corpo do texto
* Cabeçalho (se aplicável)
* Preview à direita em tempo real

### 2️⃣ Adicionando um Botão de Ação

Na área de edição, abaixo do corpo da mensagem, clique no botão:

**➕ Adicionar ação**

<br>

<img src="../../../.gitbook/assets/unknown.png" alt="" height="324" width="624">

<br>

Isso abrirá um menu com os tipos de botão disponíveis:

| Botão               | O que acontece quando o paciente clica                        |
| ------------------- | ------------------------------------------------------------- |
| Confirmar consulta  | Status da agenda atualizado para "Confirmado" automaticamente |
| Cancelar consulta   | Status da agenda atualizado para "Cancelado" automaticamente  |
| Assinar documento   | Fluxo de assinatura pelo Signbox é aberto                     |
| Ver orçamento       | Fluxo de envio de orçamento do paciente                       |
| Ver Documento       | Fluxo de envio de documentos pelo prontuário do paciente      |
| Falar com Atendente | Transfere automaticamente para o setor principal              |



\
&#xNAN;**✔️ Regras importantes**

* Cada tipo de botão já vem com a ação vinculada por padrão — não é possível alterar qual ação um botão executa.
* A validação impede que o template seja salvo sem pelo menos o tipo de botão selecionado.
* Ao escolher o botão, ele entra na lista do template pronto para uso.



### 3️⃣ Personalizando o Texto do Botão

Depois de escolher o tipo, você pode editar o rótulo exibido ao paciente no WhatsApp.

**Como funciona:**

* Clique sobre o botão adicionado para editar o texto exibido
* O texto é livre — você pode trocar "Confirmar consulta" por algo como "Confirmar presença ✅"
* A ação vinculada ao botão continua a mesma, independente do texto escolhido<br>

### 4️⃣ Editando ou Removendo Botões

**✔️ Remover**

* Na área de botões do template, basta excluir o botão adicionado

**✔️ Editar**

* Basta clicar sobre o botão e ajustar o texto exibido



### 5️⃣ Preview em Tempo Real

À direita, o painel de preview mostra exatamente como o botão será exibido para o paciente no WhatsApp.

**O preview:**

* Atualiza automaticamente a cada alteração
* Permite validar imediatamente o texto e a posição do botão na mensagem

Isso reduz erros e ajuda a confirmar a experiência antes de enviar para aprovação.



### 6️⃣ Validação Antes de Salvar ou Enviar

Antes de permitir salvar ou enviar o template para aprovação, o sistema verificará:

**✔️ Configuração correta dos botões**

* Tipo de botão selecionado
* Texto do botão preenchido



### 7️⃣ Como a Ação é Executada

Depois que o template é aprovado e enviado ao paciente, a ação acontece assim:

1. O paciente clica no botão diretamente na conversa do WhatsApp
2. O Flow recebe a ação
3. O sistema identifica a ação associada ao botão e executa automaticamente — atualiza a agenda, abre o link, ou inicia o fluxo do Signbox, dependendo do tipo de botão
4. O sistema retorna uma confirmação ao paciente
5. A ação é registrada no histórico da conversa do paciente



**✔️ Regras importantes**

* Cada botão está vinculado a apenas uma ação. Para cobrir mais de uma ação na mesma mensagem, é necessário adicionar mais de um botão ao template.
* O registro no histórico é feito automaticamente pelo Flow, sem necessidade de ação do atendente.

### Como o uso desses botões ajuda na sua clínica?

#### Ver Orçamento

Clínicas que trabalham com orçamentos agora podem incluir um botão de acesso direto nos templates do WhatsApp. Quando o paciente clica, o sistema recupera o link do orçamento dele e envia automaticamente na conversa, sem que o atendente precise intervir.

O botão pode ser disparado pela página de gestão de orçamentos ou pela aba de orçamentos no cadastro do paciente.

Atenção: se a janela de atendimento da Meta estiver aberta no momento do disparo, o sistema não envia o template — em vez disso, envia a mensagem diretamente no formato "Assine seu orçamento: \[link]", acompanhada de um aviso para o atendente. Se a unidade ainda não tiver um template de orçamento aprovado, o sistema exibe um alerta com um atalho para o fluxo de criação de template.

#### Ver Documento (Prontuário)

Receitas, declarações, resultados de exame e demais documentos do prontuário do paciente agora podem ser compartilhados via template com um clique. O atendente seleciona qual documento será atrelado à mensagem no momento do disparo, e o sistema gera um link único para aquele paciente e documento.

O botão pode ser disparado diretamente pelo prontuário do paciente — inclusive por usuários sem vínculo com um canal de atendimento, desde que exista um setor configurado.

Assim como no botão de orçamento: se a janela da Meta estiver aberta, o sistema não envia template, envia a mensagem diretamente no formato "Veja seu documento: \[link]". Se não houver template de documento aprovado para a unidade, aparece um aviso com atalho para criação.

#### Falar com Atendente

Um novo botão de transferência pode ser adicionado a qualquer template. Quando o paciente clica, a conversa é transferida automaticamente do fluxo automatizado para a fila de atendimento humano — sem que o paciente precise responder manualmente ou o atendente precisar monitorar a conversa esperando uma sinalização.

O texto do botão pode ser renomeado livremente. Exemplos de uso: "Falar com atendente", "Preciso de ajuda", "Quero reagendar".
