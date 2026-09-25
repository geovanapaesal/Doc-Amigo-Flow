---
description: >-
  Monte o caminho que cada conversa percorre no WhatsApp da sua clínica, da
  saudação ao agendamento.
---

# Agente Classic

## Fluxos de atendimento

Os **Fluxos** são roteiros automáticos que conduzem a conversa com o paciente assim que ele chama sua clínica. Você desenha o caminho em uma tela visual, passo a passo: o que o bot diz, quais opções o paciente vê, quando o agente de IA assume o agendamento e em que momento a conversa vai para a sua equipe.

**Com um fluxo, você pode:**

* Receber o paciente com uma saudação padronizada, 24 horas por dia.
* Direcionar cada assunto para o lugar certo: agendamento, dúvidas, preparos de exame, financeiro.
* Entregar ao agente de IA os pedidos de agendamento, com aceite de termos (LGPD) incluído.
* Responder de um jeito dentro do horário de funcionamento e de outro fora dele.
* Transferir para o setor ou para a pessoa certa, já com o tema do atendimento definido.

{% hint style="info" %}
**Onde encontrar:** no menu de **Configurações** do Amigo Flow, acesse **Fluxos**.&#x20;
{% endhint %}

### Como criar um fluxo

{% stepper %}
{% step %}
### Clique em "Criar fluxo"

<figure><img src="../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>


{% endstep %}

{% step %}
### Dê um nome ao fluxo

No topo da tela, preencha o campo **Nome do fluxo**. Use um nome que ajude sua equipe a identificá-lo depois — por exemplo, _Menu principal – Unidade Centro_.
{% endstep %}

{% step %}
### Personalize a saudação

Todo fluxo começa em **Conversa começa**, seguido de um passo de **Saudação** com uma mensagem sugerida. Clique no passo para editar o texto no painel lateral.&#x20;
{% endstep %}

{% step %}
### Adicione os próximos passos

Clique em **+ Adicionar passo** (ou no **+** de qualquer passo) e escolha o que acontece em seguida. O novo passo já entra conectado naquele ponto do fluxo.&#x20;
{% endstep %}

{% step %}
### Configure cada passo

Clique em um passo para abrir o painel de configuração à direita. Ali você define o nome do passo, as mensagens e para onde a conversa segue.&#x20;
{% endstep %}

{% step %}
### Publique

Revise o caminho completo e clique em **Publicar**. Se quiser sair sem salvar, clique em **Cancelar**. Em seguida, conecte o fluxo a um canal para ele começar a atender.&#x20;

{% hint style="info" %}
&#x20;**Dica:** use os botões **–** e **+** no canto inferior esquerdo para ajustar o zoom e ter uma visão geral de fluxos maiores.&#x20;
{% endhint %}
{% endstep %}
{% endstepper %}



### Tipos de passo

Ao adicionar um passo, você escolhe entre sete tipos. Todos têm o campo **Nome do passo**, que aparece no desenho do fluxo e facilita a organização.

<figure><img src="../../.gitbook/assets/image (66).png" alt="" width="375"><figcaption></figcaption></figure>

| Passo                   | O que faz                                                        |
| ----------------------- | ---------------------------------------------------------------- |
| **Enviar mensagem**     | O bot envia um texto (e, se quiser, um arquivo).                 |
| **Perguntar e esperar** | O bot faz uma pergunta e aguarda a resposta do paciente.         |
| **Dar opções**          | O paciente escolhe entre botões, e cada opção leva a um caminho. |
| **Verificar condição**  | O fluxo segue por dois caminhos, de acordo com uma regra.        |
| **Iniciar agendamento** | O agente de IA assume e agenda o paciente.                       |
| **Transferir**          | A conversa passa para um setor ou uma pessoa da equipe.          |
| **Encerrar**            | Finaliza a conversa.                                             |

#### Enviar mensagem

Use para informar algo ao paciente: endereço, orientações, horários, boas-vindas.

* **Mensagem enviada:** escreva o texto com formatação do WhatsApp (negrito, itálico, tachado) e emojis.
* **Anexar arquivo:** envie junto uma imagem, documento, áudio ou vídeo.

{% hint style="info" %}
**Formatos aceitos para anexo:** imagens (JPG, JPEG, PNG), documentos (PDF, DOCX, XLS, XLSX, CSV), áudios (OGG, MP3, M4A, AAC) e vídeos (MP4).&#x20;
{% endhint %}

Depois do envio, o fluxo segue automaticamente para o próximo passo.

#### Perguntar e esperar

Use quando precisa que o paciente diga algo antes de continuar — por exemplo, _"Em que posso ajudar?"_.

* **Pergunta enviada:** o texto que o bot envia.
* O bot **aguarda a resposta do paciente** e só então segue para o próximo passo.

#### Dar opções

Cria um menu para o paciente escolher o assunto. É o passo ideal para montar o "menu principal" da clínica.

* **Mensagem do menu:** o texto que acompanha as opções (ex.: _"Como posso te ajudar?"_).
* **Opções que a pessoa pode escolher:** o nome de cada opção, exatamente como o paciente verá.
* **Vai para:** o passo para onde cada opção leva. Você pode criar um passo novo ou apontar para um passo que já existe no fluxo — útil, por exemplo, para um botão "Voltar ao menu".

Use **+ Adicionar opção** para incluir mais escolhas, a lixeira para remover e as alças laterais para reordenar.

{% hint style="info" %}
**Quantas opções posso colocar?** Quantas precisar. Quando o menu tem muitas opções, o paciente vê um botão **Ver mais** no WhatsApp, que abre a lista completa para ele escolher.&#x20;
{% endhint %}

{% hint style="info" %}
&#x20;**Dica:** nomes curtos e diretos são mais fáceis de ler no celular. Para menus muito longos, vale agrupar assuntos em submenus (um passo **Dar opções** dentro de outro).&#x20;
{% endhint %}

#### Verificar condição

Divide o fluxo em dois caminhos, de acordo com uma regra. Hoje, a verificação disponível é o **horário de funcionamento da clínica**:

* **Dentro do horário:** para onde a conversa vai quando a clínica está aberta — por exemplo, transferir para a recepção.
* **Fora do horário:** para onde vai quando a clínica está fechada — por exemplo, avisar o horário de atendimento e oferecer o agendamento com a IA.

{% hint style="info" %}
A regra usa o horário configurado no canal em que o fluxo está conectado: acesse o canal, aba **Regras de atendimento** > **Disponibilidade de horário**. Mantenha-o atualizado para que o fluxo responda corretamente.&#x20;
{% endhint %}

#### Iniciar agendamento

Entrega a conversa para a **habilidade de agendamento** do agente de IA, que agenda o paciente de acordo com a disponibilidade de horários. Quando o agendamento é concluído, o fluxo segue para o próximo passo (por exemplo, **Encerrar**).

* **Pedir aceite de termos (LGPD):** quando ativado, o paciente autoriza o compartilhamento dos seus dados com a clínica antes do cadastro.

{% hint style="warning" %}
Este passo depende da habilidade de agendamento do agente estar ativa. Se ela estiver desativada, a conversa é transferida automaticamente para o setor padrão da conta — o paciente não fica sem atendimento.&#x20;
{% endhint %}

#### Transferir

Passa a conversa para a sua equipe.

* **Mensagem antes de transferir:** um aviso ao paciente (ex.: _"Vou te passar para um atendente. Um momento! 😊"_).
* **Transferir para:**
  * **Setor:** a conversa entra na fila do setor escolhido. Se nenhum setor for definido, ela vai para o setor padrão da conta.
  * **Atendente:** a conversa vai direto para a pessoa escolhida, na fila **Transferidas para mim**. Se essa pessoa não atender mais a conta, a conversa vai para o setor padrão.
* **Tema do atendimento:** classifica a conversa (ex.: Agendamento, Financeiro, Orçamento), o que ajuda a organizar a fila e os relatórios.

#### Encerrar

Finaliza a conversa.

* **Mensagem de despedida:** um último recado ao paciente (ex.: _"Se precisar de algo mais, é só chamar! 👋"_).
* **Tema do atendimento:** registra o assunto da conversa encerrada.

### Conectar o fluxo a um canal

Depois de publicado, o fluxo precisa ser conectado a um canal para começar a atender. A conexão é feita nas configurações do **Agente Flow** de cada canal, no modo **Agente Flow Classic**.

{% hint style="info" %}
&#x20;**Intelligent ou Classic?** O **Agente Flow Intelligent** usa IA para entender linguagem natural e responder com base na sua base de conhecimento. O **Agente Flow Classic** é um chatbot sem IA, que segue exatamente o fluxo que você desenhou, ideal para quem quer respostas 100% previsíveis e controle total do atendimento.&#x20;
{% endhint %}

{% stepper %}
{% step %}
### Acesse o canal

Abra as configurações do canal (número de WhatsApp) que vai usar o fluxo e vá até a aba **Agente Flow**.&#x20;
{% endstep %}

{% step %}
### Escolha o modo Classic

Em **Modo**, clique em **Editar** e selecione **Agente Flow Classic**. Depois, clique em **Escolher fluxo**.&#x20;

<figure><img src="../../.gitbook/assets/image (68).png" alt="" width="375"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Selecione o fluxo

Na lista **Selecione o fluxo**, escolha o fluxo que esse canal vai atender e clique em **Salvar**. Se precisar criar ou ajustar um fluxo nesse momento, use o atalho **Gerenciar**.
{% endstep %}
{% endstepper %}

Pronto: a partir daí, as conversas desse canal seguem o fluxo escolhido. Na tela **Fluxos**, a coluna **Uso** passa a mostrar o canal conectado.

{% hint style="info" %}
Um mesmo fluxo pode ser usado em mais de um canal. Assim, você mantém um padrão de atendimento entre unidades e só precisa editar em um lugar.&#x20;
{% endhint %}

### Exemplo: menu principal de uma clínica

Veja como um fluxo simples pode cobrir os principais assuntos:

```
Conversa começa
└─ Enviar mensagem: saudação
   └─ Dar opções: "Como posso te ajudar?"
      ├─ Agendamento  → Iniciar agendamento → Encerrar
      ├─ Dúvidas      → Perguntar e esperar ("Em que posso ajudar?") → Transferir (Recepção)
      ├─ Localização  → Enviar mensagem (endereço) → Encerrar
      ├─ Preparos     → Dar opções (Endoscopia / Colonoscopia / ...)
      │                  └─ cada opção → Enviar mensagem (preparo + PDF) → Encerrar
      └─ Falar com atendente → Transferir (setor ou pessoa)
```

Para atender também fora do expediente, inclua um passo **Verificar condição** logo após a saudação: dentro do horário, o paciente segue para o menu; fora dele, recebe um aviso e a opção de agendar com a IA.

***

### Gerenciar seus fluxos

Na tela **Fluxos**, você vê todos os fluxos da conta com:

* **Uso:** mostra se o fluxo está **Não utilizado** ou em quantos canais está conectado (ex.: _2 Canais conectados_).
* **Atualizado por** e **Data da atualização:** quem fez a última alteração e quando.

Use o campo **Buscar fluxo** para encontrar um fluxo pelo nome. No menu **⋮** de cada fluxo, você pode:

* **Editar:** abrir o fluxo no editor.
* **Duplicar:** criar uma cópia — ótimo para montar variações, como um fluxo por unidade, sem começar do zero.
* **Excluir:** remover o fluxo.

{% hint style="info" %}
Antes de editar ou excluir um fluxo em uso, confira a coluna **Uso**: as alterações publicadas passam a valer para os canais conectados a ele.
{% endhint %}

***

### Perguntas frequentes

#### Posso ter mais de um fluxo?

Sim. Você pode criar quantos fluxos precisar — por exemplo, um para cada unidade ou canal — e acompanhar na coluna **Uso** onde cada um está conectado.

#### Como faço o paciente voltar ao menu principal?

Em um passo **Dar opções**, crie uma opção como _"Voltar ao menu"_ e, em **Vai para**, selecione o passo do menu principal que já existe no fluxo.

#### O que acontece se a habilidade de agendamento estiver desligada?

O passo **Iniciar agendamento** transfere a conversa automaticamente para o setor padrão da conta. Assim, o paciente sempre é atendido.

#### Posso transferir direto para um profissional específico?

Sim. No passo **Transferir**, escolha **Atendente** e selecione a pessoa. A conversa aparece na fila **Transferidas para mim** dela.

#### Quais condições posso verificar?

Hoje, o passo **Verificar condição** trabalha com o horário de funcionamento da clínica (dentro ou fora do horário). Novas regras estão no nosso radar e serão comunicadas aqui.

#### Publiquei o fluxo, mas ele não está atendendo. O que fazer?

Verifique se o fluxo está conectado a um canal: nas configurações do canal, aba **Agente Flow**, o modo deve estar em **Agente Flow Classic** com o fluxo selecionado. Na tela **Fluxos**, a coluna **Uso** mostra se ele está conectado.

#### De onde vem o horário usado no "Verificar condição"?

Da **Disponibilidade de horário** configurada no canal, na aba **Regras de atendimento**. Se o fluxo estiver em mais de um canal, cada um usa o seu próprio horário.

#### Posso enviar arquivos pelo fluxo?

Sim. No passo **Enviar mensagem**, use **Anexar arquivo** para enviar imagens, PDFs, planilhas, áudios ou vídeos — ideal para preparos de exame e orientações.

#### Minhas alterações valem na hora?

As alterações passam a valer depois que você clica em **Publicar**. Se sair com **Cancelar**, nada é salvo.
