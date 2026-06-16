# Lançamentos de junho

### 1. Base de Orientações

A Base de Orientações é uma funcionalidade do Agente Flow que permite à clínica cadastrar textos aprovados para situações clínicas recorrentes — como cuidados pós-procedimento, preparo para exames ou sintomas esperados — e fazer com que o agente os envie automaticamente ao paciente no momento certo.

O agente identifica, via correspondência semântica, quando a mensagem do paciente se encaixa no contexto de uma orientação cadastrada e, se a confiança for suficiente, envia o texto exatamente como foi cadastrado pela clínica.

[Veja aqui como cadastrar orientações e como funciona a fundo](../../funcionalidades/configuracoes/orientacoes-medicas.md)



### 2. Controle de Atendimento de Contatos pelo Agente

#### O que é

Contatos são pessoas que entram em contato com a clínica via WhatsApp, mas não estão cadastradas como pacientes no sistema. Esta funcionalidade permite configurar se o Agente Flow deve atender ou não esse perfil de contato.

#### Como configurar

1. Acesse **Agente Flow → Configurações → Habilidades do Agente**.
2. Localize a opção **Atendimento de Contatos**.
3. Escolha o comportamento desejado:
   * **Habilitado:** o agente recebe e conduz o atendimento do Contato normalmente.
   * **Desabilitado:** o agente transfere o atendimento para o setor principal da clínica assim que identifica que o remetente é um Contato (não-paciente).

#### Quando usar cada configuração

| Cenário                                                                                                 | Configuração recomendada |
| ------------------------------------------------------------------------------------------------------- | ------------------------ |
| Clínica quer que o agente atenda contatos                                                               | Habilitado               |
| Clínica prefere que contatos sejam atendidos por humanos e não consumam atendimento (quando receptivos) | Desabilitado             |

