---
icon: chart-kanban
---

# Painéis

### Visão Geral

A funcionalidade **Painéis** do **Amigo Flow** é o espaço onde o usuário acompanha o **andamento dos fluxos de agendamentos da clínica em formato Kanban,** permitindo visualizar, organizar e agir sobre as etapas dos fluxos de **confirmação de consultas** e **reengajamento pós-falta**.

Com ela, é possível identificar facilmente quais pacientes **confirmaram, reagendaram, cancelaram ou ainda não responderam**, otimizando o trabalho do time de atendimento e garantindo maior previsibilidade da agenda.

### Acesso e Navegação

A funcionalidade está disponível no menu superior, dentro da aba **“Painéis”**.

Ao acessar, o sistema exibe uma visão dividida em **colunas**, cada uma representando um **status do fluxo** ativo (por exemplo, Confirmações ou Faltas).

No canto superior esquerdo, há um **seletor de fluxo**, que permite alternar entre:

* 🗓️ **Confirmações**
* 🚫 **Faltas**

### Estrutura do Painel Kanban

Cada painel é composto por **colunas de status**, que representam as etapas de acompanhamento dos fluxos.

#### Fluxo de Confirmações

Colunas padrão:

1. **Não confirmados** – pacientes ainda não contatados ou que não responderam.
2. **Confirmados** – pacientes que confirmaram presença.
3. **Reagendados** – pacientes que solicitaram novo horário.
4. **Cancelados** – pacientes que desistiram ou cancelaram a consulta.

#### Fluxo de Faltas

Colunas padrão:

1. **Mensagem enviadas** – paciente está sendo contatado para reagendar.
2. **Reagendados** – pacientes que já remarcaram a consulta.
3. **Cancelados** – pacientes que ainda não optaram por reagendar.

#### Estrutura de Cada Card (Paciente)

Cada **card** no Kanban representa um **atendimento ou agendamento individual**.

Os cartões exibem informações essenciais para o atendente agir rapidamente:

* **Nome e telefone do paciente**
* **Procedimento** (ex: Botox, Peeling, Microagulhamento)
* **Data e horário do agendamento**
* **Local da unidade**
* **Profissional responsável**
* **Logs da ação** (ex: “Agendado pelo Agente Flow” ou “Confirmado por Alberto Ribeiro”)
* **Tempo desde que a mensagem foi enviada** (ex: “Contatado há 1 hora”)
* Ícone do **WhatsApp** para abertura rápida da conversa

### Ações Disponíveis

#### Transitar entre fluxos

* O usuário pode alternar entre os fluxos **“Confirmações”** e **“Faltas”** através do seletor no topo esquerdo.
* A visualização e as colunas se adaptam automaticamente conforme o tipo de fluxo escolhido.

#### Buscar contato

* Use o campo de busca para **filtrar pacientes** pelo nome ou telefone.
* A pesquisa é instantânea e percorre todas as colunas do painel atual.

#### Filtros avançados

* O ícone de **filtro** permite refinar a visualização por:
  * Profissional responsável
  * Unidade de atendimento
  * Data da consulta
  * Tipo de atendimento

#### ⠇ Menu de Ações do Cartão

* Ao clicar nos **três pontos** no canto do cartão, o atendente pode:
  * **Abrir conversa** com o paciente (via Chat rápido)
  * **Adiantar** envio/ **Reenviar** mensagem
  * **Reagendar** o paciente

### Casos de Uso

| Cenário                                                 | Ação do Usuário                                                              | Resultado Esperado                                                 |
| ------------------------------------------------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| A clínica quer saber quem ainda não confirmou           | Seleciona o painel de “Confirmações” e observa a coluna “Mensagens Enviadas” | Mostra todos os pacientes pendentes de resposta                    |
| Paciente responde “Sim” no WhatsApp                     | O cartão muda para “Confirmados”                                             | O status é atualizado quando a tela é atualizada                   |
| Paciente pede novo horário                              | O atendente arrasta o cartão para “Reagendados”                              | O sistema abre o modal de reagendamento e registra a atualização   |
| Paciente não comparece à consulta                       | O agendamento aparece no fluxo de “Faltas”                                   | O envio é realizado no horário programado pela clínica             |
| Paciente tem mais de uma consulta agendada no mesmo dia | O sistema agrupa os envios em uma mesma mensagem                             | paciente pode confirmar, cancelar ou reagendar nenhum, um ou todos |

### Benefícios para a Clínica

* Visão **centralizada e visual** do status de todos os agendamentos.
* Redução de **faltas** por acompanhamento ativo e rápido.
* **Integração direta** com o agente inteligente (IA), permitindo que confirmações automáticas apareçam em tempo real.
* **Organização e produtividade**: cada atendente sabe exatamente o que precisa fazer.

### Boas Práticas

* Atualize os status manualmente apenas quando necessário; o sistema faz a maioria das atualizações automaticamente.
* Use o filtro de **profissional** para revisar confirmações por agenda de cada médico.
* Monitore os **cancelamentos e reagendamentos** para identificar padrões (como horários problemáticos).
* Mantenha a comunicação empática ao contatar pacientes que não compareceram.

### Suporte e Dúvidas

Em caso de:

* Cartões duplicados,
* Dados desatualizados, ou
* Falha na movimentação automática dos status

entre em contato com o nosso **Suporte .**&#x20;
