# Java EstacionaShon

## Descrição
O "EstacionaShon" é um sistema de gerenciamento de estacionamentos para diferentes sedes de uma faculdade. O sistema permite cadastrar veículos, controlar a entrada e saída de carros, e gerenciar as vagas disponíveis em cada sede. O Sistema foi criado com intuito educacional para que estudos sobre banco de dados modelagem e CRUD sejam feitos.

## Tecnologias Utilizadas
- Java SE 11+
- PostgreSQL 13+
- JDBC (Java Database Connectivity)
- Maven (futuramente)
  
## Funcionalidades
- Cadastro de veículos.
- Controle de entrada e saída dos veículos.
- Gestão de vagas por sede (Lourdes, Contagem, Barreiro, Betim, São Gabriel, Poços de Caldas).
- Cálculo de tempo de permanência e valor a ser pago.
  
## Pré-requisitos
- JDK 11+ (Java Development Kit)
- PostgreSQL 13+ instalado e configurado
- Maven (futuramente)
  
## Configuração do Ambiente
1. Clone este repositório: `https://github.com/GabrielLLucasD/estacionamentoJava.git`
2. Crie o banco de dados no PostgreSQL:
   ```sql
   CREATE DATABASE estacionashon;
## Estrutura do Banco de Dados

- **Motorista**: Armazena as informações do condutor.
  - `id` (PK)
  - `nome`
  - `matricula`
  - `documento` (CNH)
  - `telefone` 

- **Veículo**: Armazena informações sobre os veículos cadastrados e relaciona cada veículo a um motorista.
  - `id` (PK)
  - `placa`
  - `documento`
  - `modelo`
  - `cor`
  - `motorista_id` (FK para Motorista)

- **Estacionamento**: Armazena informações sobre as vagas disponíveis em cada sede.
  - `id` (PK)
  - `sede`
  - `vaga`
  - `status`

- **EntradaSaida**: Registra a entrada e saída de veículos no estacionamento.
  - `id` (PK)
  - `veiculo_id` (FK para Veículo)
  - `estacionamento_id` (FK para Estacionamento)
  - `hora_entrada`
  - `hora_saida`

## Como Usar
1. **Cadastrar um veículo**:
   - O usuário insere a placa, modelo e cor do veículo.
2. **Registrar a entrada de um veículo**:
   - O sistema registra a entrada e o horário de entrada.
3. **Registrar a saída de um veículo**:
   - O sistema calcula o tempo de permanência e gera o valor a ser cobrado.
## Melhorias Futuras
- Implementar interface gráfica com Java Swing.
- Adicionar autenticação de usuários (funcionários que gerenciam o estacionamento).
- Melhorar o relatório de histórico de veículos.
- Adicionar integração com APIs de pagamento para automatizar cobranças.
- Adicionar integração com API do detran para verificar o documento do veículo e CNH
## Contato
- Gabriel Lucas
  - email - gabriel2014.lucas@outlook.com
  - LinkedIn - https://www.linkedin.com/in/gabriel-lucas-b52620201/
