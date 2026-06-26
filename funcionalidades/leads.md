---
icon: user-magnifying-glass
---

# Leads

A base de Leads centraliza todos os contatos potenciais da sua clínica em um único lugar. Com ela, você visualiza, acompanha a jornada de cada lead, filtra por etapa ou origem, e inicia conversas diretamente pelo WhatsApp, tudo sem sair da tela.

### Acessando a tela de Leads

No menu principal do sistema, acesse a aba **Leads**. Você verá uma listagem com todos os leads cadastrados na clínica, acompanhada de cards de resumo por etapa e filtros para refinar a visualização.

### Visão geral da tela

A tela é composta por três áreas principais:

**Cards de resumo** — exibem a contagem total de leads em cada etapa da jornada. Clique em um card para filtrar a listagem automaticamente por aquele status.

**Barra de ações** — campo de busca por nome ou telefone, filtros avançados e botão para adicionar novos leads.

**Tabela de leads** — listagem completa com informações de cada contato e ações rápidas.

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

### Informações exibidas na tabela

| Coluna               | O que mostra                                                                                                               |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Contato**          | Nome completo e telefone do lead                                                                                           |
| **Última interação** | Responsável pelo último atendimento e há quanto tempo ocorreu. Exibe "Sem interação" para leads sem nenhuma conversa ainda |
| **Status**           | Etapa atual do lead na jornada. Clicável para alteração direta                                                             |
| **Criação**          | Quem criou o lead e a data de cadastro                                                                                     |
| **Origem**           | Fonte de captação (ex: Google Ads, Instagram, Importação) e tipo de entrada                                                |

Cada linha também exibe um ícone do WhatsApp para contato rápido e um menu de ações (três pontos) com opções adicionais.

### Entendendo os status

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

Cada lead possui um status que indica em qual etapa da jornada ele se encontra:

| Status                  | Quando é atribuído                              |
| ----------------------- | ----------------------------------------------- |
| **Não iniciado**        | Lead recém-criado, sem nenhuma conversa ainda   |
| **Em acolhimento**      | Primeira conversa iniciada com a clínica        |
| **Pronto para agendar** | Definido manualmente pela equipe                |
| **Agendado**            | Lead com consulta marcada e ainda não realizada |
| **Não convertido**      | Lead que faltou à consulta agendada             |

Leads que **comparecem à consulta** são marcados como Convertidos e saem automaticamente da listagem. Leads **descartados** são convertidos em contatos e também deixam de aparecer aqui.

#### Transições automáticas

O Amigo Flow atualiza alguns status sem que você precise fazer nada:

* Quando um lead entra em contato pela primeira vez → **Em acolhimento**
* Quando uma consulta é agendada → **Agendado**
* Quando a consulta é realizada (comparecimento confirmado) → **Convertido** (sai da lista)
* Quando o lead falta à consulta → **Não convertido**
* Quando o lead é sincronizado com um paciente → **Descartado** (sai da lista)
* Quando o lead é dessincronizado → retorna ao status anterior à sincronização

***

### Alterando o status de um lead

Você pode alterar o status diretamente pela listagem, sem abrir o cadastro completo:

1. Localize o lead na tabela
2. Clique no **status atual** exibido na coluna Status
3. Selecione o novo status no menu

> **Atenção:** Leads que já tiveram alguma conversa não podem retornar ao status "Não iniciado". Para esses casos, essa opção não estará disponível no menu.

Ao selecionar **Descartado**, uma confirmação será solicitada antes de concluir a ação. O lead é convertido em contato e removido da listagem.

### Buscando e filtrando leads

**Busca rápida:** digite o nome ou telefone (completo ou parcial) no campo de busca no topo da listagem. O sistema filtra os resultados instantaneamente.

**Filtros disponíveis:**

* **Status** — clique em um card de resumo ou use o filtro para exibir leads de uma etapa específica
* **Origem** — exibe apenas leads vindos de canais específicos (Instagram, Google Ads, Importação etc.)
* **Etiquetas** — agrupa leads por tags de interesse
* **Data de criação** — ideal para acompanhar campanhas recentes

Você pode combinar filtros para uma busca mais precisa.

### Ordenação

A ordenação padrão segue a progressão da jornada: Não iniciado → Em acolhimento → Pronto para agendar → Agendado → Não convertido.

Clique nos cabeçalhos das colunas **Status**, **Criação**, **Origem** ou **Contato** para reordenar a listagem e alternar entre crescente e decrescente.

### Adicionando novos leads

Clique em **"+ Adicionar Leads"** para cadastrar manualmente ou importar em lote.

#### Cadastro manual

Um formulário será exibido com os seguintes campos:

| Campo    | Tipo     | Obrigatório | Observação                  |
| -------- | -------- | ----------- | --------------------------- |
| Nome     | Texto    | ✅           | Nome completo do lead       |
| Telefone | Numérico | ✅           | Deve conter DDD             |
| Origem   | Seleção  | ✅           | Escolha o canal de captação |

Após salvar, o lead aparece imediatamente na listagem com status **Não iniciado**.

#### Importação em lote

Ao importar uma planilha (ex: CSV), o sistema cria automaticamente uma origem do tipo **Importação #** com numeração sequencial (Importação #1, Importação #2 etc.). Você pode renomear essa origem durante o processo. Todos os leads importados iniciam com status **Não iniciado**.

### Gerenciando etiquetas

As etiquetas funcionam como marcadores de interesse ou contexto, facilitando o agrupamento de leads. Cada lead pode ter uma ou várias etiquetas, exibidas visualmente na listagem.

Exemplos de uso: `Pré-consulta` · `Campanha julho` · `Indicação` · `Interesse em ortodontia`

### Exportando leads

Para exportar sua base:

1. Aplique os filtros desejados (opcional)
2. Clique no botão de exportação

A planilha gerada inclui todos os dados da listagem com a coluna de status. Se um filtro estiver ativo, apenas os leads filtrados serão exportados.

### Contatando leads pelo WhatsApp

À direita de cada lead há um ícone do WhatsApp:

* **Número com conta ativa** → abre o WhatsApp diretamente no navegador ou aplicativo, com o número já formatado
* **Número sem WhatsApp** → ícone aparece cinza com tooltip: _"Este número não possui WhatsApp vinculado."_

O sistema utiliza o formato internacional automaticamente, garantindo compatibilidade com o app.

### Origens e canais de entrada

**Origens disponíveis:** Instagram · Facebook · WhatsApp · Telegram · Site da clínica · Google Meu Negócio · Meta Ads · Google Ads · Chat do site · Indicação · Evento · Formulário de landing page · Google Forms · Lista de transmissão no WhatsApp · Campanha de e-mail marketing · Outro

**Tipos de entrada:** Detecção automática (via agente) · Importação · Manual

### Perguntas frequentes

**Por que um lead desapareceu da listagem?** Leads que comparecem à consulta são movidos para Convertido e saem automaticamente. Leads descartados também são removidos e passam a ser exibidos como contatos.

**Posso desfazer a sincronização de um lead com um paciente?** Sim. Ao dessincronizar, o lead retorna ao status que tinha antes e volta a aparecer na listagem.

**O status pode mudar mais de uma vez automaticamente?** Sim. O sistema acompanha a jornada continuamente. Um lead pode receber o status Agendado assim que a consulta for marcada e, após a consulta, ser atualizado para Convertido automaticamente.

**Como a paginação funciona?** A listagem é paginada para facilitar o carregamento. Navegue entre páginas pelo controle na parte inferior da tela.



###
