# Consentimento LGPD no Cadastro de Leads (Opt-in)

Estamos implementando uma etapa obrigatória de **consentimento explícito (opt-in)** antes da coleta de dados pessoais no fluxo de cadastro de leads via WhatsApp.

Essa evolução tem três objetivos claros:

1. **Conformidade com LGPD** (base legal documentada e auditável).
2. **Proteção jurídica da clínica**.
3. **Maturidade do produto** rumo a um CRM clínico estruturado e escalável.

A partir dessa atualização, nenhum dado pessoal será coletado antes do consentimento formal do usuário.

***

## 🧠 Como passa a funcionar

### 1️⃣ Solicitação de Consentimento (Opt-in)

Antes de qualquer coleta de dados:

**Mensagem enviada:**

> Antes de prosseguir com o cadastro, você autoriza o uso dos seus dados pessoais para realizar seu cadastro, agendamentos e comunicações com nossa clínica?

Botões:

* ✅ **Sim, autorizo**
* ❌ **Não autorizo**

***

### 2️⃣ Regras de decisão

#### ✅ Se o paciente autorizar:

* Fluxo segue normalmente para coleta de dados.
* Consentimento é registrado formalmente.

#### ❌ Se o paciente não autorizar:

* Fluxo é encerrado.
* Evento é logado.
* Nenhum dado pessoal é armazenado.
* Bloqueio automático de futuras comunicações automatizadas.

***

## 🗄️ Registro do Consentimento

Ao receber aceite positivo:

#### Dados armazenados:

* `lead_id`
* `consent_status = true`
* `timestamp`
* `channel = WhatsApp`
* `conversation_id`

#### Atualização automática:

* Ficha do paciente marcada como **“Consentimento LGPD ativo”**

***

## 📥 Coleta de Dados

A coleta de informações pessoais ocorre **somente após confirmação do opt-in**.

Fluxo de cadastro segue normalmente após essa etapa.

***

## 📩 Confirmação e Transparência

Após registro do consentimento:

> Ótimo, seus dados foram registrados com segurança.\
> Você poderá revisar ou revogar seu consentimento a qualquer momento digitando “revogar autorização”.

***

## 🔐 Revogação

Se o paciente digitar:

**“revogar autorização”**

Ações automáticas:

* Atualiza `consent_status = false`
* Bloqueia fluxos de marketing e campanhas
* Registra evento na auditoria
* Atualiza status na ficha

***

## 📊 Auditoria e Compliance

### Novos recursos:

* Registro automático em tabela de auditoria
* Endpoint `/consent/logs` para consulta e exportação
* Nova aba no painel: **“Privacidade e LGPD”**
* Bloqueio preventivo de disparos caso consentimento esteja como “não autorizado”

Isso reduz risco de:

* Disparos indevidos
* Uso indevido de base
* Questionamentos jurídicos
* Problemas em auditorias futuras

***

## 🧩 Resumo Técnico do Fluxo

| Etapa | Evento                  | Tool / Endpoint     | Registro                  |
| ----- | ----------------------- | ------------------- | ------------------------- |
| 1     | Início da conversa      | Amigo Flow          | —                         |
| 2     | Solicitação do opt-in   | Template WhatsApp   | Mensagem enviada          |
| 3     | Resposta positiva       | `/consent/register` | Consentimento + Timestamp |
| 4     | Coleta de dados         | Agente de Cadastro  | Dados armazenados         |
| 5     | Resumo do consentimento | Mensagem padrão     | —                         |
| 6     | Auditoria               | `/consent/logs`     | Consulta e exportação     |

***

## 🎯 Impacto Estratégico

Essa entrega posiciona o produto em um novo patamar:

* CRM mais robusto juridicamente
* Estrutura pronta para campanhas com base legal clara
* Base de leads com rastreabilidade
* Redução de risco regulatório
* Preparação para integrações futuras (Meta, campanhas, automações)

Sem consentimento, não existe CRM sustentável.\
Agora existe.

***

Se quiser, posso transformar isso também em:

* 📢 Comunicado interno para time comercial
* 📘 Documento técnico para engenharia
* 📄 Documento simplificado para enviar às clínicas
* 🧾 Política de privacidade adaptada ao fluxo

Qual próximo passo você quer estruturar?
