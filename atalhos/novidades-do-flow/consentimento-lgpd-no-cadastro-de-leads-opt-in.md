---
icon: user-lock
---

# Consentimento LGPD no Cadastro de Leads (Opt-in)

Estamos implementando uma etapa obrigatória de **consentimento explícito (opt-in)** antes da coleta de dados pessoais no fluxo de cadastro de leads via WhatsApp.

Essa evolução tem três objetivos claros:

1. **Conformidade com LGPD** (base legal documentada e auditável).
2. **Proteção jurídica da clínica**.
3. **Maturidade do produto** rumo a um CRM clínico estruturado e escalável.

A partir dessa atualização, nenhum dado pessoal será coletado antes do consentimento formal do usuário.

## 🧠 Como passa a funcionar

### 1️⃣ Solicitação de Consentimento (Opt-in)

Antes de qualquer coleta de dados:

**Mensagem enviada:**

> Antes de prosseguir com o cadastro, você autoriza o uso dos seus dados pessoais para realizar seu cadastro, agendamentos e comunicações com nossa clínica?

Botões:

* ✅ **Sim, autorizo**
* ❌ **Não autorizo**

### 2️⃣ Regras de decisão

#### ✅ Se o paciente autorizar:

* Fluxo segue normalmente para coleta de dados.
* Consentimento é registrado formalmente.

#### ❌ Se o paciente não autorizar:

* Fluxo é encerrado.
* Evento é logado.
* Nenhum dado pessoal é armazenado.
* Bloqueio automático de futuras comunicações automatizadas.

## 🗄️ Registro do Consentimento

Ao receber aceite positivo:

* Ficha do paciente marcada como **“Consentimento LGPD ativo”**

## 📥 Coleta de Dados

A coleta de informações pessoais ocorre **somente após confirmação do opt-in**.

Fluxo de cadastro segue normalmente após essa etapa.

## 📩 Confirmação e Transparência

Após registro do consentimento:

> Ótimo, seus dados foram registrados com segurança.\
> Você poderá revisar ou revogar seu consentimento a qualquer momento digitando “revogar autorização”.





