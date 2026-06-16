# Orientações médicas

A Base de Orientações é uma funcionalidade do Agente Flow que permite à clínica cadastrar textos aprovados para situações clínicas recorrentes, como: cuidados pós-procedimento, preparo para exames ou sintomas esperados; e fazer com que o agente os envie ao paciente no momento certo.

O agente identifica, via correspondência semântica, quando a mensagem do paciente se encaixa no contexto de uma orientação cadastrada e, se a confiança for suficiente, envia o texto exatamente como foi cadastrado pela clínica.

#### Como cadastrar uma orientação

1. Acesse **Agente Flow → Configurações → Base de Orientações**.
2. Clique em **Nova Orientação**.
3. Preencha os campos:
   * **Nome:** identificação interna da orientação (ex: "Cuidados pós-botox").
   * **Contexto de uso:** descreva em linguagem natural quando essa orientação deve ser acionada (ex: "quando o paciente relatar dor ou inchaço após aplicação de botox").
   * **Texto da orientação:** o conteúdo que será enviado ao paciente, exatamente como escrito.
   * **Arquivo de mídia (opcional):** imagem, PDF ou áudio complementar.
4. Clique em **Salvar**.

> ⚠️ O texto da orientação é enviado ao paciente **sem qualquer alteração** pelo agente. Revise o conteúdo antes de salvar.

#### Importação em lote

Em breve.

#### Como o agente decide o que fazer

Quando o agente classifica a mensagem do paciente como uma dúvida clínica ou de procedimento, ele aciona o pipeline de matching da Base de Orientações Médicas. O resultado segue três zonas de confiança:

| Nível de confiança | Ação do agente                                                                                                                                           |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Alta**           | Envia o texto da orientação diretamente                                                                                                                  |
| **Média**          | Envia a orientação com um aviso de segurança: "Encontrei esta orientação da clínica, mas se tiver dúvidas, posso encaminhá-la para o setor responsável." |
| **Baixa**          | Não envia orientação. Transfere o atendimento para um humano.                                                                                            |

Qualquer falha técnica no processo (timeout, erro de API) também resulta em transferência para humano, o agente nunca envia uma orientação sem validação.

#### Identificação nas mensagens

Quando o agente envia uma orientação, a mensagem exibe uma indicação de que o conteúdo veio da **Base de Orientações Médicas da clínica**, garantindo transparência para a clínica.



