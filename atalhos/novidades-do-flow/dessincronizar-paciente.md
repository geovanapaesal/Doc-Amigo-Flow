# Dessincronizar Paciente

#### O que é

Agora é possível desfazer a sincronização entre um contato do WhatsApp e um cadastro de paciente diretamente pela interface do Amigo Flow, sem precisar acessar o sistema de prontuário ou acionar o suporte.

#### Por que isso importa

Erros de sincronização acontecem — um atendente pode vincular o contato à pessoa errada no momento de pressão do atendimento. Antes, corrigir esse erro era manual, incompleto e muitas vezes deixava dados residuais no sistema. Agora o processo é direto, rastreável e limpo.

#### Como usar

1. Abra o **Amigo Flow** e acesse o chat do contato que foi sincronizado indevidamente.
2. No painel lateral, clique em **Detalhes do Contato**.
3. Ao lado do nome do paciente sincronizado, clique no ícone de **três pontos (⋯)**.
4. Selecione a opção **"Dessincronizar paciente"**.
5.  Um modal de confirmação será exibido com a seguinte informação:

    > _"Tem certeza que deseja desfazer a sincronização? O contato será desvinculado do paciente **\[Nome do Paciente]** e o número de telefone será removido do cadastro deste paciente."_
6. Confirme a ação clicando em **"Dessincronizar"**.

#### O que acontece após a dessincronização

| O que muda               | Resultado                                                           |
| ------------------------ | ------------------------------------------------------------------- |
| **Meus Chats**           | O nome exibido volta a ser o nome do contato registrado no WhatsApp |
| **Cadastro do paciente** | O número de telefone é removido do cadastro                         |
| **Lista de Leads**       | O contato retorna à fila de Leads                                   |
| **Botão de Sincronizar** | Reaparece nos Detalhes do Contato, disponível para um novo vínculo  |
| **Log de auditoria**     | A ação é registrada na linha do tempo do chat                       |

> ⚠️ **Atenção:** Se o paciente tinha mais de um cadastro e estava unificado por conta da sincronização, ele voltará a aparecer como duplicado após a dessincronização. Nenhum dado dos outros contatos é afetado.

#### Perfis com acesso

Qualquer atendente com acesso ao chat do contato pode realizar a dessincronização. Não é necessária permissão de administrador.

#### Perguntas frequentes

**O que acontece com o histórico de conversas?** O histórico permanece intacto. Apenas o vínculo com o paciente é desfeito — as mensagens continuam acessíveis.

**Posso ressincronizar depois?** Sim. O botão "Sincronizar" estará disponível novamente nos Detalhes do Contato após a dessincronização.

**A ação pode ser desfeita?** Não automaticamente. Uma vez dessincronizado, o vínculo precisa ser refeito manualmente via "Sincronizar".

### Notas para Implantadores

#### Dessincronizar Paciente

Nenhuma configuração adicional é necessária. A funcionalidade é habilitada por padrão para todos os atendentes com acesso ao módulo de Chat.

**Atenção ao comportamento de duplicidade:** em clínicas que utilizam unificação de pacientes, oriente as equipes sobre o comportamento esperado após a dessincronização (retorno à duplicidade pré-existente).

