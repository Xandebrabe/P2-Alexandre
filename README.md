# 20232BSET03P2
Inteli - Engenharia de Software | Avaliação 2023-2B P2

## Vulnerabilidades Identificadas e Medidas Adotadas:
### SQL Injection:
#### Vulnerabilidade 

O código provido utilizava interpolação de strings diretamente em comandos SQL, o que poderia permitir injeção de SQL.

#### Tratamento aplicado:

 Modificação das consultas SQL para usar parâmetros preparados, evitando assim a injeção de SQL.

### Validação de Entrada Insuficiente:
#### Vulnerabilidade:

Não havia validação suficiente para os parâmetros de entrada, como `animalType` e `id`.

#### Tratamento Aplicado:

Adição de validação para garantir que os parâmetros de entrada sejam adequados antes de executar operações no banco de dados.

### Tratamento Inadequado de Erros:
#### Vulnerabilidade:

O tratamento de erros original era limitado e poderia expor detalhes de implementação ao cliente.

#### Tratamento aplicado:

Refatoração do tratamento de erros para fornecer mensagens padrões, sem vazar detalhes sensíveis da implementação.

