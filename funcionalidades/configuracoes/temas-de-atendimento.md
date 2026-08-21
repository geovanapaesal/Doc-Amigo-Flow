# Temas de atendimento

Agora você consegue organizar melhor os atendimentos no Flow com **Temas de atendimento,** para classificar a temática dos atendimentos que chegam na sua clínica.

### Temas de atendimento <a href="#fb1aae05-04c8-4cc3-b83f-2fcd0b732f42" id="fb1aae05-04c8-4cc3-b83f-2fcd0b732f42"></a>

Temas de atendimento são categorias que a própria clínica cadastra para classificar os atendimentos realizados no Amigo Flow. Eles ajudam a padronizar a análise do histórico e facilitam a leitura do que mais gera demanda na operação.

#### Onde configurar <a href="#a594e1d0-51b0-459a-8c54-d0a7045e6e66" id="a594e1d0-51b0-459a-8c54-d0a7045e6e66"></a>

O cadastro fica em **Configurações → Amigo Flow → Temas de Atendimento**.

#### Como cadastrar um tema <a href="#ebaab8f8-8e9f-49b5-af90-74f96710d598" id="ebaab8f8-8e9f-49b5-af90-74f96710d598"></a>

Ao criar um tema, você informa:

* **Nome do tema**: campo obrigatório.
* **Descrição**: campo opcional, com limite de **256 caracteres**.
* **Canais**: por padrão, o tema pode ficar disponível em **Todos os canais**, mas você também pode escolher canais específicos.

#### Regras do cadastro <a href="#id-4d7784c4-76ca-4014-abc0-6add43678eac" id="id-4d7784c4-76ca-4014-abc0-6add43678eac"></a>

* Não é possível salvar dois temas com o mesmo nome.
* Não há limite de quantidade de temas cadastrados.
* Depois de salvar, o tema aparece imediatamente na listagem.
* A associação de canais define em quais atendimentos aquele tema poderá ser usado.

#### Listagem e gestão dos temas <a href="#fda4ea88-4292-4dd2-a00e-36a50c24df9a" id="fda4ea88-4292-4dd2-a00e-36a50c24df9a"></a>

Na listagem, você consegue acompanhar:

* **Temas**
* **Canal**
* **Atualizado por**
* **Data da atualização**

Também é possível:

* **Editar** um tema existente
* **Excluir** um tema existente
* **Ordenar** a listagem por **Temas** (A → Z e Z → A)
* **Ordenar** a listagem por **Data da atualização** (mais recente → mais antiga e o inverso)

### Seleção de temas ao finalizar um atendimento <a href="#id-12df145b-c1f8-4364-8ff2-f1dc1d1752b5" id="id-12df145b-c1f8-4364-8ff2-f1dc1d1752b5"></a>

> **Status atual do rascunho:** funcionalidade em validação.

Ao finalizar um atendimento, o modal de finalização passa a exibir o campo **Tema de Atendimento**.

<figure><img src="../../.gitbook/assets/Captura de Tela 2026-07-31 às 09.49.37.png" alt=""><figcaption></figcaption></figure>

#### Como funciona <a href="#id-0193d8a0-3c7b-4305-b49b-b5f07b7a65c0" id="id-0193d8a0-3c7b-4305-b49b-b5f07b7a65c0"></a>

* O campo é **opcional**.
* A lista mostra apenas os **temas ativos** associados ao canal daquele atendimento.
* Se não houver tema disponível para o canal, o sistema exibe **“Nenhum tema encontrado”**.
* Você pode selecionar **até 10 temas** no mesmo atendimento.
* Os temas escolhidos aparecem no resumo antes da confirmação.

#### Depois da finalização <a href="#id-6aa27b16-91f7-4a20-8f77-f789d71ccc8a" id="id-6aa27b16-91f7-4a20-8f77-f789d71ccc8a"></a>

* Os temas ficam registrados no atendimento finalizado.
* Esses dados passam a ficar disponíveis para consulta no histórico.
* O tema não pode ser alterado depois que o atendimento é finalizado.

### Filtro por tema no histórico de atendimentos <a href="#id-284e0475-e895-4097-b6e2-359605e18ec4" id="id-284e0475-e895-4097-b6e2-359605e18ec4"></a>

> **Status atual do rascunho:** funcionalidade em validação.

No **Histórico de Atendimentos**, o drawer de filtros passa a incluir o campo **Tema de Atendimento**.

#### O que o filtro permite <a href="#id-7dd83999-0853-4c52-bcd8-ae0fcf5e4199" id="id-7dd83999-0853-4c52-bcd8-ae0fcf5e4199"></a>

* Selecionar **um ou mais temas** ao mesmo tempo.
* Combinar o filtro de tema com outros filtros já existentes, como data, canal e atendente.
* Visualizar o filtro ativo como **tag/chip** na listagem.
* Remover apenas o filtro de tema sem limpar os demais.

#### Regras importantes <a href="#cb94ce58-cabf-45dc-b8ad-905aa127b9f0" id="cb94ce58-cabf-45dc-b8ad-905aa127b9f0"></a>

* A lista de opções inclui **temas ativos e inativos**, para preservar buscas históricas.
* Atendimentos sem tema registrado não aparecem quando esse filtro está ativo.
* Alterações ou exclusões feitas em um tema não apagam o vínculo com atendimentos já finalizados.

### Sugestão automática de temas pelo Agente Flow <a href="#d25e6576-ab45-457e-826c-cdfb51375fbd" id="d25e6576-ab45-457e-826c-cdfb51375fbd"></a>

O **Agente Flow** organiza os atendimentos automaticamente para clínicas que utilizam o Agente de IA.

Ao encerrar uma conversa ou transferi-la para um atendente humano, o agente analisa o atendimento completo. Em seguida, sugere o tema mais adequado no modal de finalização.

#### Como funciona <a href="#id-6244268c-7274-45e6-a2a8-e32e8c118d91" id="id-6244268c-7274-45e6-a2a8-e32e8c118d91"></a>

* A sugestão usa somente os **temas ativos** cadastrados pela clínica.
* Novos temas e temas inativados são considerados automaticamente.
* O tema sugerido fica **pré-selecionado** para revisão antes da confirmação.
* O atendente pode aceitar, trocar ou remover a sugestão.
* O agente não sugere um tema sem confiança na classificação.

Se não houver temas ativos, ou se a conversa não corresponder claramente a um tema, o atendimento fica sem sugestão. Nesse caso, o atendente seleciona o tema manualmente.

{% hint style="info" %}
Configure temas claros e específicos em **Configurações → Amigo Flow → Temas de Atendimento**. Uma estrutura bem definida melhora a qualidade das sugestões.
{% endhint %}

### Categorização automática dos motivos de transferência <a href="#id-5bfbde83-7613-4308-b6eb-cc364e187a60" id="id-5bfbde83-7613-4308-b6eb-cc364e187a60"></a>

Quando um atendimento é transferido do Agente Flow para o atendimento humano, o sistema também pode registrar um **motivo de transferência estruturado**. Isso ajuda a analisar volume, recorrência e gargalos com mais consistência.

#### Como funciona <a href="#id-91753392-5a2e-41b5-b2bf-fb83cdef58c1" id="id-91753392-5a2e-41b5-b2bf-fb83cdef58c1"></a>

No momento em que a razão da transferência é registrada, ela é enviada de forma assíncrona para classificação automática. O sistema associa o atendimento a uma categoria padronizada, sem travar o fluxo da transferência.

#### Categorias disponíveis <a href="#id-6db51168-f7b5-442f-85e9-70fb1cde24e5" id="id-6db51168-f7b5-442f-85e9-70fb1cde24e5"></a>

* **Agendamento a concluir pelo atendente**
* **Dúvidas e informações gerais**
* **Remarcação de consulta ou exame**
* **Parâmetros do agendamento não encontrados**
* **Documentos e solicitações administrativas**
* **Preferência por atendimento humano**
* **Encaixe ou urgência**
* **Cancelamento de consulta ou exame**
* **Cadastro e dados do paciente**
* **Outros**

#### Regras desse processo <a href="#ddab72ce-f8a7-4797-9c6f-5fdc4685b348" id="ddab72ce-f8a7-4797-9c6f-5fdc4685b348"></a>

* A classificação usa apenas o texto da razão da transferência e a lista de categorias disponíveis.
* Em caso de falha, o atendimento pode ser direcionado para **Outros**.
* O dado categorizado fica disponível para uso em análises, filtros e dashboards.

### O que isso muda na rotina da clínica <a href="#id-4fc89a50-e966-4362-86f7-2edad211c366" id="id-4fc89a50-e966-4362-86f7-2edad211c366"></a>

Com esse conjunto de entregas, a clínica passa a ter uma estrutura melhor para:

* padronizar a categorização dos atendimentos;
* entender quais temas aparecem com mais frequência;
* encontrar atendimentos no histórico com mais rapidez;
* acompanhar melhor os casos que precisaram de transferência para um humano.
