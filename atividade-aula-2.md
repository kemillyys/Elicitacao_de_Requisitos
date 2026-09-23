# Atividade da aula 2 — Histórias de usuário e MoSCoW

**Contexto:** aplicativo de delivery de comida.

## 1. Acompanhar o pedido

**História de usuário:** Como cliente que já fez um pedido, quero consultar o andamento dele no aplicativo, para saber se o restaurante já começou o preparo e quando a entrega estiver a caminho.

**Critérios de aceitação:**

1. **Dado** que o cliente tem um pedido confirmado, **quando** abre os detalhes desse pedido, **então** o aplicativo mostra o status atual e o horário da última atualização.
2. **Dado** que o restaurante atualiza o pedido para “em preparo”, **quando** o cliente consulta os detalhes, **então** encontra o status “em preparo”.
3. **Dado** que o entregador retirou o pedido, **quando** o cliente consulta os detalhes, **então** encontra o status “a caminho”.

## 2. Informar item indisponível

**História de usuário:** Como responsável pelo restaurante, quero marcar um item do cardápio como indisponível, para evitar novos pedidos de algo que não posso preparar.

**Critérios de aceitação:**

1. **Dado** que o restaurante está autenticado e possui um item ativo, **quando** marca esse item como indisponível, **então** o item aparece como indisponível no cardápio dos clientes.
2. **Dado** que um item está indisponível, **quando** o cliente tenta adicioná-lo ao carrinho, **então** o aplicativo impede a adição e informa que o item não está disponível.
3. **Dado** que um item indisponível voltou ao estoque, **quando** o restaurante o marca como disponível, **então** os clientes podem adicioná-lo ao carrinho novamente.

## 3. Reportar problema na entrega

**História de usuário:** Como entregador com uma entrega em andamento, quero registrar um problema relacionado a ela, para que o suporte possa identificar a ocorrência e orientar a solução.

**Critérios de aceitação:**

1. **Dado** que o entregador tem uma entrega em andamento, **quando** acessa os detalhes da entrega, **então** encontra a opção “Reportar problema”.
2. **Dado** que o entregador selecionou um tipo de problema e escreveu a descrição, **quando** envia o relato, **então** o aplicativo registra a ocorrência vinculada à entrega e confirma o envio.
3. **Dado** que o entregador tenta enviar o relato sem escolher o tipo de problema, **quando** confirma o envio, **então** o aplicativo solicita essa informação e não registra uma ocorrência incompleta.

## Priorização MoSCoW

| Prioridade | História | Justificativa |
| --- | --- | --- |
| **Must have** | Informar item indisponível | Evita que novos clientes comprem um item que o restaurante não consegue entregar. |
| **Should have** | Acompanhar o pedido | Reduz a incerteza do cliente após a compra e facilita o acompanhamento, embora o pedido ainda possa ser processado sem essa tela. |
| **Could have** | Reportar problema na entrega | Organiza as ocorrências no próprio pedido. Em uma primeira versão, o entregador ainda pode contatar o suporte por um canal já existente. |

As três histórias têm um objetivo por perfil de usuário, para que possam ser detalhadas, estimadas e verificadas separadamente.
