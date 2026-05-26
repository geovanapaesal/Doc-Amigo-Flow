---
icon: whatsapp
---

# Como funciona a janela de conversa da Meta?

Toda conversa feita pelo WhatsApp Business (API oficial da Meta, usada pelo Amigo Flow) acontece dentro de **janelas de 24 horas**.\
Essas janelas determinam **quando a clínica pode enviar mensagens ao paciente** e **quando um novo atendimento será contabilizado.**

#### Quando o paciente envia a mensagem primeiro

Chamamos isso de **conversa reativa.**

* Assim que o paciente manda uma mensagem, **abre-se uma janela de 24 horas**.
* Durante esse período, o agente Flow, a recepcionista ou qualquer automação podem responder livremente, **sem precisar enviar um modelo de mensagens.**
* Se a clínica responder **depois das 24h**, será necessário **enviar um modelo de mensagem aprovado pela Meta** (template) — e isso conta como **novo atendimento.**

#### Quando a clínica envia a mensagem primeiro

Chamamos isso de **conversa proativa.**

* A clínica inicia o contato com o paciente enviando um **modelo de mensagem aprovado pela Meta** (exemplo: lembrete de consulta, mensagem de reagendamento, retorno de exame etc.) - isso conta como **novo atendimento.**
* Se o paciente responder a essa mensagem, **abre uma nova janela de 24 horas** a partir do momento do envio.
* Todas as mensagens trocadas dentro dessa janela são consideradas **parte do mesmo atendimento.**

#### 🔁 Renovação da janela

* Cada vez que uma nova mensagem **modelo** é enviada **fora da janela (sem o paciente responder)**, **um novo atendimento é contabilizado**.
* Mensagens de utilidade enviadas dentro da janela aberta não contam como atendimentos.
* Se o usuário **não tiver respondido** ao modelo de **utilidade ou marketing**, você **não poderá** enviar mensagens livres depois, pois a regra da Meta exige que a interação esteja dentro da **janela de 24 horas** a partir da última mensagem do usuário.

#### O que fazer nesse caso?

1. **Aguardar uma resposta** do paciente para poder continuar a conversa com mensagens livres.
2. **Enviar um novo template de mensagem** aprovado pela Meta para reabrir a conversa, se necessário. → criar um modelo padrão para quando o usuário não responder, poder enviar outro (de preferencia com um tom mais humano e personalizado) -> **um novo atendimento é contabilizado**. Caso tenha excedido o limite de modelos de markentig por atendimento, precisará finalizar o atendimento atual e iniciar um novo (para poder enviar outro modelo).

#### Resumo prático para a clínica

| Situação                            | O que acontece                      | Conta como novo atendimento? |
| ----------------------------------- | ----------------------------------- | ---------------------------- |
| Paciente envia mensagem             | Abre janela de 24h.                 | ✅ Sim                        |
| Clínica responde dentro de 24h      | Continua o mesmo atendimento        | ❌ Não                        |
| Clínica responde após 24h           | Precisa de modelo Meta              | ✅ Sim                        |
| Clínica inicia conversa (proativa)  | Abre nova janela de 24h             | ✅ Sim                        |
| Novo disparo automático ou em massa | Cada envio conta como 1 atendimento | ✅ Sim                        |

#### **Categorias de Modelos de mensagens**

As mensagens são classificadas em duas categorias: "conversas iniciadas pela empresa" e "conversas iniciadas pelo usuário". As mensagens iniciadas pela empresa podem ser de duas categorias distintas:

1. **Mensagens de Utilidade**: Informam sobre transações anteriores, como status de pedidos, entregas ou cobranças regulares.
2. **Mensagens de Marketing**: Destinadas a promoções, ofertas, novidades da marca ou recuperação de carrinhos abandonados.

####



