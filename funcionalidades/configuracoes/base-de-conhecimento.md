# Base de conhecimento

Com a Base de conhecimento, você ensina ao Agente Flow tudo o que ele pode informar aos pacientes: convênios aceitos, valores, regras de cancelamento, prazos de retorno, endereço das unidades e as dúvidas mais comuns da sua clínica.

Em vez de um texto livre, a base é organizada em **8 seções**, uma para cada assunto. Cada seção tem campos próprios, muitos deles já preenchidos com o que está cadastrado no Amigo. Assim, o agente sabe exatamente onde buscar cada resposta, e a clínica sabe exatamente o que ele vai dizer.

{% hint style="success" %}
**Na prática:** quando um paciente pergunta "vocês atendem Bradesco Saúde?", o agente confere a lista de convênios marcados na base antes de oferecer horário. Se o convênio não está lá, ele responde que a clínica não atende, sem prometer exceção.
{% endhint %}

Veja o tour completo:

{% embed url="https://drive.google.com/file/d/1IwtgG91bZC7HDLzQCFbj2nFWUKNY9bA_/view?usp=drive_link" %}

{% hint style="info" %}
A Base de conhecimento está disponível no modo **Agente Flow Intelligent**.
{% endhint %}

## Já usa uma base de conhecimento? Nada muda até você salvar

Se a sua clínica já tinha uma base cadastrada, ela **continua funcionando normalmente**. O agente segue respondendo com o conteúdo atual enquanto nenhuma seção nova for salva.

A troca só acontece quando a clínica decide: **ao salvar a primeira seção**, o agente passa a responder com o que estiver nas novas seções. Até lá, você pode abrir, conhecer e preencher as seções com calma.

Ao entrar na tela, você verá o aviso _"A configuração da base de conhecimento mudou. A sua continua funcionando."_. Clique em **Ver itens anteriores** para consultar o conteúdo que você já tinha cadastrado e aproveitá-lo no preenchimento das novas seções.

{% hint style="warning" %}
**Antes do primeiro salvamento:** preencha primeiro as seções mais importantes para o seu atendimento, como Convênios e formas de pagamento e Localização. Depois que a primeira seção for salva, o agente passa a usar só as novas seções, e o conteúdo anterior deixa de valer.
{% endhint %}

## Como acessar

1. No Amigo Flow, acesse **Configurações › Agente Flow**.
2. Na aba **Agente Flow**, clique em **Base de conhecimento**, no menu da esquerda.

## A lista de seções

A tela abre com as 8 seções e o progresso da base, por exemplo, **"3 de 8 seções completas"**.

| Seção                                           | O que o agente usa dela                                                                   |
| ----------------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Convênios e formas de pagamento**             | Convênios aceitos, valores particulares e formas de pagamento.                            |
| **Serviços e especialidades oferecidas**        | O que a clínica atende, incluindo teleconsulta, para não oferecer o que não existe.       |
| **Cancelamento, reagendamento e faltas**        | Regras para quando o paciente quer desmarcar, remarcar ou se atrasou.                     |
| **Retornos**                                    | Prazo do retorno sem custo, com quem é feito e o que levar.                               |
| **Guias e autorização**                         | Quando o convênio exige autorização prévia e o que fazer se a guia não saiu.              |
| **Resultados e documentos**                     | Prazo e canal de entrega de resultados, segunda via de documentos e renovação de receita. |
| **Localização e como chegar**                   | Endereço, referência, estacionamento e acessibilidade de cada unidade.                    |
| **Perguntas frequentes específicas da clínica** | Perguntas e respostas que o agente usa palavra por palavra.                               |

Cada seção mostra um status:

| Status         | Quando aparece                                                                      |
| -------------- | ----------------------------------------------------------------------------------- |
| **Vazia**      | Nenhum campo obrigatório foi preenchido.                                            |
| **Incompleta** | Parte dos campos obrigatórios foi preenchida. A linha mostra quantos campos faltam. |
| **Completa**   | Todos os campos obrigatórios estão preenchidos.                                     |

Clique em qualquer linha para abrir a seção.

## Como preencher uma seção

Toda seção segue o mesmo formato:

1. No topo, o bloco **O que o agente faz com esta seção** explica, em três frases, como o agente usa aquelas informações.
2. Abaixo, preencha os campos. Cada campo tem um texto de ajuda dizendo o que o agente faz com ele.
3. Campos obrigatórios vazios mostram o aviso **"Preencha para completar a seção."**. Campos opcionais aparecem marcados como **Opcional**.
4. Clique em **Salvar seção** e confirme.

{% hint style="info" %}
Cada seção é salva e ativada de forma independente. O que você salvar já vale para o agente, mesmo que as outras seções continuem em branco. Não é preciso completar tudo de uma vez.
{% endhint %}

O salvamento vale na hora, inclusive para as conversas em andamento. O agente pode levar até 5 minutos para começar a usar a versão nova.

Se você clicar em **Voltar para as seções** com alterações não salvas, o sistema pergunta se deseja **Salvar** ou **Descartar**. Nada se perde sem a sua confirmação.

## O que preencher em cada seção

### Convênios e formas de pagamento

* **Tipo de atendimento:** ligue **A clínica atende somente particular** se a clínica não trabalha com convênios. Nesse caso, a lista de convênios sai da base e o agente usa a mensagem que você escrever.
* **Convênios aceitos:** a lista vem dos convênios já cadastrados no Amigo. Marque os que o agente pode confirmar, ou ligue **Incluir todos os convênios cadastrados** para que novos convênios entrem automaticamente.
* **Convênios não aceitos** (opcional): planos que os pacientes costumam perguntar e a clínica não atende. O agente responde que não atende, sem abrir negociação.
* **Formas de pagamento particular:** marque as opções aceitas, como Pix, Dinheiro, Débito, Crédito, Boleto e Transferência.
* **Parcelamento:** escolha **Parcelamos** ou **Não parcelamos**. O agente só fala disso quando o paciente pergunta.
* **Valores particulares:** a tabela vem preenchida com o valor particular dos procedimentos cadastrados no Amigo. Você pode editar, remover ou adicionar linhas só para o agente, sem alterar o cadastro. Para voltar aos valores originais, clique em **Restaurar valores cadastrados**.
* **Carência e cobertura** e **Reembolso e nota fiscal:** textos que o agente usa para orientar o paciente, sem afirmar cobertura de procedimentos específicos.

{% hint style="success" %}
**Na prática:** prefere que o agente não informe o valor de um procedimento? Marque **Não informar, transferir** na linha correspondente. Quando o paciente perguntar, o agente encaminha a conversa para a equipe.
{% endhint %}

Para incluir ou remover um convênio da lista, altere o cadastro em **Configurações › Convênios**. A base sempre espelha o cadastro da clínica.

### Serviços e especialidades oferecidas

* **Especialidades atendidas** e **exames e procedimentos realizados:** listas vindas do cadastro do Amigo. O agente confirma se o serviço existe antes de oferecer horário.
* Especialidades sem profissional com agenda ativa aparecem travadas, com a indicação **"Sem agenda ativa — o agente não oferece"**.
* **O que a clínica não faz:** o agente responde que o serviço não é oferecido, sem sugerir alternativas.
* **Teleconsulta:** ligue para informar como funciona, quais especialidades atendem online e o que o paciente precisa.

O preparo de cada exame continua em **Orientações médicas**, e a idade mínima e máxima para agendar fica em **Habilidades › Agendamento**.

### Cancelamento, reagendamento e faltas

* **Prazo para cancelar sem custo:** em horas antes do horário marcado.
* **Como cancelar ou remarcar:** marque os canais (WhatsApp, Telefone, Recepção, Portal ou app). O agente indica esses canais em vez de simplesmente pedir que o paciente ligue.
* **Cobrança por falta:** o agente informa a regra, mas nunca negocia valor nem concede isenção.
* **Atraso tolerado:** o tempo de tolerância que o agente informa ao paciente.

{% hint style="info" %}
O prazo informado aqui é o que o agente **comunica** ao paciente. A antecedência mínima para o próprio agente cancelar uma consulta é configurada em **Habilidades › Cancelamento**.
{% endhint %}

### Retornos

* **Prazo do retorno sem custo:** já vem preenchido com o maior prazo de retorno cadastrado nos tipos de atendimento.
* **Profissional do retorno:** com o mesmo profissional da consulta, com qualquer profissional da mesma especialidade ou outra regra.
* **O que levar no retorno:** exames solicitados, receita atual, documento com foto, carteirinha do convênio, pedido médico ou outro item.

### Guias e autorização

* **Quando é preciso autorização prévia:** marque os tipos de atendimento que exigem guia e quem solicita a autorização (a clínica ou o paciente). O agente avisa antes de agendar.
* **Validade do pedido médico:** o agente informa esse prazo ao paciente.
* **Se a guia não saiu:** a orientação que o agente passa ao paciente.

### Resultados e documentos

* **Prazo e canal de entrega de resultados:** informe o prazo e marque os canais. O agente nunca interpreta resultados nem comenta valores de exames.
* **Segunda via de atestado** e **segunda via de receita:** prazo, canais e se há cobrança de taxa.
* **Renovação de receita:** por segurança, o agente sempre encaminha esse pedido para a equipe.

### Localização e como chegar

Cada unidade cadastrada tem a sua aba. Para cada uma, preencha:

* **Endereço completo:** vem do cadastro em **Configurações › Unidades**. O agente envia esse endereço na confirmação do agendamento.
* **Ponto de referência**, **Estacionamento** e **Transporte público** (opcional).
* **Acessibilidade:** rampa de acesso, elevador, atendimento prioritário e observações.

### Perguntas frequentes específicas da clínica

Use esta seção para as perguntas que são só da sua clínica. O agente responde com o texto cadastrado, palavra por palavra, e reconhece variações da mesma pergunta.

1. Clique em **Adicionar pergunta** e preencha a pergunta e a resposta.
2. Ou clique em **Importar de PDF** para trazer perguntas de um material que a clínica já tem. As perguntas encontradas entram na lista para você revisar antes de salvar.
3. Clique em **Salvar seção**.

A seção comporta até **10 perguntas**, somando as importadas e as criadas. O PDF precisa ter texto selecionável e até 10 MB.

{% hint style="warning" %}
Quando uma resposta do FAQ contradiz outra seção, vale a resposta do FAQ. Por isso, revise valores e prazos citados nas respostas para que fiquem iguais ao restante da base.
{% endhint %}

## Quando a informação não está na base

O agente não improvisa. Se o paciente pergunta algo que nenhuma seção responde, o agente diz que não tem essa informação e oferece falar com um atendente, tirar outra dúvida ou agendar. A conversa só é transferida se o paciente aceitar o atendente ou insistir na mesma dúvida.

Se a seção trata do assunto, mas falta o dado específico, o agente transfere para a equipe na hora.

{% hint style="success" %}
**Na prática:** percebeu que muitos pacientes perguntam algo que o agente não sabe responder? É um sinal de que vale preencher a seção correspondente ou incluir a pergunta no FAQ.
{% endhint %}

## O que isso melhora na rotina

Com a nova Base de conhecimento, a clínica passa a:

* reduzir respostas vagas ou incorretas do agente;
* manter convênios, especialidades, valores e endereços alinhados ao cadastro do Amigo;
* saber exatamente o que o agente pode dizer em cada assunto;
* atualizar uma informação em um só lugar, sem reescrever todo o texto;
* evoluir a base aos poucos, seção por seção.

**Dica para o dia a dia da clínica:** comece pelas seções que mais aparecem nas conversas, como Convênios, Localização e Cancelamento. Sempre que uma regra mudar na clínica, atualize a seção correspondente. O agente passa a usar a versão nova em poucos minutos.

## Dúvidas frequentes

<details>

<summary>Já tenho uma base de conhecimento. Vou perder o que cadastrei?</summary>

Não. A sua base atual continua funcionando e o agente segue usando ela enquanto nenhuma seção nova for salva. O conteúdo anterior pode ser consultado em **Ver itens anteriores**.

</details>

<details>

<summary>Quando o agente passa a usar as novas seções?</summary>

Ao salvar a primeira seção. A partir daí, o agente responde com o que estiver nas novas seções.

</details>

<details>

<summary>Preciso preencher todas as seções de uma vez?</summary>

Não. Cada seção é salva e ativada de forma independente. Seções vazias não entram nas respostas do agente, e seções incompletas entram só com os campos preenchidos.

</details>

<details>

<summary>Em quanto tempo o agente usa uma informação que acabei de salvar?</summary>

O salvamento vale na hora, inclusive para as conversas em andamento. O agente pode levar até 5 minutos para começar a usar a versão nova.

</details>

<details>

<summary>Editar um valor na base altera o cadastro do Amigo?</summary>

Não. As alterações na tabela de valores particulares valem só para o agente. Para voltar aos valores do cadastro, use **Restaurar valores cadastrados**.

</details>

<details>

<summary>Por que um convênio ou especialidade não aparece na lista?</summary>

As listas espelham o cadastro da clínica. Para incluir um convênio, altere o cadastro em **Configurações › Convênios**. Especialidades sem profissional com agenda ativa aparecem travadas e não são oferecidas pelo agente.

</details>

<details>

<summary>O que acontece se uma resposta do FAQ for diferente de outra seção?</summary>

Vale a resposta do FAQ. Por isso, mantenha valores e prazos das respostas iguais aos das outras seções.

</details>

<details>

<summary>O agente pode inventar uma resposta quando não encontra a informação?</summary>

Não. Sem a informação na base, o agente avisa que não tem esse dado e oferece falar com um atendente, tirar outra dúvida ou agendar.

</details>
