## Modelagem de Banco de Dados

O banco de dados do sistema é composto pelas seguintes tabelas principais:

- **Motorista**:
  - `id`: Identificador único.
  - `nome`: Nome do Motorista.
  - `matricula`: Matricula de Aluno do Morotista
  - `documento`: CNH.
  - `telefone`: Telefone do Motorista.

- **Veículo**:
  - `id`: Identificador único.
  - `placa`: Placa do veículo.
  - `modelo`: Modelo do veículo.
  - `documento`: Documento do veículo.
  - `cor`: Cor do veículo.
  - `motorista_id`: Referência ao motorista.

- **Estacionamento**:
  - `id`: Identificador único.
  - `sede`: Nome da sede da faculdade.
  - `vaga`: Número da vaga.
  - `status`: Status (livre ou ocupada).

- **EntradaSaida**:
  - `id`: Identificador único.
  - `veiculo_id`: Referência ao veículo.
  - `estacionamento_id`: Referência ao estacionamento.
  - `hora_entrada`: Horário de entrada.
  - `hora_saida`: Horário de saída.
