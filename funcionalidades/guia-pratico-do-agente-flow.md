---
icon: robot
---

# Guia prático do Agente Flow

### _Como ele funciona, por que funciona assim e como isso protege sua clínica e seus pacientes_

O Agente Flow é o assistente virtual da sua clínica dentro do WhatsApp — ele agenda, reagenda, confirma horários e responde dúvidas gerais sobre a clínica, sempre seguindo padrões rígidos de segurança, LGPD e boas práticas em saúde.

Este documento explica, de forma simples, **como ele pensa**, **por que toma determinadas decisões** e **qual é o comportamento esperado em cada situação**.

## 1. **O que o Agente Flow faz (e por que isso gera valor)**

O Agente Flow foi criado para:

* **Agendar consultas com precisão:**\
  Baseado no que o paciente informa — médico, convênio, unidade, tipo de atendimento e datas disponíveis.
* **Responder dúvidas administrativas**\
  Exemplos: horários, unidades, serviços oferecidos, médicos, convênios aceitos.
* **Garantir segurança em todos os passos**\
  Antes de qualquer ação, ele **confirma informações**, não expõe informações privadas e nunca assume nada que não venha de fonte segura (Base de conhecimento fornecida pela clínica).
* **Reduzir erros de agendamento**\
  Ele cruza automaticamente as informações: se o médico atende o convênio, se o procedimento existe na unidade, se a data faz sentido, etc.
* **Evitar riscos legais**\
  Ele segue diretrizes rígidas para não fornecer orientações médicas — garantindo conformidade com normas de segurança clínica e LGPD.

## 2. **O que ele NÃO faz (e por que isso é obrigatório para a sua segurança)**

O Agente Flow **não pode**:

❌ Explicar procedimentos\
❌ Passar preparos\
❌ Falar sobre pós-operatório\
❌ Interpretar exames\
❌ Falar de doses de remédios\
❌ Dar diagnósticos ou opiniões clínicas

Isso não é limitação técnica — é **proteção da sua clínica**.

#### **Por quê?**

1. **LGPD**: qualquer resposta médica sem supervisão pode caracterizar _ato médico_ — juridicamente crítico.
2. **Risco clínico**: pacientes podem interpretar instruções incorretamente.
3. **Segurança**: o assistente não é um profissional de saúde.
4. **Responsabilização**: informações sobre preparo, medicamentos ou diagnósticos **devem sempre partir de um humano**.

{% hint style="warning" %}
**Quando o paciente fizer perguntas desse tipo, o Agente Flow transfere imediatamente para um atendente humano** — silenciosamente e no momento certo.
{% endhint %}

## 3. **Como o Agente garante LGPD e segurança de dados**

O Agente Flow segue práticas rígidas:

* **Nunca informa dados sensíveis**\
  CPF, endereço, RG, dados de nascimento e informações privadas são sempre tratados com confirmação extra ou transferência.
* **Não revela informações de outros pacientes**\
  Nem insinua duplicidade de cadastro, divergências ou qualquer dado interno.
* **Não “inventa” informações**\
  Tudo vem da configuração oficial da clínica: médicos, unidades, convênios, eventos e horários.
* **Sempre confirma antes de executar ações sensíveis**\
  Agendamento, reagendamento ou cancelamento só acontecem após confirmação explícita do paciente.

## 4. **Como ele entende as mensagens do paciente**

O agente interpreta a frase inteira, não palavras soltas.

#### Exemplos de intenção:

* “Queria marcar com o Dr. João pela Amil na Unidade Centro.”
* “Quais horários tem para limpeza hoje?”

Ele identifica automaticamente **todas as entidades** citadas (médico + convênio + procedimento + unidade) e cruza as informações em API para evitar erros.

Se alguma relação não existir, ele não responde com suposições — ele explica que não conseguiu confirmar a combinação.

## 5. **Como o agendamento funciona**&#x20;

O fluxo sempre segue estas etapas:

1. **Forma de pagamento** (convênio ou particular) - Se a clínica não possui convênios, essa etapa é assumida automaticamente como particular
2. **Unidade**
3. **Tipo de consulta/procedimento**
4. **Médico**
5. **Datas e horários disponíveis**
6. **Confirmação do paciente**
7. **Criação do agendamento**

Cada etapa é validada por dados reais da clínica obtidos via API — garantindo consistência e evitando agendamentos inválidos.

#### Por que seguir esse fluxo importa?

* Evita marcações erradas.
* Mantém a fila organizada.
* Previne divergências de convênio/médico.
* Reduz retrabalho e chamados internos.

## 6. **Quando o Agente transfere para um humano (e por que)**

O Agente Flow transfere automaticamente nos casos abaixo:

* **Conteúdo Médico Restrito**\
  Preparos, remédios, sintomas, pós-operatório, protocolos.
* **Quando falta segurança na informação**\
  Se algo não existir na API ou estiver inconsistente.
* **Quando o usuário pede ações que fogem do escopo**\
  Avaliação de valor, documentação, questões financeiras, dúvidas jurídicas, exames complexos etc.
* **Quando o usuário deseja:**
  * cancelar para terceiros
  * reagendar para outra pessoa
  * alterar médico/procedimento/unidade de um agendamento existente
* **Em caso de erro na operação**\
  Nunca diz “deu erro”. Transfere diretamente.

Essa política mantém a clínica **protegida, organizada e dentro das normas de segurança da informação**.

## 7. **Como o Agente lista datas e horários**

Ele segue um padrão pensado para clareza e organização:

* Lista **apenas horários futuros**
* Agrupa em períodos: manhã, tarde e noite
* Mostra **3 opções por turno**
* Só lista horário **após definir convênio ou particular**
* Usa apenas dados reais do calendário do médico

## 8. **Agendamentos para terceiros (dependentes)**

O Agente só realiza agendamentos — nunca cancelamentos, reagendamentos ou ações sensíveis para terceiros.

Para garantir segurança e LGPD:

* Primeiro coleta CPF
* Verifica se o cadastro do dependente existe na clínica
* Pede autorização explícita
* Só então segue para o agendamento

Tudo isso evita que uma pessoa tente manipular dados de outra sem permissão.

## 9. **Por que o Agente age assim?**&#x20;

À primeira vista, pode parecer interessante deixar o Agente Flow com um comportamento totalmente aberto e personalizado por clínica, com prompts soltos, textos livres e lógicas criadas caso a caso.\
Na prática, em saúde, isso é **perigoso**.

Nós escolhemos um modelo de comportamento **padronizado, testado e protegido**, e isso traz um valor enorme para a sua clínica:

#### **Segurança e LGPD acima de tudo**

Um prompt aberto pode levar o agente a:

* inventar informações,
* responder temas clínicos,
* agir fora do escopo,
* expor dados sensíveis.

Isso cria risco jurídico e pode comprometer a segurança do paciente. Por isso, a lógica central é fechada e controlada.

#### **Comportamento validado e confiável**

Cada decisão do agente foi testada em centenas de cenários reais antes de chegar ao usuário.\
Fluxos, respostas e regras foram refinados para:

* evitar erros de agendamento,
* impedir orientações médicas,
* garantir consistência em todas as clínicas.

Um prompt totalmente configurável apagaria essa garantia.

#### **Personalização com responsabilidade**

A clínica pode personalizar:

* informações,
* tom de voz,
* serviços,
* conhecimento do agente

Mas não pode alterar o “cérebro crítico” do agente — é nele que ficam as proteções de segurança, LGPD e governança.

#### **Menos risco, mais estabilidade**

Comportamentos padronizados garantem:

* previsibilidade,
* redução de falhas,
* atualizações seguras,
* auditoria fácil,
* experiência uniforme para o paciente.

O resultado?\
Um agente que _sempre funciona_, _nunca improvisa_ e protege de ponta a ponta o atendimento da clínica.

