---
icon: user-magnifying-glass
---

# Leads

### Leads

A base de Leads centraliza todos os contatos potenciais da sua clínica em um único lugar. Nela você visualiza os leads, acompanha a jornada de cada um, filtra por etapa ou origem e inicia conversas diretamente pelo WhatsApp, sem sair da tela.

Veja vídeo explicativo clicando aqui:

{% embed url="https://drive.google.com/file/d/113Rj_EO0u9vOw9631lh8vM3vY1_oY9kt/view?usp=drive_link" %}

#### Acessando a tela de Leads

No menu principal do sistema, acesse a aba **Leads**. Você verá a listagem com todos os leads cadastrados na clínica, os cards de resumo por etapa e os filtros para refinar a visualização.

#### Visão geral da tela

A tela tem três áreas principais:

* **Cards de resumo**: mostram quantos leads existem em cada etapa da jornada. Clique em um card para filtrar a listagem por aquela etapa.
* **Barra de ações**: campo de busca por nome ou telefone, filtros avançados e botão para adicionar novos leads.
* **Tabela de leads**: listagem completa com as informações de cada contato e ações rápidas.

#### Informações exibidas na listagem

<figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

Cada linha também tem um ícone do WhatsApp para contato rápido e um menu de ações (três pontos) com opções adicionais.

#### Entendendo os status

Cada lead tem um status que indica em qual etapa da jornada ele está:

<div align="left"><figure><img src="../../.gitbook/assets/image (54).png" alt="" width="224"><figcaption></figcaption></figure></div>

| Status                  | Quando é atribuído                              |
| ----------------------- | ----------------------------------------------- |
| **Não iniciado**        | Lead recém-criado, sem nenhuma conversa ainda   |
| **Em acolhimento**      | Primeira conversa iniciada com a clínica        |
| **Pronto para agendar** | Definido manualmente pela equipe                |
| **Agendado**            | Lead com consulta marcada e ainda não realizada |
| **Não convertido**      | Lead que faltou à consulta agendada             |



O momento em que um lead passa para **Convertidos** depende da regra de conversão escolhida pela clínica (veja a seção abaixo). Os leads convertidos saem da listagem e do quadro do funil e passam a aparecer em **Leads convertidos**. Os leads descartados viram contatos e também deixam de aparecer aqui.

#### Regra de conversão do funil

Você pode definir quando a clínica considera um lead como convertido. Assim, o funil e os indicadores ficam alinhados ao processo comercial da sua equipe.

**Escolhendo a regra de conversão**

Em **Configurações do funil**, selecione uma única regra para toda a clínica:

* **Comparecimento no atendimento**: o lead é convertido quando comparece à primeira consulta.
* **Orçamento fechado**: o lead é convertido quando um orçamento é aprovado.

<div align="center"><figure><img src="../../.gitbook/assets/image (60).png" alt="" width="375"><figcaption></figcaption></figure></div>

A configuração vale para a clínica inteira. Depois de salva, ela passa a valer para o funil e para os indicadores de conversão.

**Atenção:** ao trocar a regra de conversão, o funil e os indicadores passam a seguir apenas a nova regra, e a visualização da regra anterior deixa de ser exibida.

**Etapas automáticas do funil**

As etapas automáticas são definidas pela regra de conversão escolhida. Elas ficam no grupo **Finalização**, com a identificação **Automática**. Essas etapas não podem ser movidas, excluídas ou reordenadas, mas podem ser renomeadas conforme a organização da clínica.

| Etapa automática                       | Comparecimento no atendimento                               | Orçamento fechado |
| -------------------------------------- | ----------------------------------------------------------- | ----------------- |
| Primeiro atendimento com falta         | Exibida                                                     | Exibida           |
| Atendimento realizado/orçamento aberto | Não exibida, porque o comparecimento já conclui a conversão | Exibida           |

**Leads convertidos e indicadores**

Quando acontece o evento definido pela regra escolhida, o lead:

* entra nos indicadores de conversão;
* passa a aparecer na listagem de **Leads convertidos**;
* deixa de aparecer no quadro do funil.

Na regra **Orçamento fechado**, um lead em _Atendimento realizado/orçamento aberto_ é convertido quando o orçamento é aprovado.

**O que permanece igual**

As etapas Não iniciados, Em acolhimento, Prontos para agendar, Agendados e Não convertidos continuam funcionando como antes. A visualização dos cards, o aging, os motivos de perda e a perda automática por inatividade também não mudam.

#### Transições automáticas

O Amigo Flow atualiza alguns status automaticamente:

* Quando o lead entra em contato pela primeira vez, ele vai para **Em acolhimento**.
* Quando uma consulta é agendada, ele vai para **Agendados**.
* Quando a consulta é realizada, o resultado depende da regra de conversão:
  * Na regra **Comparecimento no atendimento**, o lead vai para **Convertidos** e sai da lista.
  * Na regra **Orçamento fechado**, o lead vai para **Atendimento realizado/orçamento aberto**.
* Na regra **Orçamento fechado**, quando o orçamento é aprovado, o lead vai para **Convertidos** e sai da lista.
* Quando o lead falta à primeira consulta, ele vai para **Primeiro atendimento com falta**.
* Quando o lead é sincronizado com um paciente, ele vai para **Descartados** e sai da lista.
* Quando o lead é dessincronizado, ele volta ao status que tinha antes da sincronização.

#### Alterando o status de um lead

Você pode alterar o status direto pela listagem, sem abrir o cadastro completo:

1. Localize o lead na tabela.
2. Clique no status atual, na coluna **Status**.
3. Selecione o novo status no menu.

**Atenção:**

* As etapas automáticas do grupo Finalização não podem ser selecionadas manualmente. Elas são atualizadas pelo sistema conforme a regra de conversão.
* Você pode mover um lead manualmente para **Agendados**, mas ele só permanece nessa etapa se houver uma consulta agendada.
* Leads que já tiveram alguma conversa não podem voltar para _Não iniciados_. Para eles, essa opção não aparece no menu.

Ao selecionar **Descartados**, o sistema pede uma confirmação antes de concluir. O lead vira contato e sai da listagem.

#### Buscando e filtrando leads

**Busca rápida:** digite o nome ou o telefone, completo ou parcial, no campo de busca no topo da listagem. Os resultados são filtrados na hora.

**Filtros disponíveis:**

* **Status**: clique em um card de resumo ou use o filtro para ver os leads de uma etapa.
* **Origem**: mostra apenas os leads vindos de canais específicos, como Instagram, Google Ads ou Importação.
* **Etiquetas**: agrupa os leads por tags de interesse.
* **Data de criação**: ideal para acompanhar campanhas recentes.

Você pode combinar filtros para uma busca mais precisa.

#### Ordenação

A ordenação padrão segue a progressão da jornada: Não iniciados → Em acolhimento → Prontos para agendar → Agendados → Não convertidos.

Clique nos cabeçalhos das colunas Status, Criação, Origem ou Contato para reordenar a listagem e alternar entre ordem crescente e decrescente.

#### Adicionando novos leads

Clique em **"+ Adicionar Leads"** para cadastrar manualmente ou importar em lote.

**Cadastro manual:** um formulário é exibido com os campos abaixo.

| Campo    | Tipo     | Obrigatório | Observação                  |
| -------- | -------- | ----------- | --------------------------- |
| Nome     | Texto    | ✅           | Nome completo do lead       |
| Telefone | Numérico | ✅           | Deve conter DDD             |
| Origem   | Seleção  | ✅           | Escolha o canal de captação |

Depois de salvar, o lead aparece na listagem com status **Não iniciados**.

**Importação em lote:** ao importar uma planilha (por exemplo, CSV), o sistema cria automaticamente uma origem do tipo _Importação #_ com numeração sequencial (Importação #1, Importação #2 etc.). Você pode renomear essa origem durante o processo. Todos os leads importados começam com status **Não iniciados**.

_(_

#### Perguntas frequentes

**Por que um lead desapareceu da listagem?**\
Quando acontece o evento de conversão definido pela clínica (comparecimento ou orçamento aprovado), o lead vai para **Convertidos** e passa a aparecer em **Leads convertidos**. Os leads descartados também saem da listagem e passam a ser exibidos como contatos.

**Onde defino quando um lead é considerado convertido?**\
Em **Configurações do funil**, escolhendo entre _Comparecimento no atendimento_ e _Orçamento fechado_. A regra vale para toda a clínica.

**Posso trocar a regra de conversão depois?**\
Sim. Ao trocar, o funil e os indicadores passam a seguir apenas a nova regra, e a visualização da regra anterior deixa de ser exibida.

**Por que não encontro mais a seção Status automáticos?**\
Agora as etapas automáticas são definidas pela regra de conversão, então não é mais preciso ativá-las ou desativá-las uma a uma.

**Posso mover um lead manualmente para uma etapa automática?**\
Não. As etapas do grupo Finalização são atualizadas apenas pelo sistema. Você pode mover um lead para **Agendados**, mas ele só permanece nessa etapa se houver uma consulta agendada.

**Posso renomear as etapas automáticas?**\
Sim. Você pode renomeá-las, mas não pode movê-las, excluí-las nem reordená-las.

**Posso desfazer a sincronização de um lead com um paciente?**\
Sim. Ao dessincronizar, o lead volta ao status que tinha antes e reaparece na listagem.

**O status pode mudar mais de uma vez automaticamente?**\
Sim. O sistema acompanha a jornada continuamente. Por exemplo, na regra _Orçamento fechado_, um lead pode ir para Agendados, depois para Atendimento realizado/orçamento aberto e, quando o orçamento for aprovado, para Convertidos.

**Como a paginação funciona?**\
A listagem é paginada para facilitar o carregamento. Navegue entre as páginas pelo controle na parte inferior da tela.



