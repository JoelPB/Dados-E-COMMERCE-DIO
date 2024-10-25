## Desafio de projeto da DIO [Refinando um Projeto Conceitual de Banco de Dados – E-COMMERCE](https://web.dio.me/lab/refinando-um-projeto-conceitual-de-banco-de-dados-e-commerce/learning/0491dff0-c197-421f-af79-daa4933dfa38?back=/track/coding-future-suzano-analise-dados)

---

## Foi refinado o modelo apresentado acrescentando os seguintes tabelas:
1 Cliente-PJ
* Armazena dados de clientes pessoa jurídica (PJ), relacionados à tabela Cliente.

* Colunas: idCliente (FK, referência a Cliente), CNPJ

2 Cliente-PF
* Armazena dados de clientes pessoa física (PF), relacionados à tabela Cliente.

* Colunas: idCliente (FK, referência a Cliente), CPF

3 Pagamento
* Permite que um pedido tenha várias formas de pagamento.

* Colunas: idPagamento, FormaPagamento, Pedido_idPedido (FK), Pedido_Cliente_idCliente1 (FK), Pedido_Pagamento_idPagamento (FK)

4 Entrega
*  Armazena o status e o código de rastreio de uma entrega relacionada a um pedido.

* Colunas: idEntrega, StatusEntrega, CodigoRastreio, Pedido_idPedido (FK), Pedido_Cliente_idCliente1 (FK), Pedido_Pagamento_idPagamento (FK)
  
