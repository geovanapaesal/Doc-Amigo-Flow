# Canais

Os **canais** representam os diferentes meios de comunicação da clínica (ex: contato com a Recepção, contato com a Comercial, contato da Unidade A, contato da Unidade B).

Cada canal concentra:

* Número e conta
* Regras de atendimento
* Envios automáticos
* Modelos
* Agente (opcional)

#### Como funciona:

* Cada canal deve ter:
  * **Nome do canal** (obrigatório)
  * **Setor principal** associado (obrigatório)
* Após criado:
  * O canal aparece imediatamente na listagem
  * Já fica disponível para configuração

***

### 📱 Número e Conta&#x20;

A aba **Número e Conta** passa a ser o primeiro passo operacional do canal.

#### Associando um número

* O fluxo segue o **de associação atual da Meta**
* Enquanto o número estiver em processo de associação:
  * Os **status das etapas** (validação da empresa, ativação da conta, etc.) ficam visíveis nessa aba
  * O cliente acompanha claramente em que fase está

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

#### Após a associação

Com o número associado, o canal passa a permitir:

* Visualização/configuração do **perfil do número**
* **Envios Automáticos**
* **Modelos de Mensagem**

***

### 🤖 Agente Flow

O agente ao invés de ser o ponto de partida, passa a ser um **componente do canal**. Ele é **opcional** dentro do canal.

#### Configurações disponíveis:

* Base de conhecimento
* Habilidades
* Regras de inatividade

#### Habilidades do agente:

* Agendamento
* Reagendamento
* Confirmação de presença
* Atendimento de leads

#### Regras de inatividade:

* Reengajamento automático
* Mensagem de finalização ou transferência

***

### 🗣️ Regras de Atendimento&#x20;

Dentro das regras de atendimento do canal, é possível configurar:

* **Setores associados ao canal**
* **Horário de atendimento do canal**
* **Mensagem de saudação**
* **Ativação da avaliação de atendimento**

#### **1. Setores associados ao canal**

* Associe os setores que terão acesso ao canal e defina regras para que o agente trie corretamente as conversas para o respectivo setor.
* Além disso, é possível também escolher ou trocar o setor principal do canal.

#### 2. **Horário de atendimento do canal**

Configure o horário **de atendimento** da sua clínica:

* De **segunda a domingo**, com configuração individual por dia.
* Intervalo diário no formato **24 horas** (ex: 08:00 - 18:00).
* **Atenção:** o sistema aceita **apenas um intervalo contínuo por dia**.
  * Não há suporte para múltiplos períodos (ex: manhã e tarde separados).
* Se o paciente tentar falar com um atendente ou o agente transferir para atendimento humano **fora do horário configurado**:
  * Ele será informado sobre os horários disponíveis.
  * A conversa ficará com o status **“Em aguardo”** até o próximo período ativo.
  * Conversas “Em aguardo” **não são encerradas por inatividade**.

#### **3. Mensagem de saudação**

Escolha uma mensagem de saudação para ser enviada sempre que os pacientes entrarem em contato com a sua Clínica.

**Obs:** Caso o **Agente esteja ativo**, ele se baseia nessa mensagem para saudar o paciente.

#### **4. Ativação da avaliação de atendimento**

Ative e Configure a avaliação de atendimento para a sua clínica, que será enviada ao finalizar os atendimentos.

{% content-ref url="avaliacao-de-atendimento.md" %}
[avaliacao-de-atendimento.md](avaliacao-de-atendimento.md)
{% endcontent-ref %}
