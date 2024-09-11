
# in.orbit

Este projeto foi desenvolvido durante o evento NLW Pocket da Rocketseat. A aplicação de metas permite aos usuários criar, gerenciar e acompanhar suas metas, incluindo a visualização de metas pendentes e a marcação de metas concluídas.


## Stack utilizada

**Back-end:** 
- Node.js com Fastify para criação e gerenciamento do servidor.
- Zod para validação de dados.
- Drizzle ORM para mapeamento de dados e operações com o banco de dados.
- Docker Compose para orquestração de containers.
- Criação de schemas e seed do banco de dados.


## Documentação da API

#### Cria uma meta

```http
  POST /goals
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `title` | `string` | título |
| `desiredWeeklyFrequency` | `number` | Frequência de dias da meta |



#### Cria uma meta atingida

```http
  POST /completions
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `goalId` | `string` | Id da meta |

#### Retorna o resumo de metas

```http
  GET /summary
```

#### Retorna as metas pendentes

```http
  GET /pending-goals
```

## Funcionalidades

- Criação de metas.
- Exibição de metas pendentes.
- Marcação de metas como concluídas.
- Conexão com a API para atualização em tempo real.


## Referência

 - [Rocketseat](https://rocketseat.com.br)
