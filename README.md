Este é um projeto conceitual de banco de dados relacionado ao sistema de e-commerce, no qual o desafio proposto foi refinado acrescentando os seguintes pontos:

Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
Entrega – Possui status e código de rastreio.

Cliente PJ e PF: dadas as condições achei pertinentes criar uma instância dentro da entidade “Cliente” do tipo INT, afim de verificar se aquela conta cadastrada pertence a uma pessoa física ou jurídica; 
Pagamento: Visto que será permitida a utilização de mais de uma forma de pagamento, criei a entidade "Forma de Pagamento atrelada a entidade "Cliente" com um relacionamento 1:1. A entidade "Forma de Pagamento" também foi relacionada à entidade "Pedido " com o tipo N:N, considerando que o cliente pode ter mais de uma forma de pagamento e, também, mais de um pedido. 
Entrega: Foi criada uma entidade nomeada "Entrega" e atrelada a entidade "Pedido" com um relacionamento 1:1 pois cada entrega é apenas relacionada a um pedido.
