# 📝 Elixir Todo List

**Nome do Aluno:** Ítalo José Silva Reis

**Link do Tutorial:** [Como Criar um App Todo List com Elixir e LiveView do Zero](https://profsergiocosta.notion.site/Como-Criar-um-App-Todo-List-com-Elixir-e-LiveView-do-Zero-2a8cce97509380eba53fc82bbeb08435)

## 📖 Descrição

Uma aplicação de gerenciamento de tarefas (Todo List) desenvolvida com **Phoenix Framework** e **LiveView**, demonstrando o poder da programação funcional com Elixir. O projeto utiliza comunicação em tempo real via WebSockets, persistência de dados com **Ecto** e uma interface moderna estilizada com **DaisyUI** e **Tailwind CSS**.

### 🚀 Tecnologias Utilizadas

- **Elixir** - Linguagem funcional para o backend
- **Phoenix Framework** - Framework web para Elixir
- **Phoenix LiveView** - Interatividade em tempo real sem JavaScript
- **Ecto** - ORM para persistência de dados
- **SQLite** - Banco de dados leve e embutido
- **DaisyUI** - Biblioteca de componentes para Tailwind CSS
- **Tailwind CSS** - Framework CSS utilitário

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- **Elixir** 1.14 ou superior ([Download](https://elixir-lang.org/install.html))
- **Erlang/OTP** 25 ou superior (geralmente instalado com Elixir)
- **Node.js** 18 ou superior ([Download](https://nodejs.org/))

> **Nota:** SQLite já vem embutido, não requer instalação separada.

### Verificando as instalações:

```powershell
elixir --version
node --version
```

## 🔧 Como Rodar

### 1. Clone o repositório

```powershell
git clone https://github.com/italojsr/elixir_todo_list.git
cd elixir_todo_list
```

### 2. Instale as dependências do Elixir

```powershell
mix deps.get
```

### 3. Crie e prepare o banco de dados

> **Nota:** Com SQLite, o banco de dados será criado automaticamente como um arquivo local.

```powershell
mix ecto.create
mix ecto.migrate
```

### 4. Instale as dependências do Node.js

```powershell
cd assets
npm install
cd ..
```

### 5. Inicie o servidor Phoenix

```powershell
mix phx.server
```

Ou para abrir automaticamente o navegador e ter um console interativo:

```powershell
iex -S mix phx.server
```

### 6. Acesse a aplicação

Abra seu navegador e acesse: [http://localhost:4000](http://localhost:4000)

## 🎯 Funcionalidades

- ✅ Adicionar novas tarefas
- ✅ Marcar tarefas como concluídas/pendentes
- ✅ Editar tarefas existentes
- ✅ Excluir tarefas
- ✅ Filtrar tarefas (Todas, Ativas, Concluídas)
- ✅ Atualização em tempo real sem recarregar a página
- ✅ Persistência de dados no SQLite

## 📁 Estrutura do Projeto

```
elixir_todo_list/
├── lib/
│   ├── elixir_todo_list/           # Contextos e schemas
│   │   ├── tasks/                  # Contexto de tarefas
│   │   └── repo.ex                 # Configuração do Ecto
│   └── elixir_todo_list_web/       # Interface web
│       ├── live/                   # LiveViews
│       └── components/             # Componentes reutilizáveis
├── priv/
│   └── repo/migrations/            # Migrações do banco
├── assets/                         # CSS, JS e imagens
├── config/                         # Configurações
└── test/                           # Testes automatizados
```

## 🧪 Executando os Testes

```powershell
mix test
```

## 🛠️ Comandos Úteis

```powershell
# Abrir console interativo
iex -S mix

# Resetar o banco de dados
mix ecto.reset

# Ver rotas disponíveis
mix phx.routes

# Formatar código
mix format

# Verificar qualidade do código
mix precommit
```

## 📚 Aprendizados

Este projeto demonstra conceitos importantes de:

- Programação funcional com Elixir
- Gerenciamento de estado no servidor com LiveView
- Comunicação em tempo real via WebSockets
- CRUD completo com Ecto
- Pattern matching e imutabilidade
- Convenções do Phoenix Framework

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais.

## 📚 Recursos Adicionais

- [Phoenix Framework](https://www.phoenixframework.org/)
- [Phoenix LiveView](https://hexdocs.pm/phoenix_live_view)
- [Elixir Lang](https://elixir-lang.org/)
- [Ecto Documentation](https://hexdocs.pm/ecto)

---

