# Envios automáticos

<figure><img src="../../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

#### Visão Geral

Os **Envios Automáticos** do **Amigo Flow** permitem que sua clínica envie mensagens de WhatsApp para pacientes e leads de forma completamente automática — sem que nenhuma pessoa precise acionar o envio manualmente.

Você configura uma vez, define as regras, e o sistema cuida do resto: envia **no momento certo**, para **o público certo**, com **a mensagem certa**.

> 💡 Imagine ter 80 consultas agendadas para amanhã. Em vez de ligar ou enviar mensagem para cada paciente confirmando a presença, o sistema já fez isso enquanto sua equipe focava no que realmente importa: cuidar das pessoas.

***

#### O que você pode automatizar

Os Envios Automáticos cobrem os principais momentos da jornada do paciente:

<table><thead><tr><th>Tipo de Envio</th><th>Para que serve</th><th data-type="checkbox">Lançado?</th></tr></thead><tbody><tr><td><strong>Confirmação</strong></td><td>Reduzir faltas pedindo que o paciente confirme a consulta com antecedência</td><td>true</td></tr><tr><td><strong>Pré-atendimento</strong></td><td>Enviar orientações e preparos antes da consulta</td><td>false</td></tr><tr><td><strong>Pós-atendimento</strong></td><td>Manter o contato após a consulta com cuidados, feedbacks ou instruções</td><td>false</td></tr><tr><td><strong>Falta</strong></td><td>Entrar em contato quando o paciente não comparece</td><td>true</td></tr><tr><td><strong>Aniversário</strong></td><td>Fortalecer o relacionamento com uma mensagem no dia do aniversário</td><td>false</td></tr><tr><td><strong>Orçamento em aberto</strong></td><td>Lembrar o paciente sobre um orçamento pendente e aumentar a conversão</td><td>false</td></tr><tr><td><strong>Cobrança</strong></td><td>Enviar lembretes financeiros de forma automática</td><td>false</td></tr></tbody></table>

***

#### Como criar um Envio Automático

**1. Acesse a tela de Envios Automáticos**

No menu lateral, vá até **Envios > Envios Automáticos** e clique em **+ Criar envio automático**.

**2. Escolha o tipo de automação**

Um catálogo vai aparecer com todas as opções organizadas em categorias:

* **Agendamentos** — Confirmação, Pré-atendimento, Pós-atendimento, Falta
* **Cobrança** — Cobrança, Orçamento em aberto
* **Engajamento** — Aniversário

Selecione o tipo que deseja configurar para avançar.

> 💡 Mudou de ideia? O botão **"Alterar"** no topo da tela permite trocar o tipo sem precisar começar do zero.

**3. Configure nas 3 abas**

Cada envio é configurado em três abas. Você só precisa preencher o mínimo (Canal + Modelo + pelo menos um Período) para conseguir salvar.

**Aba 1 — Mensagem e objetivo**

* **Canal:** selecione o número de WhatsApp por onde a mensagem vai sair. Só aparecem canais ativos.
* **Modelo:** escolha o template aprovado. Ao selecionar, um preview é exibido ao lado com as variáveis já preenchidas (nome do paciente, data, horário).
* **Objetivo do envio:** campo opcional para descrever a intenção do envio. Aparece no card da listagem para facilitar a identificação — útil quando você tiver várias automações ativas.

**Aba 2 — Quando enviar**

Define o momento em que a mensagem vai ser disparada.

* Escolha o **número** e a **unidade** (horas, dias ou semanas) antes ou depois do evento.
* Clique em **+ Adicionar período** para incluir mais de um horário de disparo no mesmo envio — por exemplo, 48h antes e 2h antes.

> ⚠️ Períodos com a mesma regra de envio não são permitidos. A ordem que eles aparecem na tela não afeta quando vão disparar.

**Aba 3 — Filtros**

Segmente quem vai receber o envio. Por padrão, a automação vale para todos — mas você pode restringir por critérios específicos.

Os filtros disponíveis variam conforme o tipo de envio escolhido:

* **Tipo de atendimento** — Confirmação, Pré, Pós, Falta
* **Profissional** — Confirmação, Pré, Pós, Falta
* **Unidade** — todos os tipos
* **Procedimento** — Confirmação, Pré, Orçamento em aberto
* **Forma de pagamento** — Confirmação, Pré, Pós
* **Gênero / Sexo** — Aniversário
* **Materiais e medicamentos** — Orçamento em aberto
* **Solicitante** — Orçamento em aberto

Todos os filtros são **multi-seleção** — você pode marcar mais de uma opção ao mesmo tempo.

**4. Salve e ative**

O botão **"Salvar e ativar"** fica habilitado quando os campos obrigatórios estão preenchidos. Ao clicar, o envio fica **Ativo** imediatamente e começa a monitorar os eventos configurados.

#### Gerenciando seus envios

A tela principal mostra todos os envios em formato de cards. Cada card exibe:

* Ícone e nome do tipo de envio
* Objetivo registrado
* Status: **Ativo** ou **Inativo**
* Canal associado
* Tags resumidas dos filtros aplicados

Em cada card você pode:

* **Editar** — ajustar qualquer configuração
* **Ativar / Desativar** — pausar sem precisar excluir
* **Excluir** — remove o envio e cancela todos os disparos futuros vinculados

Use a **busca por nome** e os **filtros** no topo da tela para encontrar envios específicos rapidamente.

#### Como funciona por dentro

O sistema foi desenvolvido para ser confiável e não incomodar o paciente com mensagens desnecessárias:

* **Sem duplicatas:** a mesma mensagem nunca é enviada duas vezes para o mesmo paciente no mesmo horário.
* **Reagendamentos:** se um atendimento for reagendado, os disparos são recalculados automaticamente para o novo horário.
* **Envio pausado:** se o envio estiver desativado, nenhuma mensagem sai — mesmo que o evento ocorra.
* **Cancelamento automático:** ao desativar ou excluir um envio, os disparos já agendados (ainda não enviados) são cancelados.
* **Múltiplos envios do mesmo tipo:** você pode ter, por exemplo, duas Confirmações ativas com públicos diferentes. O sistema gerencia cada uma de forma independente.

Cada envio realizado fica registrado no **histórico de conversas** do paciente no chat, com log de sucesso ou falha.

#### Casos de uso práticos

| Cenário                       | Configuração sugerida                                | Resultado                                                |
| ----------------------------- | ---------------------------------------------------- | -------------------------------------------------------- |
| Reduzir faltas em consultas   | Confirmação 24h antes + 2h antes                     | Paciente confirma com antecedência; equipe sabe quem vem |
| Preparo para exame com jejum  | Pré-atendimento 48h antes, filtrado por procedimento | Paciente recebe orientação no momento certo              |
| Fidelização pós-consulta      | Pós-atendimento 24h após finalização                 | Paciente recebe cuidados e se sente acompanhado          |
| Recuperar orçamentos parados  | Orçamento em aberto após 5 dias sem aprovação        | Clínica lembra o paciente sem esforço manual             |
| Relacionamento no aniversário | Aniversário no dia, 1 disparo por ano                | Paciente recebe parabéns da clínica                      |

#### Dúvidas frequentes

**Posso ter mais de um envio do mesmo tipo ativo?**\
Sim. Você pode ter duas Confirmações com templates e filtros diferentes — por exemplo, uma para pacientes particulares e outra para convênios.

**O que acontece com os disparos quando desativo um envio?**\
Todos os disparos futuros ainda não enviados são cancelados automaticamente. Você pode reativar quando quiser.

**Se o paciente reagendar, a mensagem é reenviada?**\
Sim. O sistema recalcula os períodos com base no novo horário. Se o novo agendamento bater com uma janela configurada, a mensagem é enviada — sem duplicatas para o mesmo horário.

**Posso usar qualquer template de mensagem?**\
Só aparecem para seleção os modelos já aprovados no canal de WhatsApp escolhido. Ao selecionar, o preview é exibido com as variáveis preenchidas.

**Por qual canal as mensagens são enviadas?**\
Atualmente apenas pelo **WhatsApp**. O campo de seleção de canal já está preparado para receber novos canais no futuro.

#### Boas práticas

* Dê um **objetivo claro** em cada envio, facilita muito quando você tiver várias automações ativas ao mesmo tempo.
* Use **múltiplos períodos** em automações de confirmação para aumentar a taxa de resposta.
* Revise os **filtros** antes de ativar: um envio mal segmentado pode gerar mensagens irrelevantes para o paciente.
* Prefira **desativar** em vez de excluir quando quiser pausar temporariamente — você mantém toda a configuração salva.
