# Desafio 1: Projeto Conceitual de Banco de Dados - E-COMMERCE

Este projeto foi desenvolvido como parte do bootcamp para aprimorar habilidades de modelagem de dados, com foco em um sistema de cadastro de clientes e processos de pagamento e entrega. O desafio consistiu em refinar um modelo de dados para atender a requisitos específicos, como a distinção entre clientes **PJ (Pessoa Jurídica)** e **PF (Pessoa Física)**, a gestão de múltiplas formas de pagamento e o rastreamento de entregas.

## 🎯 Objetivo do Desafio
Refinar e expandir o modelo de dados fornecido, atendendo aos seguintes requisitos:
- **Cliente PJ e PF**: Uma conta pode ser PJ ou PF, mas não pode ter ambas as informações. Isso foi implementado de maneira que cada cliente tenha um único tipo de cadastro.
- **Formas de Pagamento**: Um cliente pode ter várias formas de pagamento cadastradas. O modelo foi ajustado para suportar múltiplos registros de pagamento para cada cliente.
- **Entrega**: A entrega deve ter um **status** (ex: "Em andamento", "Concluída", "Cancelada") e um **código de rastreio** para monitoramento. O modelo de dados foi ajustado para incluir essas informações.

## 🔧 Tecnologias Utilizadas
- **MySQL Workbench**: Ferramenta usada para modelar e gerenciar o banco de dados MySQL. Utilizada para criar o esquema, estruturar as tabelas e realizar as manipulações de dados.
- **SQL**: Linguagem utilizada para criar as tabelas e realizar as manipulações no banco de dados.
- **Diagrama ER**: Representação visual do modelo de dados no MySQL Workbench, facilitando o entendimento dos relacionamentos entre as tabelas.

## 🛠️ Estrutura do Projeto
O projeto é composto pelos seguintes elementos principais:
- **Esquema de Banco de Dados**: Modelagem relacional que define as tabelas, relacionamentos e restrições entre elas.
- **Tabelas**:
  - **Cliente**: Armazena as informações básicas sobre o cliente, diferenciando entre **PJ** e **PF**.
  - **Pagamento**: Registra múltiplas formas de pagamento associadas a cada cliente.
  - **Entrega**: Contém informações sobre o status da entrega e o código de rastreio.
  
- **Relacionamentos**:
  - Um cliente pode ter **múltiplos pagamentos**, mas cada pagamento está associado a um único cliente.
  - Cada entrega está vinculada a um único cliente, com informações de status e rastreio.

## 📊 Diagrama ER
O modelo foi desenhado de forma a otimizar o desempenho das consultas e garantir a integridade dos dados. Abaixo, estão as principais tabelas e seus relacionamentos:
- **Cliente**: Contém os dados de cadastro, com um campo para identificar se o cliente é PJ ou PF.
- **Pagamento**: Tabela associada ao cliente, com campo para diferentes métodos de pagamento (cartão, boleto, etc.).
- **Entrega**: Relacionamento entre o cliente e a entrega, com status e código de rastreio.

![E-COMMERCE](https://github.com/user-attachments/assets/81876ade-dd61-41b7-bb61-ea74e1e2d0d1)
