---
icon: robot
---

# Novo modo de agendamento via link

**O que há de novo**

A habilidade de agendamento do Amigo Flow agora suporta três modos de operação distintos. As clínicas escolhem como o agente se comporta quando um paciente solicita um agendamento,  e a configuração reflete esse comportamento de forma consistente em toda a experiência.

**Os três modos:**

**1. Conversa com o Agente Flow** _(comportamento anterior, inalterado)_ O agente conduz o fluxo completo de agendamento dentro da conversa.

**2. Envio de link de agendamento:**  O agente detecta a intenção de agendar e encaminha o paciente para o link oficial de autoagendamento da clínica (o Agende.ai). Ao ativar esse modo, o fluxo nativo de agendamento é automaticamente desativado. A aba de configuração da habilidade passa a exibir apenas as regras de atendimento, sem os campos de agenda. O agente não lista horários e não sugere disponibilidade: apenas filtra a intenção e entrega o link.

**3. Agendamento desligado** _(sem link configurado + habilidade inativa):_ Quando não há link configurado e a habilidade está inativa, o agente transfere o atendimento para um humano automaticamente. Sem mensagens intermediárias, sem explicações.

**Lógica de fallback**

| Cenário                                      | Comportamento do agente                          |
| -------------------------------------------- | ------------------------------------------------ |
| Modo "link" ativo + link configurado         | Envia o link ao detectar intenção de agendamento |
| Modo "link" ativo + link **não** configurado | Transfere para atendente humano                  |
| Habilidade inativa + sem link                | Transfere para atendente humano                  |
| Modo "agente" ativo                          | Fluxo nativo padrão                              |

**Como configurar**

1. Acessar configurações gerais do Amigo Flow
2. Inserir o link de agendamento em **Configurações → Agendamento Online**
3. Acessar **Habilidades → Agendamento**
4. Selecionar a opção desejada: _"Conversa com o Agente Flow"_ ou _"Envio de link de agendamento"_

> Ao selecionar o modo de link, a habilidade de agendamento nativo é desativada automaticamente e a interface de configuração simplifica para exibir apenas as regras de atendimento.

<figure><img src="../../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>

* Clínicas que já usam o fluxo nativo **não são afetadas,** nenhuma mudança sem configuração ativa
* O modo "link" é especialmente relevante para clínicas que já têm sistema próprio de autoagendamento e usavam o Amigo Flow como triagem
* Se uma clínica ativar o modo "link" sem configurar a URL, o agente transfere para humano ( deve configurar o link antes de ativar)

