# SmartFood Delivery

## Status do Projeto

🚧 Em desenvolvimento

\---

## Sobre o Projeto

O **SmartFood Delivery** é um sistema desktop de gerenciamento de pedidos de delivery, desenvolvido em Java com banco de dados MySQL. Ele permite o cadastro de clientes, produtos, entregadores e o registro completo de pedidos com acompanhamento de status.

\---

## Tecnologias Utilizadas

* **Java** (JDK 17+) — linguagem principal de programação
* **Java Swing** — interface gráfica desktop
* **MySQL** — banco de dados relacional
* **JDBC** — conexão Java com MySQL
* **MySQL Connector/J** — driver JDBC para MySQL
* **NetBeans IDE** — ambiente de desenvolvimento

\---

## Time de Desenvolvedores

|Nome|Função|
|-|-|
|Daniel Guerra|Desenvolvedor Full Stack|

\---

## Objetivo do Software

O SmartFood Delivery tem como objetivo centralizar e simplificar o gerenciamento de um serviço de delivery de alimentos, permitindo:

* Controle de cardápio com preços e disponibilidade
* Cadastro e consulta de clientes
* Registro e acompanhamento de pedidos em tempo real
* Gestão de entregadores e formas de pagamento

\---

## Funcionalidades do Sistema

### Módulo de Produtos (Cardápio)

* \[ ] Cadastrar novo produto com nome, descrição, preço e categoria
* \[ ] Listar todos os produtos do cardápio
* \[ ] Editar informações de um produto
* \[ ] Excluir produto do cardápio
* \[ ] Ativar/desativar disponibilidade de produto

### Módulo de Clientes

* \[ ] Cadastrar novo cliente
* \[ ] Listar clientes cadastrados
* \[ ] Editar dados do cliente
* \[ ] Excluir cliente
* \[ ] Buscar cliente por nome

### Módulo de Pedidos

* \[ ] Registrar novo pedido (vinculado a cliente, produto e forma de pagamento)
* \[ ] Listar pedidos com status atual
* \[ ] Alterar status do pedido (Em preparo → A caminho → Entregue)
* \[ ] Calcular total do pedido automaticamente

### Módulo de Entregadores

* \[ ] Cadastrar entregadores com veículo e disponibilidade
* \[ ] Gerenciar disponibilidade para atribuição de pedidos

\---

## Como Executar

### Pré-requisitos

1. Java JDK 17 ou superior instalado
2. MySQL Server rodando na porta 3306
3. MySQL Connector/J adicionado ao classpath do projeto

### Configuração do banco de dados

1. Execute o arquivo `smartfood\_delivery.sql` no MySQL Workbench
2. Abra o arquivo `src/smartfood/dao/ConexaoDB.java`
3. Ajuste a senha do MySQL na constante `SENHA`

### Executar o projeto

1. Abra o projeto no NetBeans IDE
2. Clique com o botão direito no projeto → Run
3. A tela principal do sistema será exibida

\---

## Estrutura do Projeto

```
SmartFoodDelivery/
├── src/
│   └── smartfood/
│       ├── Main.java
│       ├── model/
│       │   ├── Cliente.java
│       │   ├── Produto.java
│       │   ├── Pedido.java
│       │   ├── Entregador.java
│       │   ├── FormaPagamento.java
│       │   └── Usuario.java
│       ├── dao/
│       │   ├── ConexaoDB.java
│       │   ├── ClienteDAO.java
│       │   ├── ProdutoDAO.java
│       │   └── PedidoDAO.java
│       └── view/
│           ├── TelaPrincipal.java
│           ├── TelaProdutos.java
│           ├── TelaClientes.java
│           └── TelaPedidos.java
└── sql/
    └── smartfood\_delivery.sql
```
Projeto finalizado em abril/2026

