# Lançamento de Setembro

## Envios em massa

A funcionalidade permite criar campanhas de WhatsApp para pacientes usando templates aprovados. É possível segmentar o público, acompanhar o envio por status, identificar campanhas com baixo desempenho e acessar os chats de cada destinatário.

Também há reenvio apenas para contatos não alcançados, registro de auditoria e automações por campanha para encerrar ou transferir enviossem respostas. Os disparos ficam visíveis no histórico da conversa e contam como um consumo por destinatário.

{% content-ref url="../../funcionalidades/envios/envios-em-massa.md" %}
[envios-em-massa.md](../../funcionalidades/envios/envios-em-massa.md)
{% endcontent-ref %}

## **Atualização no Funil de leads**

A clínica poderá agora ter uma visão de kanban no Funil de leads e definir uma regra única de conversão em **Configurações do funil**:

* **Comparecimento no atendimento**: converte após a primeira consulta.
* **Orçamento fechado**: converte quando o orçamento é aprovado.

As etapas automáticas passam a ser obrigatórias e definidas pela regra escolhida. A seção de controles individuais de status automáticos será removida.

Os indicadores e a listagem de **Leads convertidos** acompanharão a regra ativa. Aging, motivos de perda e perda automática por inatividade podem ser configurados pela clínica.

{% content-ref url="../../funcionalidades/leads/" %}
[leads](../../funcionalidades/leads/)
{% endcontent-ref %}

## Novo tipo de envio automático: Pós-agendamento <a href="#id-71787702-2197-4ad9-9da6-4f6402924540" id="id-71787702-2197-4ad9-9da6-4f6402924540"></a>

Novo tipo em **Envios automáticos**: **Pós-agendamento**. Agora é possível enviar mensagens após a criação de um agendamento, com intervalo configurável e filtros de público. O envio respeita o horário da consulta e é cancelado em cenários específicos de cancelamento ou reagendamento.

<details>

<summary>Saiba mais</summary>

Agora você pode configurar mensagens automáticas para serem enviadas logo após a criação de um agendamento. Use esse tipo de envio para dar boas-vindas, compartilhar orientações de preparo, documentos ou instruções de chegada sem precisar esperar a consulta se aproximar.

### Configure o envio <a href="#e39134be-6646-49b1-b985-417b3bde2313" id="e39134be-6646-49b1-b985-417b3bde2313"></a>

Em **Envios automáticos**, selecione o tipo **Pós-agendamento** e defina:

* O intervalo para o envio, entre **10 minutos e 30 dias**.
* A unidade do intervalo: minutos, horas ou dias.
* Os filtros de público disponíveis, como tipo de atendimento, profissional, unidade, procedimento e forma de pagamento.
* Um template aprovado para a mensagem.

Quando você não selecionar opções em um filtro, o envio será considerado para todos os agendamentos naquele critério.

### Quando a mensagem é enviada <a href="#id-49c38246-fb4c-49b9-bf8f-9c9c1b556c8c" id="id-49c38246-fb4c-49b9-bf8f-9c9c1b556c8c"></a>

A contagem do intervalo começa no momento em que o agendamento é criado. Por exemplo, ao configurar o envio para 1 hora, uma mensagem será programada para uma hora após o agendamento.

A mensagem só é programada quando o horário calculado fica antes da consulta. Se o intervalo resultar no mesmo horário da consulta ou em um horário posterior, não haverá envio.

> O Pós-agendamento é disparado apenas na criação do agendamento. Editar ou reagendar depois não cria uma nova mensagem.

### Cancelamentos e reagendamentos <a href="#id-58e73823-9c3e-4ce6-954f-1591d32a5dd7" id="id-58e73823-9c3e-4ce6-954f-1591d32a5dd7"></a>

Enquanto a mensagem ainda estiver pendente:

* Ao cancelar a consulta, o envio é cancelado.
* Ao reagendar para uma data posterior ao horário programado, o envio é mantido.
* Ao reagendar para o mesmo horário ou antes da mensagem programada, o envio é cancelado.
* Ao desativar ou excluir a configuração, os envios pendentes dela também são cancelados.

Depois que a mensagem é enviada, cancelar, reagendar ou concluir a consulta não gera um novo envio de Pós-agendamento.

### Outras regras do envio <a href="#b335ca1d-115a-48c9-a172-1cb524cbdc18" id="b335ca1d-115a-48c9-a172-1cb524cbdc18"></a>

Você pode ter mais de uma configuração de Pós-agendamento aplicável ao mesmo agendamento. Cada configuração gera seu próprio envio, respeitando a ordem das automações e as regras já existentes para evitar mensagens duplicadas.

As regras de bloqueio de número, canal e template continuam sendo aplicadas. Cada tentativa fica registrada como enviada ou com falha.

***

</details>



## Novo Dashboard de atendimento

O Dashboard de atendimento foi ampliado com novas análises do Agente Flow, capacidade e qualidade da operação. Agora é possível acompanhar receita, tempos de resposta e resolução, conversões, transferências, distribuição dos atendimentos, desempenho por setor e origem, avaliações e ranking de atendentes, com filtros por período, clínica, canal e setor.

{% content-ref url="../../funcionalidades/dashboard-de-atendimentos.md" %}
[dashboard-de-atendimentos.md](../../funcionalidades/dashboard-de-atendimentos.md)
{% endcontent-ref %}
