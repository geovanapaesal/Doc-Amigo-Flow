# 📲 Como fazer a portabilidade de um número com API Oficial para o Amigo Flow

O que é a portabilidade entre provedores da API Oficial?

A **portabilidade**, neste caso, significa **migrar seu número da API Oficial** de um provedor atual para a infraestrutura de API utilizada pelo **Amigo Flow**.\
É um processo técnico homologado pela **Meta**, que permite manter o mesmo número, preservando o **histórico de mensagens**, a **qualidade da conta** e a **reputação empresarial**.

{% hint style="warning" %}
### &#x20;**Pré-requisitos**

Antes de começar, garanta que todos esses pontos estão ok:

1. O cliente **já possui uma WABA própria** (não pode ser uma conta “em nome de” outro parceiro) e tem **acesso de administrador** ao **Gerenciador de Negócios da Meta**;
2. As **moedas da linha de crédito** do cliente e da sua empresa **devem ser iguais**.
3. O cliente **está ciente que não poderá enviar mensagens** entre a remoção do parceiro antigo e a ativação da nova linha de crédito (ver cronograma abaixo).
4. A migração **não deve ser feita nos primeiros 4 dias nem nos últimos 3 dias do mês**, por limitação da Meta.
5. Se o cliente usa **API Local**, será preciso **registrar os números novamente** após a migração (API de Nuvem não precisa disso).
6. O número **já está conectado** à API Oficial da Meta com outro provedor;
7. O número está vinculado a uma **conta de portfólio empresarial verificado**;
8. A **autenticação em dois fatores (2FA)** da **WABA** está **desativada**;
9. O número está **ativo** e habilitado para **receber chamadas telefônicas**, pois o código de verificação da Meta será enviado por ligação durante o processo.
{% endhint %}

### &#x20;**Dependências**

* Acesso do cliente ao **Meta Business Suite**.
* Acesso do parceiro ao **Gerenciador de Negócios** e à **API Meta** (para trocar tokens e compartilhar crédito).
* Comunicação clara com o cliente durante o processo (o envio de mensagens fica temporariamente bloqueado).

### **Passo a Passo**

#### **Etapa 1: Cliente cancela o compartilhamento com o parceiro atual**

1. Peça para o cliente acessar:\
   👉 [https://business.facebook.com/settings](https://business.facebook.com/settings)
2. No menu, ele deve entrar em:\
   **Configurações do negócio > Contas > Contas do WhatsApp > Aba “Parceiros”**
3. Ele deve localizar o parceiro atual, clicar no ícone 🗑️ (lixeira) e **remover o compartilhamento**.
4. Após isso, **o cliente não poderá enviar mensagens** até a nova linha de crédito ser aplicada.
   * Se tentar enviar, receberá o erro **131042**.

> 💡 Dica: oriente o cliente a fazer isso **3 a 5 dias antes do final do mês**, para que você consiga concluir tudo ainda dentro do mesmo ciclo.

#### **Etapa 2: Cliente faz o cadastro incorporado com você**

1. Peça que o cliente **acesse seu fluxo de cadastro incorporado** (associar um número na configuração do agente no Amigo Flow).
2.  Ele deve **selecionar a WABA existente** quando o sistema mostrar a mensagem:

    > “Esta Conta do WhatsApp Business foi compartilhada anteriormente.”
3. O cliente **não precisa escolher novamente o número de telefone** — apenas confirmar a WABA.
4. Ao finalizar, você já poderá receber os dados dessa sessão.



📆 **Exemplo de Cronograma**

| Data            | Ação                                                        | Situação do Cliente          |
| --------------- | ----------------------------------------------------------- | ---------------------------- |
| **20 de abril** | Cliente remove o parceiro antigo                            | Envio de mensagens bloqueado |
| **21 de abril** | Cliente faz cadastro incorporado e você compartilha crédito | Ainda bloqueado              |
| **1º de maio**  | Nova linha de crédito entra em vigor                        | Envio de mensagens liberado  |



### 🧠 **Resumo Final**

* A migração **não apaga** números nem modelos.
* O cliente **fica sem enviar mensagens por alguns dias** até o novo crédito entrar.
* Faça tudo **com antecedência** e **evite o início/fim do mês**.
* Após o primeiro dia do mês seguinte, **tudo volta a funcionar normalmente** com sua linha de crédito.

### Considerações finais

* É possível — e recomendado — **migrar o número de WABA**, mas **não é possível migrar o Portfólio Empresarial**.\
  O número continuará associado ao mesmo **Gerenciador de Negócios**.
* A **Meta não permite** migração de **conta empresarial**.\
  Se desejar mover o número para outra **Business Manager (BM)**, será necessário **desconectá-lo** da API Oficial e integrá-lo novamente como **um novo número**.
* Se o número estiver conectado a uma **URA (Unidade de Resposta Audível)**, **desative a URA** temporariamente para receber o código de verificação.





