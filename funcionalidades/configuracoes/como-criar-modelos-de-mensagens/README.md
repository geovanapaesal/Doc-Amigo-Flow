# Como criar modelos de mensagens

Criar e utilizar modelos de mensagem no **Amigo Flow** é essencial para padronizar a comunicação da clínica com pacientes via WhatsApp Oficial (API da Meta).

Os modelos podem ser utilizados em:

* Confirmações de consulta
* Lembretes automáticos
* Mensagens pré e pós-atendimento
* Envio de documentos
* Orçamentos em aberto
* Campanhas informativas
* Comunicados operacionais

Isso garante uma comunicação mais profissional, consistente e automatizada.



### Passo 1: Acessar o canal com um número conectado

1. No menu Número e conta, acesse **Modelos da conta**.
2. Clique em **Criar Modelo** e selecione a categoria desejada.

<figure><img src="../../../.gitbook/assets/Captura de Tela 2026-02-24 às 16.15.30.png" alt=""><figcaption></figcaption></figure>



As categorias seguem a classificação da Meta:

* **Marketing** → Promoções, campanhas, divulgação de serviços.
* **Atendimento (Utilidade)** → Confirmações, lembetes, notificações operacionais.

### Passo 2: Preencher as informações do modelo

#### Nome do Modelo

Escolha um nome claro e objetivo.

Exemplos:

* Confirmação de Consulta
* Lembrete 24h
* Orçamento em Aberto
* Boas-vindas Paciente Novo

#### 📝 Conteúdo

**Cabeçalho (Opcional):**&#x20;

É possível escolher inserir um cabeçalho, podendo este conter uma mídia (vídeo, imagem, doc, aúdio) ou não.

**Corpo da Mensagem**

Digite o texto que será enviado ao paciente.

É possível usar **variáveis do Amigo Clinic** ou **variáveis dinâmicas** para personalizar automaticamente a mensagem.

Exemplo:

{% code overflow="wrap" %}
```
Olá @@@nome, sua consulta com @@@medico está confirmada para @@data às @@horario.
```
{% endcode %}

As variáveis do Clinic disponíveis aparecem embaixo do editor e podem ser inseridas com um clique.

As variáveis dinâmicas precisam ser substituídas no momento do envio.

Além disso, é possível ver uma preview do modelo que está sendo criado na lateral do formulário.<br>

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

#### 🔘 Botões (opcional)

Você pode adicionar botões interativos:

**1. Resposta Rápida**\
Permite que o paciente responda com um clique.\
Exemplo:

* Confirmar presença
* Reagendar
* Falar com atendente

**2. Abrir Página (Call to Action)**\
Direciona para um link externo.\
Exemplo:

* Acessar mapa da clínica
* Assinar documento

<figure><img src="../../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

### Passo 3: Enviar para aprovação

Clique em **Validar modelo** e o modelo será enviado automaticamente para análise da **Meta**.

### Passo 4: Acompanhar o status

Você pode acompanhar o status diretamente na listagem de modelos:

* 🟡 Em Análise
* 🟢 Aprovado (Ativo)
* 🔴 Reprovado

Se for reprovado, o motivo será exibido. Basta ajustar e reenviar.

## Considerações Importantes

#### ⏳ Tempo de aprovação

O prazo é definido exclusivamente pela Meta.

Contas mais novas ou com pouco histórico de envio podem ter aprovação mais demorada.

#### 💰 Custos

Envios de mensagens fora da janela de 24h são cobrados como um atendimento.

#### 🔎 Boas práticas para aprovação

* Não utilizar linguagem sensível ou promessas médicas.
* Evitar excesso de emojis.
* Não usar caixa alta excessiva.
* Garantir clareza e objetividade.
* Evitar termos promocionais agressivos em categoria errada.

#### 📏 Limite de caracteres

O limite por modelo é de **1024 caracteres**.

## Dica:

No contexto clínico, os modelos mais relevantes normalmente são:

* Confirmação automática
* Lembrete 24h
* Pós-consulta
* Orçamento em aberto
* Solicitação de documentos
* Retorno médico

Modelos bem estruturados reduzem no-show, aumentam taxa de conversão de orçamento e aliviam a recepção.\
Modelo mal configurado? Pode gerar bloqueio de número.
