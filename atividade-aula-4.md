# Atividade da aula 4 — Requisitos e fontes de informação

**Cenário:** a empresa vende produtos por telefone e em encontros presenciais. As fontes abaixo representam pessoas e materiais que eu consultaria para confirmar as regras antes de desenvolver o sistema; não são entrevistas já realizadas.

## Processo 1 — Vendedor registra pedidos

### RQ-01 — Cadastro do pedido

**Requisito:** O sistema deve permitir que o vendedor registre o cliente, os produtos, as quantidades e o canal da venda (telefone ou encontro presencial) em cada pedido.

- **Fonte 1:** Entrevista com vendedores que registram as vendas. **Humana**, nível **operacional**, classe de usuário **vendedor**.
- **Fonte 2:** Modelo atual de pedido ou formulário utilizado nas vendas. **Não humana**, categoria **documentação**.

### RQ-02 — Total do pedido

**Requisito:** O sistema deve calcular o valor total do pedido a partir das quantidades e dos preços cadastrados para os produtos selecionados.

- **Fonte 1:** Entrevista com a pessoa responsável por definir preços e regras comerciais. **Humana**, nível **tático**, classe de usuário **gestor comercial**.
- **Fonte 2:** Tabela de preços e política comercial da empresa. **Não humana**, categoria **documentação**.

### RQ-03 — Consulta após o registro

**Requisito:** Depois de confirmar um pedido, o sistema deve gerar um identificador e permitir que o vendedor consulte seus itens, valor total e situação.

- **Fonte 1:** Entrevista com vendedores sobre dúvidas e correções após a venda. **Humana**, nível **operacional**, classe de usuário **vendedor**.
- **Fonte 2:** Registros anteriores de pedidos e comprovantes utilizados pela empresa. **Não humana**, categoria **documentação**.

## Processo 2 — Administrador cadastra e remove produtos

### RQ-04 — Cadastro de produto

**Requisito:** O sistema deve permitir que o administrador cadastre um produto com nome, descrição, preço e identificação única.

- **Fonte 1:** Entrevista com o administrador responsável pelo catálogo. **Humana**, nível **tático**, classe de usuário **administrador**.
- **Fonte 2:** Catálogo ou planilha atual de produtos. **Não humana**, categoria **documentação**.

### RQ-05 — Edição do catálogo

**Requisito:** O sistema deve permitir que o administrador altere o nome, a descrição e o preço de um produto cadastrado.

- **Fonte 1:** Entrevista com o administrador sobre a rotina de atualização de preços. **Humana**, nível **tático**, classe de usuário **administrador**.
- **Fonte 2:** Histórico de tabelas de preços e alterações de produtos. **Não humana**, categoria **documentação**.

### RQ-06 — Remoção da oferta

**Requisito:** O sistema deve permitir que o administrador retire um produto de novas vendas, preservando seus dados nos pedidos já registrados.

- **Fonte 1:** Entrevista com o administrador sobre produtos descontinuados. **Humana**, nível **tático**, classe de usuário **administrador**.
- **Fonte 2:** Histórico de pedidos e regras de guarda de registros da empresa. **Não humana**, categoria **documentação**.

## Processo 3 — Equipe de estoque controla as quantidades

### RQ-07 — Registro de entrada

**Requisito:** O sistema deve permitir que a equipe de estoque registre a entrada de unidades de um produto, informando a quantidade e a data.

- **Fonte 1:** Observação e entrevista com a equipe que recebe mercadorias. **Humana**, nível **operacional**, classe de usuário **estoquista**.
- **Fonte 2:** Notas de recebimento e planilha de movimentação do estoque. **Não humana**, categoria **documentação**.

### RQ-08 — Registro de saída

**Requisito:** O sistema deve registrar a saída de unidades quando um pedido for confirmado e reduzir a quantidade disponível dos respectivos produtos.

- **Fonte 1:** Entrevista com a equipe responsável por separar pedidos. **Humana**, nível **operacional**, classe de usuário **estoquista**.
- **Fonte 2:** Registros de separação e expedição dos pedidos. **Não humana**, categoria **documentação**.

### RQ-09 — Consulta e limite de estoque

**Requisito:** O sistema deve mostrar a quantidade disponível de cada produto e impedir a confirmação de pedidos com quantidades superiores ao estoque disponível.

- **Fonte 1:** Entrevista com a equipe que confere a disponibilidade antes da venda. **Humana**, nível **operacional**, classe de usuário **estoquista**.
- **Fonte 2:** Procedimento de controle e conferência de estoque da empresa. **Não humana**, categoria **documentação**.
