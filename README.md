# API Gerenciador de Tarefas

Essa será uma aplicação para gerenciar tarefas (em inglês todos).

### Funcionalidades:

- [x] Criar um novo _todo_;
- [x] Listar todos os _todos_;
- [x] Alterar o `title` e `deadline` de um _todo_ existente;
- [x] Marcar um _todo_ como feito;
- [x] Excluir um _todo_;

Tudo isso para cada usuário em específico (o username será passado pelo header).

### Estruturação do Usuário:

- id: 'uuid' (v4)
- name: string
- username: string unique
- todos: todo[]

### Estruturaçaõ da Tarefa(todo):

- id: 'uuid' (v4)
- title: string
- done: boolean default = false
- deadline: date
  created_at: date

### Regras de negócio

- [x] Deve se possivel cadastrar um usuario.
- [x] Não deve se possivel cadastrar um usuario com o mesmo username.
- [x] Não deve se possivel atualizar uma `todo` com ID invalido.
- [x] Não deve se possivel marcar uma `todo` como `done` se o ID for invalido.
- [x] Para todas requisições de todo deve se verificado se o usuario é valido.

### Rodando o projeto

```
Puxe as dependencias
$ yarn

Rode o projeto
$ yarn dev
```
