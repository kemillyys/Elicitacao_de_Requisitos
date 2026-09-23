# Atividade da aula 3 — Requisitos não funcionais

**Contexto:** aplicativo de delivery de comida. Cada história abaixo recebeu três requisitos não funcionais (RNF), com sua característica de qualidade correspondente na **ISO/IEC 25010:2023**. Os limites numéricos são metas propostas para o exercício e podem ser ajustados com a equipe.

## História 1 — Avaliar o pedido

> Como cliente, quero avaliar o pedido depois da entrega, para ajudar outros clientes a escolherem melhor.

| ID | Requisito não funcional | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-01 | A tela de avaliações do restaurante deve carregar em até 2 segundos em pelo menos 95% das consultas, considerando uma conexão de 10 Mb/s e até 100 avaliações exibidas. | Eficiência de desempenho |
| RNF-02 | O sistema deve permitir o envio de uma avaliação somente pela conta vinculada ao pedido entregue e impedir que outra conta a altere. | Segurança |
| RNF-03 | O formulário de avaliação deve permitir navegar pelos campos, selecionar a nota e enviar o comentário usando apenas o teclado. | Capacidade de interação |

## História 2 — Salvar um cartão

> Como cliente, quero salvar um cartão de pagamento, para não digitar os dados a cada compra.

| ID | Requisito não funcional | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-04 | O aplicativo não deve armazenar o número completo nem o código de segurança do cartão nos seus registros ou logs; deve guardar apenas a referência protegida fornecida pelo serviço de pagamento. | Segurança |
| RNF-05 | A lista de cartões salvos deve estar disponível em pelo menos 99,9% do tempo em cada mês, desconsiderando períodos de manutenção previamente comunicados. | Confiabilidade |
| RNF-06 | Durante a escolha do cartão, a interface deve identificar cada opção pela bandeira e pelos quatro últimos dígitos, sem expor os demais números. | Capacidade de interação |

## História 3 — Consultar o resumo de vendas

> Como dono de restaurante, quero ver um resumo diário de vendas, para acompanhar o desempenho do dia.

| ID | Requisito não funcional | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-07 | Para períodos de até 90 dias e até 10 mil pedidos, o painel deve apresentar o resumo em até 3 segundos em pelo menos 95% das consultas. | Eficiência de desempenho |
| RNF-08 | Após uma falha durante o processamento do resumo, os registros de pedidos já confirmados devem permanecer íntegros, sem duplicação ou perda. | Confiabilidade |
| RNF-09 | Os dados de vendas devem ser exibidos somente para contas autorizadas do respectivo restaurante. | Segurança |

**Referência do modelo de qualidade:** [ISO/IEC 25010:2023 — Product quality model](https://www.iso.org/standard/78176.html).
