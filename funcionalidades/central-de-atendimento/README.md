---
icon: messages
---

# Central de Atendimento

## Visão geral

Reformulamos a central de atendimento do Amigo Flow. Nela, a equipe da clínica conversa com pacientes e leads de **diferentes canais em um só lugar**. Hoje são WhatsApp e Instagram.

Sem sair da central, você pode:

* organizar as conversas por fila;
* acompanhar quem está conduzindo cada atendimento: o agente de IA ou uma pessoa da equipe;
* consultar o perfil do contato;
* resolver demandas como agendar, criar tarefa ou enviar um orçamento.

### Conceitos importantes

* **Conversa:** troca de mensagens com um contato em um canal.
* **Contato:** quem está do outro lado. Pode ser **Paciente**, quando já tem cadastro no Amigo Clinic, **Lead**, quando ainda não tem, ou um **Contato,** quando é alguém sem vínculo com o sistema.
* **Etiqueta:** marcação do **contato** criada pela clínica, como "orçamento aberto" ou "black friday".
* **Tema:** classificação do **assunto da conversa**, escolhida de uma lista definida pela clínica, como Agendamento, Orçamento ou Financeiro.

## 1. Filas de atendimento

As conversas ficam separadas em filas. Assim, você vê primeiro o que precisa da sua ação.

| Fila                 | O que mostra                                      |
| -------------------- | ------------------------------------------------- |
| **Minhas conversas** | Atendimentos atribuídos a você                    |
| **Com o agente**     | Atendimentos conduzidos pelo agente de IA         |
| **Em aguardo**       | Conversas que ainda não têm atendente responsável |
| **Todos**            | Todos os atendimentos ativos da clínica           |
| **Histórico**        | Conversas encerradas                              |

Cada fila mostra um contador com o número de conversas. Quando uma fila está vazia, uma mensagem explica o motivo.

<figure><img src="../../.gitbook/assets/Captura de Tela 2026-10-29 às 15.15.32.png" alt=""><figcaption></figcaption></figure>

## 2. Lista de conversas

Cada item da lista mostra:

* foto ou iniciais do contato;
* nome do contato, ou o telefone se o nome não estiver cadastrado;
* canal da conversa (WhatsApp ou Instagram);
* responsável pelo atendimento: o agente Flow ou uma pessoa da equipe;
* trecho da última mensagem, horário e indicador de mensagens não lidas.

A lista se atualiza sozinha quando chegam novas mensagens, sem precisar recarregar a página. Por padrão, as conversas aparecem pela última mensagem. Você também pode ordená-las por **tempo de espera**. Um destaque visual indica atendimentos que passaram do prazo de resposta configurado pela clínica.

### Busca e filtros

Você pode buscar pelo nome ou pelo telefone do contato dentro da fila selecionada. Também pode filtrar por:

* canal;
* tema;
* situação;
* responsável;
* etiquetas.

Ao combinar filtros, aparecem apenas as conversas que atendem a todos eles. A busca e os filtros continuam aplicados quando você troca de fila.

## 3. Iniciar uma conversa

Use **Nova conversa** para falar com um contato que ainda não escreveu para a clínica:

1. Busque o contato.
2. Escolha o canal no painel lateral.

> No Instagram, só é possível iniciar uma conversa quando a janela de 72 horas está aberta, ou seja, quando o contato enviou mensagem há menos de 72 horas. Essa é uma regra da Meta.

Uma conversa só entra em **Minhas conversas** quando você **inicia o atendimento** de fato:

* **Janela do WhatsApp aberta:** aceitar a conversa já inicia o atendimento.
* **Janela do WhatsApp encerrada:** escolha um modelo de mensagem aprovado para retomar o contato.

Se a clínica ainda não tem WhatsApp conectado, a central mostra o passo a passo para conectar a conta.

## 4. Janela de atendimento do WhatsApp

A Meta define uma janela de 24 horas, contadas a partir da última mensagem do contato. Na conversa, você vê se essa janela está aberta e quanto tempo falta para ela encerrar.

* **Janela aberta:** você pode enviar mensagens livres, áudios e anexos.
* **Janela encerrada:** o campo de mensagem dá lugar à seleção de **modelos aprovados**. Você vê uma prévia do modelo já preenchida com os dados do contato.

Para enviar com segurança:

* Só aparecem para seleção os modelos aprovados pela Meta.
* Se o contato pediu para não receber mensagens, o envio fica bloqueado e você vê um aviso.
* Se um envio falhar, você vê o motivo, como janela encerrada ou número inválido.

> Para criar novos modelos e enviá-los para aprovação da Meta, use o fluxo de **Campanhas**.

## 5. Agente de IA e equipe na mesma conversa

Na lista e na conversa, você sempre vê quem está conduzindo o atendimento: o agente de IA ou uma pessoa da equipe.

* **Assumir:** com um clique, o atendimento passa para você e o agente é pausado. Assim, o contato não recebe respostas duplicadas.
* **Devolver para o agente:** uma confirmação avisa que o agente voltará a responder.
* **Pausa automática:** o agente também passa a conversa para a equipe quando o contato pede atendimento humano, quando o assunto sai do que ele foi configurado para atender ou quando ele atinge o limite de tentativas.
* **Duas pessoas ao mesmo tempo:** se duas pessoas tentarem assumir a mesma conversa, quem clicou primeiro fica com ela e a outra pessoa é avisada.

### Transferências

Você pode transferir uma conversa para outro atendente ou para um setor e, se quiser, registrar o motivo. A conversa vai para a fila de quem recebeu a transferência. Se o responsável ficar indisponível, a conversa volta para **Em aguardo** depois do tempo configurado pela clínica.

### Notas internas

As notas internas têm visual diferente das mensagens e **nunca são enviadas ao contato**. Mencione uma pessoa da equipe para notificá-la, com acesso direto à conversa.

O histórico da conversa registra, com data e horário, quem assumiu, transferiu, pausou o agente ou encerrou o atendimento.

## 6. Etiquetas e temas

### Etiquetas: organizam o contato

* Ficam vinculadas ao contato e permanecem até alguém removê-las.
* Servem para filtrar a base e montar públicos em **Campanhas**.
* Cada contato pode ter até **10 etiquetas**. Assim, a classificação continua objetiva e fácil de usar em filtros e campanhas.
* Administradores criam, renomeiam, mesclam e arquivam etiquetas. Atendentes podem sugerir novas etiquetas para aprovação.
* Antes de criar uma etiqueta, o sistema sugere etiquetas parecidas, para evitar duplicidade.
* Etiquetas aplicadas por automações têm identificação própria e indicam a regra que as aplicou.

### Temas: classificam o assunto da conversa

* Uma conversa pode ter mais de um tema, adicionado inclusive durante o atendimento.
* A lista de temas é definida pelos administradores da clínica.
* Ao encerrar uma conversa, o agente de IA pode sugerir um tema. A sugestão só é aplicada depois que alguém da equipe confirma.
* A clínica pode exigir pelo menos um tema para encerrar o atendimento. Essa opção vem desligada por padrão.

## 7. Ações a partir da conversa

Resolva a demanda sem sair do atendimento:

* **Criar tarefa:** defina prazo e responsável. A tarefa aparece em **Meu dia** de quem for o responsável.
* **Criar oportunidade:** o formulário já abre com o contato preenchido, e o sistema avisa se existir uma oportunidade parecida.
* **Agendar consulta:** siga o fluxo da agenda e volte ao chat ao terminar. Se o contato for um lead, o sistema oferece criar o cadastro antes.
* **Enviar documento ou orçamento:** envie e acompanhe a situação pela conversa.
* **Criar anotação no prontuário:** disponível apenas para pacientes.

Cada ação fica registrada na conversa, com acesso direto ao item criado. Quando uma ação não está disponível para leads, o botão aparece desabilitado com uma explicação.

## 8. Perfil do contato

O painel ao lado da conversa reúne nome, foto, telefone, e-mail, cidade e responsável atual. O contato aparece identificado como **Paciente** ou **Lead**. Para leads, você encontra o botão **Criar cadastro**. Para pacientes, o botão **Abrir no Amigo Clinic**. Alertas clínicos, como alergias, aparecem em destaque no topo do painel.

O painel tem os seguintes blocos:

* **Etiquetas:** consulte, adicione e remova etiquetas.
* **Atendimentos:** próximo agendamento em destaque e atendimentos recentes.
* **Oportunidades:** oportunidades abertas, com valor e etapa.
* **Tarefas:** tarefas abertas e seus responsáveis.
* **Documentos:** documentos assinados ou pendentes, com opção de reenviar.
* **Anotações:** anotações registradas sobre o contato.

Você pode fechar o painel para ganhar espaço na conversa.

## 9. Campo de mensagem

Quando a janela do canal permite, você pode:

* digitar mensagens;
* enviar áudios e emojis;
* anexar arquivos, como PDFs, imagens e documentos;
* usar respostas rápidas;
* enviar modelos aprovados no WhatsApp.
