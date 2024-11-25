# Desafio DIO - Refinando um Projeto Conceitual de Banco de Dados – E-COMMERCE

# Banco de Dados de E-Commerce

Este projeto implementa um banco de dados relacional para um sistema de e-commerce. O banco foi projetado para gerenciar informações de clientes, produtos, fornecedores, pedidos, pagamentos e estoque.

## Estrutura do Banco de Dados

### Entidades Principais

1. **Cliente**
   - Cadastro de clientes PF (Pessoa Física) ou PJ (Pessoa Jurídica).
   - Inclui CPF/CNPJ, endereço, telefone e e-mail.

2. **Produto**
   - Informações sobre produtos disponíveis para venda.
   - Cada produto é fornecido por um único fornecedor.

3. **Fornecedor**
   - Registro de fornecedores com nome, contato e informações de comunicação.

4. **Estoque**
   - Controle da quantidade de produtos disponíveis.

5. **Pedido**
   - Registra pedidos feitos pelos clientes.
   - Inclui status, código de rastreamento, endereço de entrega e prazo para devolução.

6. **Pagamento**
   - Permite o cadastro de múltiplas formas de pagamento (cartão, boleto, Pix, etc.).
   - Associa o pagamento aos pedidos realizados.

7. **ItemPedido**
   - Relaciona os produtos aos pedidos, registrando a quantidade e o valor total.

### Relacionamentos

- Um cliente pode realizar vários pedidos.
- Um pedido pode conter vários produtos.
- Cada produto possui apenas um fornecedor.
- Um pedido pode ter múltiplas formas de pagamento.

## Como Executar o Script

1. Certifique-se de ter o MySQL instalado.
2. Crie o banco de dados:
   ```sql
   CREATE DATABASE ECommerce;
