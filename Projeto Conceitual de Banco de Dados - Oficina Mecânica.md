# Desafio 2: Projeto Conceitual de Banco de Dados - Oficina Mecânica

## 🎯 Objetivo do Desafio
Este projeto foi desenvolvido como parte do bootcamp para construir um **esquema conceitual de banco de dados** para um sistema de controle e gerenciamento de ordens de serviço em uma oficina mecânica. O desafio consistiu em criar as entidades, relacionamentos e atributos necessários para gerenciar informações sobre clientes, veículos, serviços, mecânicos e ordens de serviço (OS).

## 🔧 Tecnologias Utilizadas
- **MySQL Workbench**: Utilizado para modelar e criar o banco de dados MySQL, definindo tabelas, relacionamentos e consultas.
- **SQL**: Linguagem utilizada para definir as entidades, realizar as manipulações de dados e calcular valores de serviços.

## 🛠️ Estrutura do Projeto
O projeto é composto pelos seguintes elementos principais:
- **Entidades**:
  - **Cliente**: Contém as informações sobre o cliente, como nome, endereço e telefone.
  - **Veículo**: Informações sobre os veículos dos clientes, como marca, modelo, ano e tipo de serviço solicitado.
  - **Ordem de Serviço (OS)**: Cada OS é vinculada a um veículo e contém o número da ordem, data de emissão, valor total (mão-de-obra + peças), status e data para conclusão.
  - **Mecânico**: Contém dados sobre os mecânicos, como código, nome, endereço e especialidade.
  - **Peça**: Informações sobre as peças necessárias para os serviços, incluindo nome e valor.
  - **Tabela de Mão-de-Obra**: Contém valores de referência de mão-de-obra para diferentes tipos de serviço.

- **Relacionamentos**:
  - **Cliente - Veículo**: Um cliente pode ter vários veículos, mas cada veículo pertence a um único cliente.
  - **Veículo - Ordem de Serviço (OS)**: Cada veículo pode ter várias ordens de serviço associadas.
  - **Ordem de Serviço - Mecânico**: Cada ordem de serviço pode ser atribuída a uma equipe de mecânicos, que a avalia e executa.
  - **Ordem de Serviço - Peça**: A OS pode incluir várias peças necessárias para o serviço.
  - **Ordem de Serviço - Tabela de Mão-de-Obra**: Cada serviço possui um valor calculado de acordo com a tabela de referência de mão-de-obra.

## 📝 Diagrama ER
Este esquema foi desenvolvido com base na narrativa fornecida, levando em consideração a necessidade de controle detalhado sobre os **clientes**, os **veículos** que eles possuem, as **ordens de serviço** geradas para manutenção, as **equipes de mecânicos** responsáveis pelos serviços, e os **custos de peças e mão-de-obra**. O modelo busca refletir o fluxo de informações que ocorre dentro de uma oficina mecânica, desde a entrada do veículo até a conclusão do serviço e o pagamento final.

![Oficina Mecânica](https://github.com/user-attachments/assets/1fca00e0-f2a5-4021-a6e8-17a45efbf0b5)
