---
icon: square-whatsapp
---

# Como associar meu número do Whatsapp no Flow?

Para associar um número a um agente

O Embedded Signup é o fluxo oficial da Meta para conectar empresas ao WhatsApp Business API via BSP. Com ele, é possível criar uma nova WABA ou migrar uma existente.



#### Fluxo de Associação

1.  Na configuração do Amigo Flow, na configuração do agente, clicar em **Associar número**. Um pop-up será aberto e você deve selecionar a opção **Whatsapp Business API.**<br>

    <figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>
2. Realizar login na conta do Facebook com acesso ao Gerenciador de Negócios.\
   ![](<../../.gitbook/assets/image (18).png>)
3. Conceda permissões à Amigo Tech clicando em **Confirmar.**\
   ![](<../../.gitbook/assets/image (20).png>)
4. Cria ou seleciona um [Portfólio empresarial ](como-criar-um-portfolio-empresarial-meta-business-suite.md)existente
5. Cria ou seleciona uma WABA(conta do Whatsapp Business) existente
6. Adicione um número de telefone a ser conectado.
7. Realize a verificação do número via SMS/ligação.
8. Ao final, a tela é atualizada e o número é ativado no painel do Amigo Flow.

#### ⚠️ Cuidados Importantes

* Você precisa ser o administrador do Gerenciador de Negócios.
* O número **não pode estar ativo em outra WABA**. Caso esteja, primeiramente ele deve ser excluído da Waba atual, para depois ser colocado em outra.
* [Verificação em duas etapas](como-desativar-a-autenticacao-em-dois-fatores-2fa-no-portfolio-empresarial.md) **deve estar desativada** no número.

#### Acompanhamento da verificação do número

* Após finalizar a associação do número, você pode acompanhar os status da validação do seu novo número, que são divididas em 3 fases:
  * Verificação da empresa
  * Verificação da Conta Whatsapp Business (WABA)
  * Verificação do nome do número

Onde? No configurador do Amigo Flow:

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
Caso seu número já esteja associado a um outro parceiro da Meta e precise realizar a migração, veja o módulo completo sobre [Migração de Números](como-fazer-a-portabilidade-de-um-numero-com-api-oficial-para-o-amigo-flow.md)
{% endhint %}
