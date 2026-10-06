MER - Confeitaria da Neide
1- Entidades

    Cliente: Quem compra na padaria.

    Produto: Doces, pães, bolos e salgados do catálogo.

    Pedido: As encomendas/compras realizadas.

2- Atributos

    Cliente:

        id_cliente (PK - Primary Key)

        nome

        telefone

        endereco

    Produto:

        id_produto (PK - Primary Key)

        nome

        categoria (Ex: "Bolos", "Pães", "Salgados")

        preco

    Pedido:

        id_pedido (PK - Primary Key)

        data_entrega

        valor_total

        status (Ex: "Recebido", "Em Produção", "Entregue")

        id_cliente (FK - Foreign Key)

        id_produto (FK - Foreign Key)

3-Relacionamentos

    Cliente -> Pedido: 1 Cliente faz 1 ou vários Pedidos (1:N).

    Pedido -> Produto: 1 Pedido contém 1 ou vários Produtos (1:N).