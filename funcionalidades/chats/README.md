---
icon: messages
---

# Chats

### Visão Geral

A **Chats** do **Amigo Flow** é a central de Atendimento**s,** painel onde os atendentes da clínica gerenciam todas as conversas com pacientes em tempo real. Por meio dela, é possível visualizar, responder, transferir e finalizar atendimentos, mantendo a comunicação centralizada e organizada.

Essa funcionalidade integra mensagens vindas do **WhatsApp**, garantindo que nenhum contato fique sem resposta.

### Navegação Principal

A Central está dividida em **três áreas principais**:

1. **Menu lateral esquerdo (Atendentes e Filtros)**
2. **Lista de conversas (Chats)**
3. **Janela de conversa (Histórico e Interação)**

#### 1. Menu Lateral Esquerd&#x6F;**(Atendentes e Filtros)**

**Seções**

* **Meus Chats:** exibe apenas os atendimentos atribuídos ao usuário logado.
* **Em Aguardando:** mostra conversas que foram transbordadas para atendimento humano e no momento ainda não estão atribuídas a nenhum atendente.
* **Todos:** lista todos os atendimentos ativos na clínica.

**Outros Atendentes**

Nesta seção é possível visualizar todos os atendentes conectados do mesmo setor, junto com o número de conversas em andamento de cada um. Isso permite acompanhar a carga de trabalho e facilitar transferências.

#### 2. Lista de Conversas

Nesta área, o atendente vê uma prévia das conversas. Cada item da lista mostra:

* Foto e nome do paciente
* Trecho da última mensagem
* Horário da última interação
* Indicador azul 🔵 para mensagens não lidas

**Busca e Filtros**

Na parte superior, é possível **buscar pelo nome do paciente ou número de telefone.** Os resultados são atualizados em tempo real.

#### 3. Janela de Conversa

Ao clicar em um chat, o histórico completo da conversa é exibido à direita.

**Campo de Mensagem**

O atendente pode:

* Digitar mensagens manuais
* Enviar áudio
* Enviar emojis 😄
* Anexar arquivos (como PDFs, imagens ou documentos médicos)
* Utilizar **atalhos rápidos** pré-configurados (modelos de mensagem)
* Utilizar **templates de mensagens** (Se API Oficial)
* **Edição e exclusão de conversa:** O usuário só poderá editar e excluir mensagens em até 10 min após o envio. E ele só poderá excluir conversas que forem enviadas por ele e pelo agente.

### Funções Principais

#### Transferir Atendimento

O botão **“Transferir”** permite enviar a conversa para outro atendente ou setor. Ao transferir:

* O histórico é mantido.
* O novo atendente recebe a conversa em tempo real.
* O paciente não percebe a troca de operador (garantindo continuidade).
* Os logs de interações ficam registrados na conversa

#### Finalizar Atendimento

Ao encerrar o contato, clique em **“Finalizar”**. Isso:

* Remove a conversa da lista ativa.
* Arquiva o histórico para consultas futuras.
* Libera o atendente para novos atendimentos.
* Pode-se enviar uma mensagem de avaliação após a finalização caso o envio esteja ativo (em desenvolvimento)

#### Indicação de Paciente

No topo do chat:

* Exibe o **nome do paciente** e o **status “Online”**.
* Mostra a etiqueta **“Paciente”** se o contato estiver vinculado a um cadastro do prontuário no Amigo Clinic. Caso não haja esse vinculo o a etiqueta exibida será **"Lead"**, e caso se trate de um cadastro duplicado virá a etiqueta **"Paciente duplicado”**

Isso ajuda a identificar rapidamente quem já é paciente da clínica e quem é um novo contato.

#### Agente Flow (IA)

Quando a inteligência artificial estiver ativa:

* Os atendimentos automáticos são mostrados sob o atendente “Agente Flow”.
* O número ao lado do nome do agente no menu lateral indica quantas conversas a IA está conduzindo.
* O atendente pode **intervir manualmente**, **assumindo** um chat automatizado quando necessário.

#### Nova Conversa

Clínica pode buscar por contatos (Pacientes e leads) **pelo nome contato ou número de telefone,** e iniciar uma nova conversa com aquele contato.

* Quando o número for API oficial, para realizar essa ação a clínica deverá selecionar um template de mensagem predefinido previamente (caso o contato esteja fora da janela de atendimento).

#### **Histórico**

Um atendimento consta como um conjunto de conversas entre um atendente (ou agente) e um terceiro (Engloba tudo entre o momento que a conversa foi aberta/ deu início até o momento que ela foi finalizada pelo atendente ou transferida para outro).

* Para todo atendimento é gerado um resumo feito pela IA para facilitar a contextualização da clínica

### Casos de Uso Práticos

| Cenário                             | Ação do Atendente                                            | Resultado Esperado                                  |
| ----------------------------------- | ------------------------------------------------------------ | --------------------------------------------------- |
| Novo paciente envia mensagem        | A conversa aparece em “Em Aguardando”                        | O atendente pode assumir e responder                |
| O paciente pede algo de outro setor | Atendente clica em “Transferir” e escolhe o novo responsável | O outro atendente recebe a conversa automaticamente |
| Finalização de consulta ou dúvida   | Clica em “Finalizar”                                         | O chat sai da lista e fica arquivado                |
| Busca por paciente específico       | Usa o campo de busca por nome ou número                      | A lista mostra apenas as conversas relacionadas     |
| Atendimento via IA                  | O Agente Flow responde automaticamente                       | O atendente pode monitorar ou intervir              |

### Boas Práticas

* Sempre **finalize os chats** concluídos para manter a central organizada.
* Use **atalhos** para respostas frequentes e ganhar agilidade.
* Transfira apenas quando necessário — evite quebrar o fluxo da conversa.
* Acompanhe os **indicadores de status (online, lida, não lida)** para evitar falhas de comunicação.
