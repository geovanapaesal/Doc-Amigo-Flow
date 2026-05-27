---
description: Exemplos, sugestões e cadências para clínicas e implantadores
---

# Guia de Mensagens para Envios Automáticos

> **Como usar este guia** Este documento reúne exemplos prontos de mensagens para cada tipo de Envio Automático disponível no Amigo Flow. Para cada tipo, você encontrará: uma explicação do objetivo, as melhores cadências de envio, múltiplos exemplos de templates com variações de tom, e dicas práticas de configuração.
>
> Os textos entre colchetes — como `[nome_paciente]` e `[data_consulta]` — representam variáveis dinâmicas preenchidas automaticamente pelo sistema.

### Sumário

1. [Confirmação de Consulta](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#confirma%C3%A7%C3%A3o)
2. [Pré-atendimento](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#pr%C3%A9-atendimento)
3. [Pós-atendimento](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#p%C3%B3s-atendimento)
4. [Falta](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#falta)
5. [Aniversário](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#anivers%C3%A1rio)
6. [Orçamento em Aberto](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#or%C3%A7amento-em-aberto)
7. [Apêndice: Boas Práticas de Redação](https://claude.ai/chat/9dd891f5-5f99-4bb7-8ef6-2ba634204985#boas-pr%C3%A1ticas)

***

### 1. Confirmação de Consulta {#confirmação}

#### Objetivo

Reduzir faltas pedindo que o paciente confirme presença com antecedência. Quando o paciente confirma, a equipe já sabe quem vem — e quando não confirma, há tempo de reagir (ligar, reagendar ou abrir a agenda para outro paciente).

#### Cadência recomendada

| Período   | Objetivo                                                                   |
| --------- | -------------------------------------------------------------------------- |
| 48h antes | Aviso principal — tempo suficiente para reorganizar a agenda se necessário |
| 2h antes  | Lembrete final — garante que o paciente não esqueceu no dia                |

> 💡 **Dica para implantadores:** Configure os dois períodos no mesmo Envio Automático usando o botão **+ Adicionar período**. Usar templates ligeiramente diferentes em cada período (um mais formal, outro mais curto) torna a experiência mais natural para o paciente.

***

#### Exemplos de Templates

**✅ Exemplo 1 — Tom neutro e objetivo&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]! 👋

Sua consulta com [nome_profissional] está confirmada para:

📅 [data_consulta]
🕐 [horario_consulta]
📍 [nome_unidade]

Para confirmar sua presença, responda com *SIM*.
Se precisar reagendar, responda com *NÃO* ou entre em contato.

Até lá! 😊
[nome_clinica]
```

***

**✅ Exemplo 2 — Tom acolhedor&#x20;**_**(48h antes)**_

```
Oi, [nome_paciente]! Tudo bem?

Aqui é da [nome_clinica]. 🩺

Queremos confirmar seu agendamento:
📅 *[data_consulta]* às *[horario_consulta]*
👨‍⚕️ Com [nome_profissional]

Você confirma sua presença?
👉 Responda *SIM* para confirmar
👉 Responda *NÃO* se precisar remarcar

Qualquer dúvida, é só falar com a gente. 💙
```

***

**✅ Exemplo 3 — Tom curto e direto&#x20;**_**(2h antes — lembrete final)**_

```
[nome_paciente], lembrete rápido! ⏰

Sua consulta com [nome_profissional] é *hoje, às [horario_consulta]*.

📍 [nome_unidade] — [endereço_unidade]

Até já! 🙂
[nome_clinica]
```

***

**✅ Exemplo 4 — Com instrução de chegada&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]! 

Sua consulta está agendada para *[data_consulta] às [horario_consulta]* com [nome_profissional].

📍 *[nome_unidade]*
[endereço_unidade]

⏱️ Pedimos que chegue *15 minutos antes* para realizar o cadastro ou atualização dos seus dados.

Confirme sua presença respondendo *SIM*.
Precisa remarcar? Responda *NÃO* e entraremos em contato.

[nome_clinica] 💙
```

***

**✅ Exemplo 5 — Convênio / plano de saúde&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]!

Confirmando sua consulta pelo [nome_convenio]:

📅 [data_consulta] às [horario_consulta]
👨‍⚕️ [nome_profissional] — [especialidade_profissional]
📍 [nome_unidade]

⚠️ *Lembre-se de trazer:*
• Carteirinha do plano
• Documento de identidade com foto
• Pedido médico (se necessário)

Confirma sua presença? Responda *SIM* ou *NÃO*.

[nome_clinica]
```

***

**✅ Exemplo 6 — Apenas confirmação, sem instruções&#x20;**_**(2h antes — versão mínima)**_

```
Oi [nome_paciente]! 👋 Só um lembrete que sua consulta é *hoje às [horario_consulta]* aqui na [nome_clinica]. Aguardamos você! 😊
```

***

#### Filtros sugeridos para segmentação

| Cenário                   | Filtro recomendado                       |
| ------------------------- | ---------------------------------------- |
| Pacientes particulares    | Forma de pagamento = Particular          |
| Pacientes de convênio     | Forma de pagamento = \[nome do convênio] |
| Primeira consulta         | Tipo de atendimento = Primeira consulta  |
| Consultas de retorno      | Tipo de atendimento = Retorno            |
| Procedimentos específicos | Procedimento = \[nome do procedimento]   |

***

### 2. Pré-atendimento {#pré-atendimento}

#### Objetivo

Garantir que o paciente chegue preparado para a consulta ou exame — evitando remarcar por falta de preparo (jejum, exames esquecidos, etc.) e aumentando a qualidade do atendimento.

#### Cadência recomendada

| Período   | Objetivo                                                            |
| --------- | ------------------------------------------------------------------- |
| 48h antes | Enviar orientações com tempo suficiente para o paciente se preparar |
| 24h antes | Reforçar preparos críticos (como jejum) para o dia seguinte         |

> 💡 **Dica para implantadores:** Use o filtro **Procedimento** para criar envios diferentes por tipo de exame ou consulta. Um template para "consulta de rotina" será muito diferente de um para "colonoscopia", por exemplo. Crie um envio para cada grupo de procedimento.

***

#### Exemplos de Templates

**✅ Exemplo 1 — Consulta de rotina sem preparo especial&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]! 🩺

Sua consulta com [nome_profissional] está marcada para *[data_consulta] às [horario_consulta]*.

Para aproveitarmos bem o seu tempo, sugerimos que você traga:

📋 Exames ou laudos anteriores relacionados à sua queixa
💊 Lista de medicamentos que usa regularmente
📝 Anotações de sintomas ou dúvidas que queira tirar

Qualquer dúvida, entre em contato. Te esperamos! 💙
[nome_clinica]
```

***

**✅ Exemplo 2 — Exame com jejum&#x20;**_**(48h antes)**_

```
Oi, [nome_paciente]!

Sua consulta/exame está agendado para *[data_consulta] às [horario_consulta]*.

⚠️ *Orientações importantes:*

🚫 *Jejum de 8 horas* antes do exame (água pode ser ingerida normalmente)
💊 Se você usa medicação contínua, pode tomá-la com um pequeno gole d'água, salvo orientação médica diferente
🚗 Recomendamos não vir sozinho, pois poderá sentir-se desconfortável após o procedimento

Dúvidas? Responda esta mensagem ou ligue para [telefone_clinica].

[nome_clinica] 💙
```

***

**✅ Exemplo 3 — Retorno com exames&#x20;**_**(48h antes)**_

\*Filtrar TAs que são nomeados como retorno, se for o caso.

```
Olá, [nome_paciente]! 👋

Seu retorno com [nome_profissional] está marcado para *[data_consulta] às [horario_consulta]*.

Para que a consulta seja mais proveitosa, não esqueça de trazer:

📄 Os exames solicitados na consulta anterior
🗓️ Se ainda não realizou todos os exames, traga os que tiver disponíveis

Precisa de ajuda ou tem alguma dúvida? É só nos chamar.

Até lá! 😊
[nome_clinica]
```

***

**✅ Exemplo 4 — Procedimento estético ou odontológico&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]!

Sua sessão de [procedimento] está agendada para *[data_consulta] às [horario_consulta]* com [nome_profissional].

Antes da sua visita, algumas orientações:

✅ Chegue com a pele/área limpa, sem cremes ou maquiagem
✅ Use roupas confortáveis
✅ Se tiver qualquer desconforto ou sintoma novo, nos avise antes de vir
🚫 Evite exposição solar intensa nas 48h anteriores ao procedimento

Qualquer dúvida, estamos aqui! 💙
[nome_clinica]
```

***

**✅ Exemplo 5 — Primeira consulta (anamnese)&#x20;**_**(24h antes)**_

```
[nome_paciente], amanhã é dia da sua primeira consulta aqui na [nome_clinica]! 🎉

📅 *[data_consulta] às [horario_consulta]*
👨‍⚕️ Com [nome_profissional]

Para agilizar seu atendimento:
• Traga um documento com foto (RG ou CNH)
• Se tiver carteirinha de plano de saúde, traga também
• Chegue 10 minutinhos antes para o cadastro

Estamos ansiosos para te conhecer! 💙
[nome_clinica]
```

***

**✅ Exemplo 6 — Exame de imagem&#x20;**_**(48h antes)**_

```
Olá, [nome_paciente]!

Lembrete do seu exame de *[procedimento]* agendado para *[data_consulta] às [horario_consulta]*.

📍 [nome_unidade] — [endereço_unidade]

⚠️ *Preparo necessário:*
[campo_livre_preparo — preencher conforme o exame]

📄 *Documentos:*
• Pedido médico (original)
• Documento de identidade
• Carteirinha do plano (se convênio)

Dúvidas sobre o preparo? Fale com a gente: [telefone_clinica]

[nome_clinica]
```

***

### 3. Pós-atendimento {#pós-atendimento}

#### Objetivo

Manter o vínculo com o paciente após a consulta — transmitir cuidado, reforçar orientações, solicitar feedback ou incentivar o retorno quando indicado.

#### Cadência recomendada

| Período                | Objetivo                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------------- |
| 24h após finalização   | Mensagem principal de acompanhamento — mais relevante enquanto a consulta ainda está fresca |
| 7 dias após (opcional) | Follow-up para procedimentos específicos ou verificação de evolução                         |

> 💡 **Dica para implantadores:** O pós-atendimento é um diferencial de clínicas que querem fidelizar pacientes. Muitas clínicas ainda não fazem isso — implantá-lo bem gera impacto visível na satisfação. Use o filtro **Tipo de atendimento** para criar mensagens diferentes para primeira consulta vs. retorno.

***

#### Exemplos de Templates

**✅ Exemplo 1 — Acompanhamento geral&#x20;**_**(24h após)**_

```
Olá, [nome_paciente]! 😊

Esperamos que sua consulta com [nome_profissional] tenha sido ótima!

Como você está se sentindo? Se tiver qualquer dúvida sobre as orientações que recebeu ou precisar de alguma informação, estamos aqui para ajudar.

Cuide-se bem! 💙
[nome_clinica]
```

***

**✅ Exemplo 2 — Com solicitação de feedback&#x20;**_**(24h após)**_

```
Oi, [nome_paciente]! Tudo bem?

Ontem você passou por aqui para uma consulta com [nome_profissional] e gostaríamos de saber como foi sua experiência. 😊

Em uma escala de 1 a 5, como você avalia seu atendimento hoje?
⭐ 1 – Ruim
⭐⭐ 2 – Regular
⭐⭐⭐ 3 – Bom
⭐⭐⭐⭐ 4 – Ótimo
⭐⭐⭐⭐⭐ 5 – Excelente

Sua opinião nos ajuda a melhorar cada vez mais! 💙
[nome_clinica]
```

***

**✅ Exemplo 3 — Após procedimento estético/cirúrgico&#x20;**_**(24h após)**_

```
Olá, [nome_paciente]!

Passando para saber como você está se sentindo após o procedimento de *[procedimento]* realizado ontem com [nome_profissional]. 💙

Lembrete dos cuidados pós-procedimento:
✅ [orientação_1]
✅ [orientação_2]
✅ [orientação_3]

Em caso de dúvida, incômodo ou intercorrência, entre em contato imediatamente pelo [telefone_clinica].

Estamos aqui! 🌟
[nome_clinica]
```

***

**✅ Exemplo 4 — Incentivo ao retorno / exames solicitados&#x20;**_**(48h após)**_

```
Oi, [nome_paciente]! 👋

Esperamos que esteja bem após sua consulta com [nome_profissional]!

Se você recebeu solicitação de exames, lembre-se de realizá-los em breve para que o acompanhamento seja feito no tempo certo. 

Quando estiver com os resultados, já pode agendar seu retorno por aqui mesmo ou pelo [telefone_clinica].

Qualquer dúvida, é só nos chamar. Cuide-se! 💙
[nome_clinica]
```

***

**✅ Exemplo 5 — Pós primeira consulta&#x20;**_**(24h após)**_

```
[nome_paciente], foi um prazer ter você aqui na [nome_clinica] pela primeira vez! 🎉

Esperamos que a consulta com [nome_profissional] tenha sido esclarecedora.

Siga as orientações recebidas e, se precisar de qualquer apoio, estamos sempre disponíveis.

Até a próxima! 😊💙
[nome_clinica]
```

***

**✅ Exemplo 6 — Follow-up semanal pós procedimento&#x20;**_**(7 dias após)**_

```
Olá, [nome_paciente]!

Faz uma semana do seu procedimento com [nome_profissional] e queríamos saber como você está. 💙

Está tudo bem? O resultado tem sido o esperado?

Caso precise de alguma orientação adicional ou queira agendar uma avaliação, estamos à disposição.

[nome_clinica]
```

***

### 4. Falta {#falta}

#### Objetivo

Entrar em contato com pacientes que não compareceram à consulta — com empatia, sem julgamento — para entender o que aconteceu, reagendar e manter o vínculo.

#### Cadência recomendada

| Período                       | Objetivo                                                                         |
| ----------------------------- | -------------------------------------------------------------------------------- |
| 2h após o horário da consulta | Contato imediato, ainda com abertura para reagendar no mesmo dia ou dia seguinte |
| 24h após (opcional)           | Segunda tentativa para pacientes que não responderam                             |

> ⚠️ **Atenção para implantadores:** O tom da mensagem de falta é crítico. Mensagens que soam como cobrança ou julgamento afastam o paciente. O objetivo é sempre acolher e facilitar o reagendamento. Evite palavras como "faltou", "não compareceu" ou "ausente" de forma direta.

***

#### Exemplos de Templates

**✅ Exemplo 1 — Tom acolhedor e direto&#x20;**_**(2h após)**_

```
Olá, [nome_paciente]!

Percebemos que você não pôde comparecer à sua consulta com [nome_profissional] hoje.

Sabemos que imprevistos acontecem! 😊

Quando você quiser reagendar, é só responder esta mensagem ou entrar em contato pelo [telefone_clinica].

Estamos à disposição! 💙
[nome_clinica]
```

***

**✅ Exemplo 2 — Com oferta de reagendamento imediato&#x20;**_**(2h após)**_

```
Oi, [nome_paciente]! Tudo bem?

Notamos que hoje não foi possível comparecer à sua consulta com [nome_profissional]. 

Ainda temos horários disponíveis essa semana. Gostaria de reagendar? 📅

É só nos responder ou ligar para [telefone_clinica].

[nome_clinica] — cuidando de você com carinho 💙
```

***

**✅ Exemplo 3 — Tom mais neutro&#x20;**_**(2h após)**_

```
Olá, [nome_paciente].

Sua consulta de hoje com [nome_profissional] não foi realizada.

Caso queira reagendar, entre em contato conosco:
📱 [telefone_clinica]
💬 Responda esta mensagem

Ficamos à disposição!
[nome_clinica]
```

***

**✅ Exemplo 4 — Segunda tentativa / follow-up&#x20;**_**(24h após — sem resposta)**_

```
[nome_paciente], oi!

Tentamos entrar em contato ontem porque notamos sua ausência na consulta com [nome_profissional].

Esperamos que esteja tudo bem com você! 💙

Quando quiser marcar um novo horário, é só nos chamar. Estamos aqui para cuidar de você.

[nome_clinica]
```

***

**✅ Exemplo 5 — Falta em procedimento&#x20;**_**(2h após)**_

```
Olá, [nome_paciente]!

Hoje estava reservado um horário especial para seu procedimento de *[procedimento]* com [nome_profissional], mas não conseguimos te receber.

Se aconteceu algum imprevisto, sem problemas — acontece com todo mundo! 😊

Para reagendar, entre em contato:
📱 [telefone_clinica]
💬 Responda aqui mesmo

Te esperamos! 💙
[nome_clinica]
```

***

**✅ Exemplo 6 — Falta em primeira consulta&#x20;**_**(2h após)**_

```
Oi, [nome_paciente]!

Sua primeira consulta com [nome_profissional] estava marcada para hoje, mas não foi possível realizá-la.

Queremos muito poder te atender! Quando você tiver disponibilidade, é só nos contatar para remarcar:

📱 [telefone_clinica]
💬 Ou responda aqui 😊

[nome_clinica]
```

***

### 5. Aniversário {#aniversário}

#### Objetivo

Fortalecer o relacionamento com o paciente em um momento especial — gerando afeto, lembrança de marca e, potencialmente, estimulando o retorno à clínica.

#### Cadência recomendada

| Período               | Configuração                      |
| --------------------- | --------------------------------- |
| No dia do aniversário | 1 disparo por ano, no próprio dia |

> 💡 **Dica para implantadores:** O aniversário é o único envio automático que não está vinculado a um agendamento — ele é acionado pela data de nascimento do paciente. Funciona mesmo para pacientes que não têm consulta marcada. Ótimo para reativar pacientes inativos.

#### Exemplos de Templates

**✅ Exemplo 1 — Simples e afetuoso**

```
Feliz aniversário, [nome_paciente]! 🎉🎂

Hoje é o seu dia especial e aqui na [nome_clinica] queremos te desejar muita saúde, alegria e realizações.

Que esse novo ciclo seja repleto de coisas boas! 💙

Com carinho,
[nome_clinica]
```

***

**✅ Exemplo 2 — Com CTA suave de retorno**

```
Oi, [nome_paciente]! 🎉

Hoje é seu aniversário e não poderíamos deixar essa data passar sem te dar os parabéns! 🎂

Aqui na [nome_clinica], torcemos muito pela sua saúde e bem-estar.

Que tal se presentear com uma consulta de check-up? Cuidar de si mesmo também é comemorar! 💙

Agende pelo [telefone_clinica] ou responda esta mensagem.

[nome_clinica]
```

***

**✅ Exemplo 3 — Tom mais formal e elegante**

```
[nome_paciente], nesta data tão especial, toda a equipe da [nome_clinica] deseja a você um feliz aniversário. 🎂

Que você tenha um ano com muita saúde, paz e conquistas.

Com carinho e cuidado,
[nome_clinica]
```

***

**✅ Exemplo 4 — Tom descontraído e leve**

```
🎉 Parabéns, [nome_paciente]!

Hoje é DIA DE VOCÊ! 🥳🎂

Toda a equipe da [nome_clinica] manda um abraço enorme e deseja muito:

✨ Saúde
💛 Felicidade
🌟 Realizações

Que o seu ano seja incrível!

[nome_clinica] 💙
```

***

**✅ Exemplo 5 — Clínica infantil / pediátrica**

```
Parabéns, [nome_paciente]! 🎈🎂

Hoje você está mais velho e nós estamos torcendo muito por você!

Que esse novo aninho seja cheio de saúde, brincadeiras e alegrias! 🌈

Com muito carinho,
Equipe [nome_clinica] 💙
```

***

#### Sugestão de segmentação por filtro

| Público               | Configuração                                 |
| --------------------- | -------------------------------------------- |
| Todos os pacientes    | Sem filtro (padrão)                          |
| Somente mulheres      | Gênero = Feminino                            |
| Somente homens        | Gênero = Masculino                           |
| Pacientes pediátricos | Criar envio específico com template infantil |

***

### 6. Orçamento em Aberto {#orçamento-em-aberto}

#### Objetivo

Lembrar o paciente sobre um orçamento pendente de procedimento — estimulando a decisão de aprovação sem pressão excessiva, e recuperando conversões que seriam perdidas sem acompanhamento.

#### Cadência recomendada

| Período                     | Objetivo                                                  |
| --------------------------- | --------------------------------------------------------- |
| 3 dias após a emissão       | Primeiro lembrete suave — o orçamento ainda está fresco   |
| 7 dias após (sem resposta)  | Segundo lembrete — reforça urgência com leveza            |
| 15 dias após (sem resposta) | Última tentativa — desperta curiosidade ou urgência final |

> 💡 **Dica :** Combine o filtro **Procedimento** para criar mensagens específicas por tipo de tratamento (ex.: implante, ortodontia, cirurgia, estética). Mensagens contextualizadas para o procedimento em questão têm taxa de retorno significativamente maior do que mensagens genéricas.

***

#### Exemplos de Templates

**✅ Exemplo 1 — Primeiro lembrete, tom suave&#x20;**_**(3 dias após)**_

```
Olá, [nome_paciente]!

Passando para lembrar que você possui um orçamento em aberto aqui na [nome_clinica] para *[procedimento]*. 😊

Sabemos que decisões assim merecem um tempinho para pensar. Se tiver alguma dúvida sobre o tratamento, os valores ou as condições de pagamento, estamos aqui para ajudar!

Qualquer coisa, é só responder esta mensagem ou ligar para [telefone_clinica].

[nome_clinica] 💙
```

***

**✅ Exemplo 2 — Segundo lembrete, com abertura para dúvidas&#x20;**_**(7 dias após)**_

```
Oi, [nome_paciente]!

Seu orçamento para *[procedimento]* ainda está disponível para você. 📋

Se ainda está em dúvida se é o momento certo, que tal conversar com a gente? Podemos esclarecer melhor sobre o procedimento, o processo e as formas de pagamento disponíveis.

Estamos aqui para facilitar! 💙

[telefone_clinica]
[nome_clinica]
```

***

**✅ Exemplo 3 — Terceiro contato, senso de encerramento&#x20;**_**(15 dias após)**_

```
Olá, [nome_paciente].

Sabemos que a vida é corrida e que às vezes um orçamento acaba ficando para depois. 😊

Só queremos que você saiba que seu orçamento para *[procedimento]* ainda está disponível e nossa equipe está pronta para dar início ao seu tratamento assim que você decidir.

Se precisar de qualquer informação ou quiser conversar antes de decidir, pode nos chamar à vontade.

[telefone_clinica]
[nome_clinica] 💙
```

***

**✅ Exemplo 4 — Focado em condições especiais&#x20;**_**(7 dias após)**_

```
[nome_paciente], boa tarde!

Você tem um orçamento em aberto conosco para *[procedimento]* e gostaríamos de te lembrar que trabalhamos com condições facilitadas de pagamento:

💳 Parcelamento em até [X] vezes
🤝 Negociação direta com nossa equipe

Se quiser aproveitar e garantir seu horário, é só entrar em contato:
📱 [telefone_clinica]
💬 Responda aqui

[nome_clinica] 💙
```

***

**✅ Exemplo 5 — Odontologia / Procedimento longo&#x20;**_**(3 dias após)**_

```
Oi, [nome_paciente]! 😊

Seu planejamento de tratamento para *[procedimento]* está esperando por você.

Sabemos que é uma decisão importante, e por isso nossa equipe está disponível para tirar todas as suas dúvidas antes de começar — seja sobre o procedimento em si, o tempo estimado ou as condições de pagamento.

Quando estiver pronto, é só nos sinalizar!
📱 [telefone_clinica]

[nome_clinica] 💙
```

***

#### Filtros sugeridos

| Situação                             | Filtro                                               |
| ------------------------------------ | ---------------------------------------------------- |
| Orçamentos de alto valor             | Procedimento = \[lista de procedimentos específicos] |
| Pacientes com solicitante específico | Solicitante = \[nome do médico/profissional]         |
| Por material ou tipo                 | Materiais e medicamentos = \[item]                   |

***

### Apêndice: Boas Práticas de Redação de Templates {#boas-práticas}

#### ✅ O que funciona bem

| Prática                                                    | Por quê funciona                                            |
| ---------------------------------------------------------- | ----------------------------------------------------------- |
| Usar o nome do paciente logo no início                     | Cria conexão imediata e senso de personalização             |
| Frases curtas e parágrafos pequenos                        | Mais fácil de ler em tela de celular                        |
| Emojis com moderação                                       | Tornam a mensagem mais amigável sem perder profissionalismo |
| Tom positivo mesmo em mensagens difíceis (falta, cobrança) | Mantém o paciente como aliado, não como devedor             |
| CTA claro ("responda SIM", "ligue para X")                 | O paciente sabe exatamente o que fazer                      |
| Preview das variáveis antes de ativar                      | Evita templates com variáveis vazias chegando ao paciente   |

***

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

* \[ ] O template foi aprovado no canal de WhatsApp selecionado?
* \[ ] O tom da mensagem está adequado para o tipo de envio?
* \[ ] Os períodos de disparo fazem sentido para o fluxo do paciente?
* \[ ] Os filtros aplicados segmentam corretamente o público desejado?
* \[ ] O objetivo do envio foi descrito no campo "Objetivo" para facilitar identificação futura?
* \[ ] Você verificou se já existe outro envio do mesmo tipo ativo para o mesmo público?

***

#### Estrutura-padrão de um bom template de WhatsApp

```
[Saudação + nome do paciente]

[Contexto em 1 linha — o que está acontecendo]

[Informação principal — data, hora, local, valor]

[Orientações ou próximos passos, se necessário]

[CTA claro — o que o paciente deve fazer]

[Assinatura da clínica]
```

***

_Documento elaborado para uso interno de clínicas e implantadores do Amigo Flow._ _Última atualização: Maio 2026_
