# Envios em massa

## 1. **Acesso e Visão Geral da Listagem de Campanhas**

Acesse o menu:

**Amigo Flow → Envios em Massa**

Você verá a listagem principal das campanhas, contendo:

#### Informações por campanha:

* Nome do envio
* Prévia do conteúdo
* Setor responsável
* Audiência aplicada
* Data de envio
* Status
  * **Enviado**
  * **Agendado**
  * **Rascunho**

#### Pesquisa e Filtros

* Pesquise campanhas pelo nome
* Aplique filtros para refinar a listagem (status, setor, data etc.)

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

## 2. **Criando um Envio em Massa**

Clique em **Criar Envio em Massa**.

A criação é dividida em 3 etapas principais:\
**Informações Gerais**, **Conteúdo** e **Público-Alvo**.

### 2.1 **Informações Gerais**

Aqui você configura a estrutura da campanha:

* **Nome do envio**
* **Setor responsável**

💡 _O canal corresponde ao número do WhatsApp que está selecionado no topo da página._

### 2.2 **Conteúdo do envio (obrigatório)**

Você deve selecionar **um modelo de mensagem** previamente aprovado no WhatsApp (template).

Ao selecionar:

* A prévia do template aparecerá automaticamente à direita, incluindo:
  * Cabeçalho
  * Corpo
  * Botões
  * Variáveis de preenchimento

Se nenhum modelo for selecionado, o sistema **não permite avançar**.

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

### 2.3 **Público-Alvo (obrigatório)**

Escolha a audiência:

#### Segmentações adicionais

Você pode aplicar filtros avançados, como:

* “Contatos que realizaram consulta nos últimos X dias”
* “Pacientes que possuem convênio X”

A cada filtro aplicado, o sistema atualiza em **tempo real**:

* Total de contatos atingidos

Isso evita disparos para públicos não desejados ou campanhas superdimensionadas.

{% hint style="warning" %}
Caso nenhuma segmentação seja selecionada, o público alvo é toda a base de pacientes da clínica
{% endhint %}

***

## 3. **Ações Disponíveis**

Ao finalizar as configurações, você pode:

#### **Salvar como rascunho**

Permite continuar a campanha depois sem perder informações.

#### **Agendar um envio**

Selecione:

* Data
* Turno

O sistema valida automaticamente horários e exibe feedback de sucesso após o agendamento.

#### **Envio**&#x20;

Quando enviado ou agendado com sucesso, o sistema confirma visualmente a ação.

## 4. **Visualizando os Resultados dos Envios**

Após o disparo (envio com status "Enviado") você pode clicar na campanha para abrir o painel detalhado



Ele exibirá:

#### Métricas gerais por campanha:

* **Público-alvo** (o planejado para envio incialmente)
* **Mensagens enviadas**
* **Entregues**
* **Lidas** (essa métrica depende se o usuário possui verificação de leitura no whatsapp)
* **Respondidas**

#### Lista individual dos contatos:

Com colunas para:

* Nome
* Telefone
* Data de envio
* Data de entrega
* Data de leitura
* Abertura de conversa (ícone WhatsApp verde)

É possível:

* Pesquisar contatos por nome
* Clicar no ícone de conversa para abrir o chat com o paciente no Amigo Flow

## 5.Reagendamento de campanhas

Quando uma campanha é enviada e parte das mensagens não chega ao destino, você pode reagendá-la com poucos cliques (sem reenviar para quem já recebeu).

Como funciona:&#x20;

**5.1 Acesse a listagem de campanhas**

Localize a campanha com status _Enviada_. Se o envio ficou abaixo de 80%, um alerta visual amarelo aparece na linha.

**5.2 Clique em "Reagendar"**

O botão aparece apenas quando ainda há mensagens que não foram disparadas. Se 100% dos envios foram realizados, a opção não é exibida.

**5.3 Escolha a nova data e o turno**

Defina quando a campanha deve ser reenviada. A data original é removida e a campanha passa ao status _Reagendada_.

**5.4 Somente quem não recebeu é impactado**

No reenvio, o sistema identifica automaticamente os pacientes que ainda não receberam. Quem já recebeu não é contactado novamente.

## 6. Estimativa de custo por campanha

Antes de confirmar o disparo, você vê exatamente quanto a campanha vai custar — calculado em tempo real com base no tipo de template e no público final selecionado.

Custo por tipo de template

| Categoria do template | Custo unitário    | Quando usar                                   |
| --------------------- | ----------------- | --------------------------------------------- |
| Marketing             | R$ 0,45 / contato | Promoções, campanhas de relacionamento        |
| Utilidade             | R$ 0,10 / contato | Lembretes, confirmações, avisos transacionais |

<figure><img src="../../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

O bloco exibe o breakdown completo: valor unitário × quantidade de contatos = total estimado. Atualiza automaticamente a cada mudança de filtro ou importação de lista.

**Resultado da campanha**

Após o envio, o custo estimado fica registrado nos detalhes da campanha para consulta e comparação.

#### O que acontece se eu mudar o template depois de definir o público?

O custo é recalculado automaticamente. Se você trocar de Marketing para Utilidade, o valor cai proporcionalmente sem precisar refazer nenhum passo.

#### O custo fica registrado após o envio?

Sim. O valor estimado no momento do disparo fica salvo nos detalhes da campanha para consulta posterior.

{% hint style="info" icon="lightbulb" %}
**Dica:** prefira templates de Utilidade para comunicações transacionais (lembretes de consulta, confirmações). Além de custar 78% menos por contato, eles tendem a ter taxas de entrega mais altas por serem esperados pelo paciente.
{% endhint %}
