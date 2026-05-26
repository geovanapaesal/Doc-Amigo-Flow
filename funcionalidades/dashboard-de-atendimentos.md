---
icon: chart-line
---

# Dashboard de atendimentos

### Visão Geral

O **Dashboard de Atendimentos** é o painel de análise do **Amigo Flow**, onde gestores e atendentes podem acompanhar em tempo real o desempenho do agente de IA e da equipe humana.

Essa tela reúne **indicadores operacionais e de qualidade**, oferecendo uma visão completa da produtividade da clínica e da eficiência da automação nas conversas com pacientes.

### Acesso

A funcionalidade pode ser acessada pelo menu superior do sistema, na aba **“Dashboard”** dentro do módulo **Amigo Flow**.

### Estrutura do Dashboard

O Dashboard é dividido em **três seções principais**:

1. **Em tempo real**
2. **Histórico e Indicadores de desempenho**
3. **Métricas de disparos automáticos**

#### 1. Em Tempo Real

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

Nesta área, o usuário acompanha o **status atual dos atendimentos**, divididos por categoria:

| Categoria                  | Descrição                                                                                                                     |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **Em aguardando**          | Conversas novas que foram transbordadas para atendimento humano pelo agente e ainda não foram assumidas por nenhum atendente. |
| **Com o Agente (IA)**      | Conversas que estão sendo conduzidas pelo Agente Flow.                                                                        |
| **Com atendentes humanos** | Conversas que estão em andamento com um atendente da equipe.                                                                  |

Cada linha exibe:

* **Nome do paciente**
* **Tempo de espera ou duração da conversa**
* **Resumo da solicitação**
* **Ícone de WhatsApp** para acesso direto à conversa

> 🔁 Os dados são atualizados automaticamente a cada poucos minutos.\
> O horário da última atualização é exibido no canto superior direito.

#### 2. Atendimentos Concluídos

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

Essa área apresenta um **resumo estatístico** dos atendimentos em determinado período.\
É possível selecionar:

* **Últimos 7 dias**
* **Últimos 15 dias**
* **Período personalizado**

**Principais Indicadores**

| Indicador                                     | Descrição                                                                     |
| --------------------------------------------- | ----------------------------------------------------------------------------- |
| **Total de conversas**                        | Número total de atendimentos realizados no período.                           |
| **Tempo médio de resolução**                  | Tempo médio para concluir um atendimento, desde o início até o encerramento.  |
| **Taxa de transferência**                     | Percentual de conversas que precisaram ser transferidas para outro atendente. |
| **Resolvidas pelo Agente**                    | Percentual de conversas que foram concluídas pela IA sem intervenção humana.  |
| **Agendadas pelo Agente**                     | Quantidade de consultas marcadas automaticamente pelo Agente Flow.            |
| **Leads convertidos pelo Agente**             | Número de novos pacientes agendados a partir de interações com o agente.      |
| **Iniciadas por leads / pacientes / clínica** | Origem dos atendimentos (quem iniciou a conversa).                            |

Esses dados ajudam o gestor a identificar:

* A **eficiência da automação**,
* O **tempo médio de resposta**, e
* O **nível de engajamento** dos pacientes.

#### Avaliação de Atendimento

Exibe o **índice de satisfação dos pacientes**, com base nas avaliações pós-atendimento.

* **Respostas:** número total de avaliações recebidas no período.
* **Média geral:** nota média de satisfação (escala de 1 a 5).
* **Ranking por  tipo de atendente:** mostra a pontuação média da equipe e do Agente Flow.

> 💡 O Agente Flow também é avaliado, permitindo medir a aceitação e qualidade do atendimento automatizado.

#### 3. Disparos automáticos

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

Na parte inferior do Dashboard, o módulo de Disparos automáticos resume o progresso das disparos de confirmações de consultas e reagendamento após faltas realizadas pelo agente.

**Exibe:**

* **Gráfico de progresso:** percentual de confirmações/reagendamentos concluídos.
* **Lista detalhada:** cada confirmação com:
  * Nome do paciente
  * Telefone
  * Procedimento
  * Status atual (Confirmado, Pendente, etc.)

**Indicadores:**

* **Total de confirmações/reagendamentos no período**
* **Percentual de sucesso dos disparos automáticos**

> Permite identificar se o volume de confirmações automáticas está coerente com a agenda da clínica e se há necessidade de reforço humano.

### Casos de Uso

| Cenário                                                          | Ação do Usuário                                                      | Resultado Esperado                                           |
| ---------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------ |
| O gestor quer saber quantas conversas o agente finalizou sozinho | Acessa o painel e observa o indicador “Resolvidas pelo Agente”       | Percentual de atendimentos automatizados é exibido           |
| A clínica deseja saber o tempo médio de atendimento humano       | Consulta o card “Tempo médio de resolução”                           | O tempo médio é mostrado em horas e minutos                  |
| O atendente quer saber sua própria nota de atendimento           | Observa o ranking de avaliação                                       | Sua pontuação aparece individualmente                        |
| O gestor quer comparar desempenho entre IA e humanos             | Analisa os indicadores “Agendadas pelo Agente” e “Leads convertidos” | Permite ver o impacto da automação nos resultados da clínica |

### Benefícios

* **Gestão inteligente** de atendimentos com base em dados reais.
* **Medição de performance da IA e da equipe humana.**
* **Tomada de decisão rápida**, com visibilidade de gargalos e oportunidades.
* **Acompanhamento em tempo real** do volume de atendimentos e tempo médio de resposta.

### Boas Práticas

* Verifique o painel **diariamente**, especialmente o status _“Em aguardando”_, para evitar atrasos e demoras no atendimento.
* Use filtros de **período personalizado** para comparar desempenho entre semanas ou campanhas.
* Observe a **taxa de transferência**: índices altos podem indicar necessidade de requalificação da IA ou da equipe.
* Analise as **avaliações de atendimento** para reconhecer bons resultados e ajustar pontos de melhoria.

### Suporte e Dúvidas

Se os dados do painel não atualizarem corretamente ou algum indicador exibir valores inconsistentes:

1. Recarregue a página.
2. Verifique o horário da última atualização.
3. Caso o problema persista, contate o **Suporte Amigo**
