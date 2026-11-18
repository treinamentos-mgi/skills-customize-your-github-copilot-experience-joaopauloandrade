# 📘 Atividade: Construindo APIs REST com FastAPI

## 🎯 Objetivo

Aprenda os fundamentos de APIs REST usando o framework FastAPI em Python. Ao final, você terá criado uma API para consultar, cadastrar, atualizar e remover tarefas, com validação dos dados e respostas HTTP adequadas.

## 📝 Tarefas

### 🛠️ Criar a aplicação e consultar tarefas

#### Descrição
Configure uma aplicação FastAPI e crie endpoints para verificar se a API está funcionando e consultar as tarefas cadastradas. Use uma lista em memória para armazenar os dados durante a execução.

#### Requisitos
O programa concluído deve:

- Criar uma aplicação FastAPI que possa ser iniciada localmente.
- Implementar `GET /` ou `GET /health` para retornar uma confirmação de que a API está disponível.
- Implementar `GET /tasks` para retornar a lista de tarefas, inicialmente vazia.
- Expor a documentação interativa gerada pelo FastAPI.

### 🛠️ Adicionar e buscar tarefas

#### Descrição
Permita que clientes da API cadastrem tarefas e consultem uma tarefa específica pelo seu identificador.

#### Requisitos
O programa concluído deve:

- Implementar `POST /tasks` para cadastrar uma tarefa com título e descrição.
- Atribuir um identificador único a cada tarefa criada.
- Implementar `GET /tasks/{task_id}` para buscar uma tarefa pelo identificador.
- Retornar a tarefa criada ou encontrada em formato JSON.

### 🛠️ Atualizar e remover tarefas com validação

#### Descrição
Complete as operações da API permitindo atualizar e remover tarefas. Valide os dados recebidos e informe corretamente o resultado de cada operação por meio dos códigos de status HTTP.

#### Requisitos
O programa concluído deve:

- Implementar `PUT /tasks/{task_id}` para atualizar uma tarefa existente.
- Implementar `DELETE /tasks/{task_id}` para remover uma tarefa existente.
- Validar os campos recebidos usando modelos do Pydantic.
- Retornar um código de sucesso apropriado para cada operação e `404 Not Found` quando o identificador não existir.
