---
description: Exemplos, sugestões e cadências para clínicas e implantadores
---

# Guia de Mensagens para Envios Automáticos

> **Como usar este guia** Este documento reúne exemplos prontos de mensagens para cada tipo de Envio Automático disponível no Amigo Flow. Os atalhos como `@@nome` e `@@data` são variáveis dinâmicas preenchidas automaticamente pelo sistema no momento do envio.

### Sumário

1. [Confirmação de Consulta](guia-de-mensagens-para-envios-automaticos.md#id-1.-confirmacao-de-consulta-confirmacao)
2. [Pré-atendimento](guia-de-mensagens-para-envios-automaticos.md#id-2.-pre-atendimento-pre-atendimento)
3. [Pós-atendimento](guia-de-mensagens-para-envios-automaticos.md#id-3.-pos-atendimento-pos-atendimento)
4. [Falta](guia-de-mensagens-para-envios-automaticos.md#id-4.-falta-falta)
5. [Aniversário](guia-de-mensagens-para-envios-automaticos.md#id-5.-aniversario-aniversario)
6. [Orçamento em Aberto](guia-de-mensagens-para-envios-automaticos.md#id-6.-orcamento-em-aberto-orcamento-em-aberto)
7. [Apêndice: Boas Práticas de Redação](guia-de-mensagens-para-envios-automaticos.md#apendice-boas-praticas-de-redacao-de-templates-boas-praticas)

***

### 1. Confirmação de Consulta&#x20;

**Objetivo** Reduzir faltas pedindo que o paciente confirme presença com antecedência. Quando o paciente confirma, a equipe já sabe quem vem — e quando não confirma, há tempo de reagir (ligar, reagendar ou abrir a agenda para outro paciente).

**Cadência recomendada**

| Período   | Objetivo                                                                   |
| --------- | -------------------------------------------------------------------------- |
| 48h antes | Aviso principal — tempo suficiente para reorganizar a agenda se necessário |
| 2h antes  | Lembrete final — garante que o paciente não esqueceu no dia                |

{% hint style="info" icon="lightbulb" %}
**Dica:** Configure os dois períodos no mesmo Envio Automático usando o botão **+ Adicionar período**. Usar templates ligeiramente diferentes em cada período torna a experiência mais natural para o paciente.&#x20;
{% endhint %}

#### Exemplos de Templates

**✅ Exemplo 1 — Tom neutro e objetivo&#x20;**_**(48h antes)**_

```
Olá, @@nome! 👋

Passando para lembrar da sua consulta agendada:

📅 Data: @@data
🕐 Horário: @@horario
📍 Unidade: @@unidade
👨‍⚕️ Profissional: Dr(a). @@medico

Para confirmar sua presença, responda SIM a esta mensagem.

Caso precise remarcar, entre em contato o quanto antes.

Atenciosamente,
[Nome da clínica]
```

**✅ Exemplo 2 — Tom acolhedor&#x20;**_**(48h antes)**_

```
Oi, @@nome! 😊

Estamos te esperando! Sua consulta está chegando:

📅 @@data às @@horario
📍 @@unidade
👨‍⚕️ Com Dr(a). @@medico

Responda SIM para confirmar ou entre em contato para reagendar.

Será um prazer te atender! 💙
[Nome da clínica]
```

**✅ Exemplo 3 — Tom curto e direto&#x20;**_**(2h antes — lembrete final)**_

```
@@nome, lembrete rápido! ⏰

Sua consulta com Dr(a). @@medico é hoje às @@horario.
📍 @@unidade

Te esperamos! Responda SIM para confirmar.
[Nome da clínica]
```

**✅ Exemplo 4 — Com instrução de chegada&#x20;**_**(48h antes)**_

```
Olá, @@nome!

Sua consulta está confirmada:

📅 @@data | 🕐 @@horario
📍 @@unidade
👨‍⚕️ Dr(a). @@medico
📋 Tipo: @@tipodeatendimento

Por favor, chegue com 15 minutos de antecedência para realizar o cadastro e os procedimentos de chegada.

Confirme sua presença respondendo SIM. 😊
[Nome da clínica]
```

**✅ Exemplo 5 — Convênio / plano de saúde&#x20;**_**(48h antes)**_

```
Olá, @@nome!

Sua consulta pelo convênio @@convenio está marcada:

📅 @@data às @@horario
📍 @@unidade
👨‍⚕️ Dr(a). @@medico

Lembre-se de trazer:
• Carteirinha do plano @@convenio
• Documento com foto
• Pedido médico (se houver)

Confirme respondendo SIM. Em caso de dúvidas, estamos à disposição!
[Nome da clínica]
```

**✅ Exemplo 6 — Apenas confirmação, sem instruções&#x20;**_**(2h antes — versão mínima)**_

```
@@nome, sua consulta é hoje! 🗓️

⏰ @@horario | 📍 @@unidade

Responda SIM para confirmar sua presença.
[Nome da clínica]
```

***

**Filtros sugeridos para segmentação**

| Segmento                  | Filtro                                   |
| ------------------------- | ---------------------------------------- |
| Pacientes particulares    | Forma de pagamento = Particular          |
| Pacientes de convênio     | Forma de pagamento = \[nome do convênio] |
| Primeira consulta         | Tipo de atendimento = Primeira consulta  |
| Consultas de retorno      | Tipo de atendimento = Retorno            |
| Procedimentos específicos | Procedimento = \[nome do procedimento]   |

***

### 2. Pré-atendimento

**Objetivo** Garantir que o paciente chegue preparado para a consulta ou exame — evitando remarcar por falta de preparo (jejum, exames esquecidos, etc.) e aumentando a qualidade do atendimento.

**Cadência recomendada**

| Período   | Objetivo                                                            |
| --------- | ------------------------------------------------------------------- |
| 48h antes | Enviar orientações com tempo suficiente para o paciente se preparar |
| 24h antes | Reforçar preparos críticos (como jejum) para o dia seguinte         |

{% hint style="info" icon="lightbulb" %}
**Dica:** Use o filtro **Procedimento** para criar envios diferentes por tipo de exame ou consulta. Um template para "consulta de rotina" será muito diferente de um para "colonoscopia". Crie um envio para cada grupo de procedimento.&#x20;
{% endhint %}

***

#### Exemplos de Templates

**✅ Exemplo 1 — Consulta de rotina sem preparo especial&#x20;**_**(48h antes)**_

```
Olá, @@nome! 😊

Sua consulta com Dr(a). @@medico está chegando:

📅 @@data às @@horario
📍 @@unidade

Não é necessário nenhum preparo especial.
Apenas traga seus documentos e, se tiver, exames anteriores relacionados.

Qualquer dúvida, estamos à disposição!
[Nome da clínica]
```

**✅ Exemplo 2 — Exame com jejum&#x20;**_**(48h antes)**_

```
Oi, @@nome! Sua consulta se aproxima. 🗓️

📅 @@data às @@horario
📍 @@unidade
👨‍⚕️ Dr(a). @@medico

⚠️ ATENÇÃO — Preparo obrigatório:
• Jejum de 8 horas antes do exame
• Pode ingerir água
• Evite atividades físicas intensas no dia anterior

Dúvidas? Entre em contato antes da consulta.
[Nome da clínica]
```

**✅ Exemplo 3 — Retorno com exames&#x20;**_**(48h antes)**_

```
Olá, @@nome!

Seu retorno com Dr(a). @@medico está agendado:

📅 @@data às @@horario | 📍 @@unidade

📋 Lembre-se de trazer todos os exames solicitados na sua última consulta para facilitar o atendimento.

Te esperamos! 😊
[Nome da clínica]
```

**✅ Exemplo 4 — Procedimento estético ou odontológico&#x20;**_**(48h antes)**_

```
Oi, @@nome! 🌟

Sua consulta está chegando:

📅 @@data às @@horario
📍 @@unidade
👨‍⚕️ Dr(a). @@medico

Recomendações para seu procedimento:
• Venha com o rosto limpo (sem maquiagem, se aplicável)
• Use roupas confortáveis
• Evite exposição solar intensa no dia anterior

Estamos animados para te receber! 💙
[Nome da clínica]
```

**✅ Exemplo 5 — Primeira consulta&#x20;**_**(24h antes)**_

```
Olá, @@nome!

Amanhã é sua primeira consulta com a gente! 🎉

📅 @@data às @@horario
📍 @@unidade
👨‍⚕️ Dr(a). @@medico

Para agilizar seu atendimento, traga:
• Documento com foto
• Cartão do convênio (se aplicável)
• Lista de medicamentos em uso
• Exames anteriores (se houver)

Chegue com 10 minutinhos de antecedência. Até amanhã! 😊
[Nome da clínica]
```

**✅ Exemplo 6 — Exame de imagem&#x20;**_**(48h antes)**_

```
Olá, @@nome!

Seu exame com Dr(a). @@medico está agendado:

📅 @@data às @@horario
📍 @@unidade

📋 Orientações importantes:
• Traga o pedido médico original
• Traga documento com foto
• Caso use convênio, leve a carteirinha

Dúvidas sobre o preparo? Fale conosco antes do exame.
[Nome da clínica]
```

***

### 3. Pós-atendimento

**Objetivo** Manter o vínculo com o paciente após a consulta — transmitir cuidado, reforçar orientações, solicitar feedback ou incentivar o retorno quando indicado.

**Cadência recomendada**

| Período                | Objetivo                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------------- |
| 24h após finalização   | Mensagem principal de acompanhamento — mais relevante enquanto a consulta ainda está fresca |
| 7 dias após (opcional) | Follow-up para procedimentos específicos ou verificação de evolução                         |

{% hint style="info" icon="lightbulb" %}
**Dica para implantadores:** O pós-atendimento é um diferencial de clínicas que querem fidelizar pacientes. Muitas clínicas ainda não fazem isso — implantá-lo bem gera impacto visível na satisfação. Use o filtro **Tipo de atendimento** para criar mensagens diferentes para primeira consulta vs. retorno.&#x20;
{% endhint %}

***

#### Exemplos de Templates

**✅ Exemplo 1 — Acompanhamento geral&#x20;**_**(24h após)**_

```
Olá, @@nome! 😊

Esperamos que sua consulta com Dr(a). @@medico tenha sido ótima!

Caso tenha alguma dúvida ou precise de mais informações sobre o que foi orientado, estamos aqui para ajudar.

Cuide-se! 💙
[Nome da clínica]
```

**✅ Exemplo 2 — Com solicitação de feedback&#x20;**_**(24h após)**_

```
Oi, @@nome! Tudo bem?

Gostaríamos de saber como foi sua experiência na consulta com Dr(a). @@medico.

⭐ De 1 a 5, como foi seu atendimento?

Sua opinião é muito importante para continuarmos melhorando! 🙏
[Nome da clínica]
```

**✅ Exemplo 3 — Após procedimento estético/cirúrgico&#x20;**_**(24h após)**_

```
Olá, @@nome! 💙

Como você está se sentindo após o procedimento realizado ontem com Dr(a). @@medico?

Lembre-se das orientações recebidas:
• Siga as recomendações de cuidados pós-procedimento
• Em caso de dúvidas ou desconforto incomum, entre em contato imediatamente

Estamos à disposição para o que precisar!
[Nome da clínica]
```

**✅ Exemplo 4 — Incentivo ao retorno / exames solicitados&#x20;**_**(48h após)**_

```
Oi, @@nome!

Passando para lembrar que Dr(a). @@medico pode ter solicitado exames ou indicado um retorno.

📋 Não esqueça de realizar os exames recomendados! Assim conseguimos acompanhar melhor sua saúde.

Para agendar seu retorno ou tirar dúvidas, é só entrar em contato. 😊
[Nome da clínica]
```

**✅ Exemplo 5 — Pós primeira consulta&#x20;**_**(24h após)**_

```
Olá, @@nome! Foi um prazer te receber pela primeira vez! 🎉

Esperamos que sua consulta com Dr(a). @@medico tenha atendido suas expectativas.

Estamos à disposição para qualquer dúvida que surgir. Será sempre um prazer te atender! 💙
[Nome da clínica]
```

**✅ Exemplo 6 — Follow-up semanal pós procedimento&#x20;**_**(7 dias após)**_

```
Olá, @@nome! 😊

Já faz uma semana desde o seu procedimento com Dr(a). @@medico.

Como você está se sentindo? Está tudo bem com a recuperação?

Qualquer dúvida ou sinal diferente, não hesite em entrar em contato conosco.

Cuidar de você é o que nos motiva! 💙
[Nome da clínica]
```

***

### 4. Falta

**Objetivo** Entrar em contato com pacientes que não compareceram à consulta — com empatia, sem julgamento — para entender o que aconteceu, reagendar e manter o vínculo.

**Cadência recomendada**

| Período             | Objetivo                                                                         |
| ------------------- | -------------------------------------------------------------------------------- |
| 2h após o horário   | Contato imediato, ainda com abertura para reagendar no mesmo dia ou dia seguinte |
| 24h após (opcional) | Segunda tentativa para pacientes que não responderam                             |

{% hint style="info" icon="lightbulb" %}
**Atenção:** O tom da mensagem de falta é crítico. Mensagens que soam como cobrança ou julgamento afastam o paciente. O objetivo é sempre acolher e facilitar o reagendamento. Evite palavras como "faltou", "não compareceu" ou "ausente" de forma direta.
{% endhint %}

***

#### Exemplos de Templates

**✅ Exemplo 1 — Tom acolhedor e direto&#x20;**_**(2h após)**_

```
Oi, @@nome! Tudo bem?

Percebemos que você não conseguiu comparecer à sua consulta hoje com Dr(a). @@medico.

Acontece! Se quiser reagendar, é só nos avisar que encontramos o melhor horário para você. 😊

[Nome da clínica]
```

**✅ Exemplo 2 — Com oferta de reagendamento imediato&#x20;**_**(2h após)**_

```
Olá, @@nome!

Notamos que sua consulta com Dr(a). @@medico hoje às @@horario não ocorreu como planejado.

Gostaríamos de ajudar a encontrar um novo horário conveniente para você.

📅 Para reagendar, responda essa mensagem ou ligue para nós. Temos horários disponíveis! 😊
[Nome da clínica]
```

**✅ Exemplo 3 — Tom mais neutro&#x20;**_**(2h após)**_

```
@@nome, olá!

Sua consulta estava agendada para hoje às @@horario na @@unidade.

Se precisar remarcar, estamos à disposição. É só entrar em contato! 😊
[Nome da clínica]
```

**✅ Exemplo 4 — Segunda tentativa / follow-up&#x20;**_**(24h após — sem resposta)**_

```
Olá, @@nome! 😊

Tentamos entrar em contato ontem, mas não conseguimos falar com você.

Sua saúde é importante para nós! Quando quiser reagendar com Dr(a). @@medico, é só nos chamar.

Estaremos aqui! 💙
[Nome da clínica]
```

**✅ Exemplo 5 — Falta em procedimento&#x20;**_**(2h após)**_

```
Oi, @@nome!

Notamos que seu procedimento agendado para hoje às @@horario não aconteceu.

Sabemos que imprevistos acontecem. Quando quiser reagendar, estamos prontos para encontrar o melhor horário para você! 📅

[Nome da clínica]
```

**✅ Exemplo 6 — Falta em primeira consulta&#x20;**_**(2h após)**_

```
Olá, @@nome! Tudo bem?

Sua primeira consulta com Dr(a). @@medico estava marcada para hoje e sentimos sua falta.

Adoraríamos te receber em breve! 😊 Para reagendar, é só responder essa mensagem.

[Nome da clínica]
```

***

### 5. Aniversário

**Objetivo** Fortalecer o relacionamento com o paciente em um momento especial — gerando afeto, lembrança de marca e, potencialmente, estimulando o retorno à clínica.

**Cadência recomendada**

| Período               | Objetivo                          |
| --------------------- | --------------------------------- |
| No dia do aniversário | 1 disparo por ano, no próprio dia |

\{% hint style="info" %\} **Dica para implantadores:** O aniversário é o único envio automático que não está vinculado a um agendamento — ele é acionado pela data de nascimento do paciente. Funciona mesmo para pacientes que não têm consulta marcada. Ótimo para reativar pacientes inativos. \{% endhint %\}

***

#### Exemplos de Templates

**✅ Exemplo 1 — Simples e afetuoso**

```
🎂 Feliz Aniversário, @@nome!

Que este dia seja repleto de alegria, saúde e muito carinho!

Com carinho,
[Nome da clínica] 💙
```

**✅ Exemplo 2 — Com CTA suave de retorno**

```
🎉 Parabéns, @@nome!

Em seu aniversário, desejamos muita saúde e felicidade!

Que tal celebrar cuidando ainda mais de você? Estamos aqui sempre que precisar. 😊

Um abraço,
[Nome da clínica]
```

**✅ Exemplo 3 — Tom mais formal e elegante**

```
Olá, @@nome.

Nesta data tão especial, toda a equipe de [Nome da clínica] deseja a você um feliz aniversário, com muita saúde, conquistas e bem-estar.

Com admiração e carinho,
[Nome da clínica]
```

**✅ Exemplo 4 — Tom descontraído e leve**

```
Ei, @@nome! 🥳

Hoje é SEU dia e a gente não poderia deixar passar sem celebrar com você!

🎂 Feliz aniversário! Que venham muitos e muitos anos com muita saúde e alegria!

[Nome da clínica] 🎉
```

**✅ Exemplo 5 — Clínica infantil / pediátrica**

```
🎈 Hoje é dia de festa!

Parabéns, @@nome! 🎂

Toda a equipe deseja um aniversário cheio de alegria, saúde e muita diversão!

Com carinho,
[Nome da clínica] 💙
```

***

**Sugestão de segmentação por filtro**

| Segmento              | Filtro                                       |
| --------------------- | -------------------------------------------- |
| Todos os pacientes    | Sem filtro (padrão)                          |
| Somente mulheres      | Gênero = Feminino                            |
| Somente homens        | Gênero = Masculino                           |
| Pacientes pediátricos | Criar envio específico com template infantil |

***

### 6. Orçamento em Aberto

**Objetivo** Lembrar o paciente sobre um orçamento pendente de procedimento — estimulando a decisão de aprovação sem pressão excessiva, e recuperando conversões que seriam perdidas sem acompanhamento.

**Cadência recomendada**

| Período                     | Objetivo                                                  |
| --------------------------- | --------------------------------------------------------- |
| 3 dias após a emissão       | Primeiro lembrete suave — o orçamento ainda está fresco   |
| 7 dias após (sem resposta)  | Segundo lembrete — reforça urgência com leveza            |
| 15 dias após (sem resposta) | Última tentativa — desperta curiosidade ou urgência final |

{% hint style="info" icon="lightbulb" %}
**Dica:** Combine o filtro **Procedimento** para criar mensagens específicas por tipo de tratamento (implante, ortodontia, cirurgia, estética). Mensagens contextualizadas têm taxa de retorno significativamente maior do que mensagens genéricas.&#x20;
{% endhint %}

***

#### Exemplos de Templates

**✅ Exemplo 1 — Primeiro lembrete, tom suave&#x20;**_**(3 dias após)**_

```
Olá, @@nome! 😊

Passando para lembrar que seu orçamento ainda está disponível para análise.

Se tiver alguma dúvida sobre os procedimentos, valores ou formas de pagamento, é só nos chamar.

Estamos à disposição para ajudar!
[Nome da clínica]
```

**✅ Exemplo 2 — Segundo lembrete, com abertura para dúvidas&#x20;**_**(7 dias após)**_

```
Oi, @@nome!

Notamos que seu orçamento ainda está em aberto.

Tem alguma dúvida que podemos esclarecer? Sobre o procedimento, parcelamento ou condições especiais?

Estamos aqui para facilitar sua decisão. 💙
[Nome da clínica]
```

**✅ Exemplo 3 — Terceiro contato, senso de encerramento&#x20;**_**(15 dias após)**_

```
@@nome, olá!

Seu orçamento está prestes a expirar e não queremos que você perca essa oportunidade.

Se ainda estiver considerando, este é um bom momento para conversarmos! Entre em contato e vemos como podemos ajudar. 😊

[Nome da clínica]
```

**✅ Exemplo 4 — Focado em condições especiais&#x20;**_**(7 dias após)**_

```
Oi, @@nome! 🌟

Seu orçamento ainda está aguardando sua decisão.

Sabia que temos condições especiais de parcelamento disponíveis? Podemos conversar sobre a melhor forma de viabilizar seu tratamento.

Fale conosco! 😊
[Nome da clínica]
```

**✅ Exemplo 5 — Odontologia / Procedimento longo&#x20;**_**(3 dias após)**_

```
Olá, @@nome!

Passando para lembrar do orçamento do seu tratamento que elaboramos recentemente.

Iniciar logo faz toda a diferença nos resultados! Se tiver dúvidas sobre o procedimento ou as etapas do tratamento, estamos à disposição. 😊

[Nome da clínica]
```

***

**Filtros sugeridos**

| Segmento                             | Filtro                                               |
| ------------------------------------ | ---------------------------------------------------- |
| Orçamentos de alto valor             | Procedimento = \[lista de procedimentos específicos] |
| Pacientes com solicitante específico | Solicitante = \[nome do médico/profissional]         |
| Por material ou tipo                 | Materiais e medicamentos = \[item]                   |

***

### Apêndice: Boas Práticas de Redação

#### ✅ O que funciona bem

| Prática                                    | Por quê funciona                                            |
| ------------------------------------------ | ----------------------------------------------------------- |
| Usar `@@nome` logo no início               | Cria conexão imediata e senso de personalização             |
| Frases curtas e parágrafos pequenos        | Mais fácil de ler em tela de celular                        |
| Emojis com moderação                       | Tornam a mensagem mais amigável sem perder profissionalismo |
| Tom positivo mesmo em mensagens difíceis   | Mantém o paciente como aliado                               |
| CTA claro ("responda SIM", "ligue para X") | O paciente sabe exatamente o que fazer                      |
| Preview das variáveis antes de ativar      | Evita templates com variáveis vazias chegando ao paciente   |

#### ❌ O que evitar

| Prática                                    | Problema                                              |
| ------------------------------------------ | ----------------------------------------------------- |
| Mensagens longas com muita informação      | O paciente não lê até o fim                           |
| Tom formal demais ("Prezado Sr./Sra.")     | Parece robô — quebra a naturalidade do WhatsApp       |
| Muitas informações em uma única mensagem   | Melhor dividir em dois envios com períodos diferentes |
| Cobrar ou pressionar em mensagens de falta | Afasta o paciente ao invés de trazê-lo de volta       |
| Texto sem nenhum CTA                       | O paciente fica sem saber o que fazer                 |
| Usar gírias ou linguagem muito informal    | Pode destoar da imagem da clínica                     |

***

#### Checklist antes de ativar um envio automático

Antes de clicar em **Salvar e ativar**, valide:

* \[ ] O tom da mensagem está adequado para o tipo de envio?
* \[ ] Os períodos de disparo fazem sentido para o fluxo do paciente?
* \[ ] Os filtros aplicados segmentam corretamente o público desejado?
* \[ ] O objetivo do envio foi descrito no campo "Objetivo" para facilitar identificação futura?
* \[ ] Você verificou se já existe outro envio do mesmo tipo ativo para o mesmo público?

#### Estrutura-padrão de um bom template de WhatsApp

```
[Saudação + @@nome]

[Contexto em 1 linha — o que está acontecendo]

[Informação principal — data, hora, local, valor]

[Orientações ou próximos passos, se necessário]

[CTA claro — o que o paciente deve fazer]

[Assinatura da clínica]
```

***

#### Variáveis disponíveis no sistema

| Variável              | Descrição                       |
| --------------------- | ------------------------------- |
| `@@nome`              | Nome do paciente                |
| `@@cpf`               | CPF do paciente                 |
| `@@data`              | Data do agendamento             |
| `@@horario`           | Horário do agendamento          |
| `@@unidade`           | Unidade                         |
| `@@tipodeatendimento` | Tipo de atendimento             |
| `@@medico`            | Médico                          |
| `@@convenio`          | Convênio do paciente            |
| `@@numerodamatricula` | Número da matrícula             |
| `@@naturalidade`      | Naturalidade do paciente        |
| `@@nomedoresponsavel` | Nome do responsável do paciente |
| `@@cpfdoresponsavel`  | CPF do responsável do paciente  |
| `@@nomedamae`         | Nome da mãe do paciente         |
| `@@nomedopai`         | Nome do pai do paciente         |

***

_Documento elaborado para uso interno de clínicas e implantadores do Amigo Flow. Última atualização: Maio 2026_
