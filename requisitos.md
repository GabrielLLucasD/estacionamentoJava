# Requisitos Funcionais (RFs) e Não Funcionais (RNFs)

Este documento descreve os requisitos funcionais e não funcionais que o sistema de gerenciamento de estacionamento deve atender.

## Requisitos Funcionais (RFs)

- **RF01 - Cadastro de Motoristas**: O sistema deve permitir o cadastro de motoristas com as seguintes informações:
  - **Nome**: Nome completo do motorista.
  - **Matricula**: Matricula do Aluno na instituição
  - **Documento**: Documento de identificação do motorista (CNH).
  - **Telefone**: Número de telefone de contato.

- **RF02 - Cadastro de Veículos**: O sistema deve permitir o cadastro de veículos com as seguintes informações e associá-los a motoristas:
  - **Placa**: Placa do veículo.
  - **Modelo**: Modelo do veículo.
  - **Documento**: Documento do Veículo.
  - **Cor**: Cor do veículo.
  - **Motorista**: Identificação do motorista ao qual o veículo está associado (relacionado ao cadastro de motoristas).

- **RF03 - Registro de Entrada e Saída**: O sistema deve registrar as entradas e saídas dos veículos no estacionamento, com os seguintes detalhes:
  - **Horário de Entrada**: Registro do horário em que o veículo entra no estacionamento.
  - **Horário de Saída**: Registro do horário em que o veículo sai do estacionamento.
  - **Sede**: Sede específica do estacionamento onde o veículo está localizado.

- **RF04 - Consulta de Vagas**: O sistema deve permitir a consulta da quantidade de vagas disponíveis e ocupadas em cada sede, fornecendo:
  - **Número de Vagas Livres**: Quantidade de vagas atualmente livres em uma sede.
  - **Número de Vagas Ocupadas**: Quantidade de vagas atualmente ocupadas em uma sede.

- **RF05 - Geração de Relatórios**: O sistema deve gerar relatórios com o histórico de entradas e saídas de veículos, incluindo:
  - **Data e Hora**: Registro da data e hora de cada entrada e saída.
  - **Veículo**: Informações do veículo que entrou ou saiu.
  - **Motorista**: Informações do motorista associado ao veículo.
  - **Sede**: Localização da vaga no estacionamento.

## Requisitos Não Funcionais (RNFs)

- **RNF01 - Desempenho**: O sistema deve responder a consultas em menos de 2 segundos, garantindo eficiência nas operações.

- **RNF02 - Integridade e Consistência**: O banco de dados deve garantir integridade e consistência nas operações, mesmo com múltiplos acessos simultâneos, prevenindo erros e corrupções de dados.

- **RNF03 - Tecnologias**: O sistema deve ser desenvolvido em Java e utilizar PostgreSQL como banco de dados, assegurando uma base tecnológica sólida.

- **RNF04 - Escalabilidade**: O sistema deve ser escalável, permitindo a inclusão de novas sedes no futuro sem a necessidade de grandes alterações na estrutura existente.

- **RNF05 - Usabilidade**: A interface de uso (CLI ou GUI) deve ser simples e intuitiva para os operadores, garantindo uma experiência de usuário eficiente e agradável.

