---
icon: chart-line
---

# Dashboard de atendimentos

### Visão Geral

O **Dashboard de Atendimentos** é o painel de análise do **Amigo Flow**, onde gestores e atendentes podem acompanhar em tempo real o desempenho do agente de IA e da equipe humana.

Essa tela reúne **indicadores operacionais e de qualidade**, oferecendo uma visão completa da produtividade da clínica e da eficiência da automação nas conversas com pacientes.

### Acesso

A funcionalidade pode ser acessada pelo menu superior do sistema, na aba **“Dashboard”** dentro do módulo **Amigo Flow**.

{% embed url="https://drive.google.com/file/d/1j9fX7kI3YEmCPA-qoepAUYsSvdy78VeA/view?usp=drive_link" %}

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

**Principais Indicadores:**\
Acompanhe os principais resultados do Agente Flow no período selecionado:

* Receita gerada.
* Tempo médio até a primeira resposta.
* Tempo médio de resolução.
* Qualidade do atendimento.
* Agendamentos, confirmações de presença e leads convertidos.

Você também pode consultar os **Motivos de transferência**, organizados por volume de ocorrências, para identificar os temas que mais levam um atendimento à equipe humana.

### Capacidade da operação <a href="#id-90e70165-a6f1-4b70-8725-3120e633a1b5" id="id-90e70165-a6f1-4b70-8725-3120e633a1b5"></a>

Veja como os atendimentos foram distribuídos e concluídos:

* Total de atendimentos finalizados.
* Percentual resolvido pelo Agente Flow.
* Percentual transferido para atendentes.
* Percentual finalizado por inatividade.
* Tempo médio em aguardo e tempo médio de atendimento.

A visualização de **Origem dos atendimentos** separa os dados entre pacientes, leads e clínica. A análise por **Setor** permite comparar o volume de atendimentos e o tempo em aguardo em cada área.

### Qualidade da operação <a href="#id-1370562a-295e-4817-addc-4196927c7446" id="id-1370562a-295e-4817-addc-4196927c7446"></a>

Acompanhe a qualidade dos atendimentos com:

* Nota geral e distribuição das avaliações recebidas.
* Ranking de atendentes.
* **Qualidade por tema**, com ocorrências, percentual resolvido pelo Agente Flow e avaliação.
* **Qualidade por atendente**, com busca e dados de atendimentos, tempo médio de primeira resposta, tempo médio de resolução e avaliação.

### Filtros e disponibilidade dos dados <a href="#b99387ef-2168-47a7-bed8-4662ae8bddde" id="b99387ef-2168-47a7-bed8-4662ae8bddde"></a>

Use os filtros de período, clínica, canal e setor quando eles estiverem disponíveis para o tipo de análise. Os blocos são atualizados de acordo com o recorte escolhido.

Quando não houver dados para um período ou filtro, o dashboard indica que não há informações disponíveis. Caso apenas parte dos dados esteja disponível, os demais indicadores continuam sendo exibidos.

Esses dados ajudam o gestor a identificar:

* A **eficiência da automação**,
* O **tempo médio de resposta**, e
* O **nível de engajamento** dos pacientes.



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
