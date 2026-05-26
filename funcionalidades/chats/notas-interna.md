---
icon: notes-sticky
---

# Notas interna

### O que são Notas Internas?

Notas Internas são mensagens visíveis apenas para os usuários do Amigo Flow que têm acesso ao atendimento. Elas ficam registradas no histórico da conversa, identificadas visualmente com destaque em **amarelo**, e nunca chegam ao cliente nem são enviadas para canais externos.

Você pode usar notas para:

* Repassar contexto para um colega que vai assumir o atendimento
* Registrar observações importantes sobre o caso
* Coordenar internamente sem interromper o fluxo da conversa com o cliente

### Como usar

#### Alternar entre Responder e Nota

Dentro de qualquer atendimento ativo, o campo de texto tem duas opções: **Responder** (padrão) e **Nota**.

* **Responder** — a mensagem vai para o cliente normalmente
* **Nota** — a mensagem vira uma nota interna, visível apenas para a equipe

> ⚠️ Ao trocar de modo, tudo que estiver digitado no campo é apagado automaticamente, sem confirmação. Certifique-se de que não há conteúdo importante antes de alternar.

Ao ativar o modo Nota, o campo fica com destaque amarelo e exibe o aviso: **"O que for digitado aqui não será visível ao cliente."**

#### O que você pode fazer em uma nota

* Enviar texto
* Adicionar emojis
* Anexar arquivos
* Enviar áudios
* Responder (reply) a uma nota existente

#### Excluir uma nota

Você pode excluir apenas as suas próprias notas. Não há exceção para perfis administradores — ninguém pode excluir a nota de outra pessoa.

Ao excluir uma nota:

* O balão permanece na conversa com o texto **"Mensagem excluída"**
* Se a nota tinha um reply, o conteúdo da nota excluída continua aparecendo na área de reply

> Notas **não podem ser editadas** após o envio.

#### Responder (reply) a uma nota

É possível fazer reply em qualquer nota. Ao responder, quem é responsável pelo atendimento pode escolher entre enviar como **Nota** ou como **Resposta ao cliente**.

O reply não gera notificação automática para quem escreveu a nota original.

### Notas em atendimentos que não são seus

Mesmo que você não seja o responsável pelo atendimento, você pode:

* Visualizar todas as mensagens e notas
* Adicionar notas internas sem precisar assumir o atendimento

Para enviar uma resposta ao cliente, é necessário assumir o atendimento primeiro — essa regra já existia e não muda com as notas.

### Notas no Histórico

Ao acessar um atendimento já finalizado pelo Histórico, você pode **visualizar** todas as notas que foram criadas durante o atendimento. Não é possível criar, editar ou excluir notas em atendimentos finalizados.

As notas no histórico são apenas para consulta — não reabrem o atendimento, não alteram o status e não afetam métricas.

***

### Notas criadas pelo Agente Flow

Quando o **Agente Flow** transfere um atendimento para um atendente humano, ele cria automaticamente uma nota no momento exato da transferência. Essa nota traz o contexto do que foi tratado no atendimento automatizado, para que o atendente assuma já com as informações necessárias — sem precisar reler toda a conversa.

Essas notas têm identificação visual distinta, com a origem **"Agente Flow"**, e se diferenciam claramente das notas criadas por humanos.

**Regras das notas do Agente Flow:**

* São criadas automaticamente no momento do handoff (transferência para atendimento humano)
* Exibem a data e hora de criação normalmente
* **Não podem ser editadas nem excluídas** por nenhum usuário, incluindo administradores
* Não exibem os controles de editar/excluir na interface
* O conteúdo é configurado diretamente no nó de transferência do Agente Flow, com suporte a variáveis dinâmicas (ex: nome do paciente, motivo do contato, última intenção detectada)
* Se nenhum conteúdo for configurado no nó, a nota exibe a mensagem padrão: **"Atendimento transferido pelo Agente Flow."**

### O que as Notas Internas não fazem

| O que não acontece                         | Detalhe                                                |
| ------------------------------------------ | ------------------------------------------------------ |
| O cliente não vê as notas                  | Notas são estritamente internas                        |
| Notas não são enviadas para a Docana       | Nem durante o atendimento, nem no resumo               |
| Notas não afetam métricas                  | Não alteram status, SLA nem indicadores do atendimento |
| Notas não reabrem atendimentos finalizados | Apenas visualização no histórico                       |

### Perguntas frequentes

**Posso criar uma nota em um atendimento que não é meu?** Sim. Você pode adicionar notas em qualquer atendimento que consiga visualizar, sem precisar assumir a responsabilidade.

**O que acontece com uma nota que eu excluí?** O balão permanece no chat com o texto "Mensagem excluída". Se havia um reply nessa nota, o conteúdo dela continua sendo exibido na área de reply.

**Posso editar uma nota depois de enviada?** Não. Notas não podem ser editadas após o envio.

**Um administrador pode excluir a nota de outro usuário?** Não. Cada usuário só pode excluir as próprias notas. Não há exceção por perfil.

**As notas do Agente Flow podem ser removidas?** Não. Essas notas são imutáveis e não podem ser editadas nem excluídas por nenhum usuário ou perfil.

**As notas aparecem para o cliente de alguma forma?** Não. Notas nunca são exibidas ao cliente nem enviadas para nenhum canal externo.
