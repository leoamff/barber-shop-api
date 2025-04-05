
# Barber Shop API

Este repositório contém a API RESTful para o sistema de gerenciamento da Barber Shop. Desenvolvido em Node.js com Express, o projeto permite o gerenciamento de clientes, serviços, agendamentos e usuários administrativos.

## 🚀 Tecnologias Utilizadas

- Node.js
- Express.js
- Sequelize ORM
- PostgreSQL
- JWT para autenticação
- Dotenv
- Cors

## 📁 Estrutura do Projeto

```
barber-shop-api/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   ├── config/
│   └── app.js
├── .env
├── .gitignore
├── package.json
└── README.md
```

## ⚙️ Funcionalidades

- ✅ Cadastro e autenticação de usuários
- ✂️ Gerenciamento de serviços (criação, edição, exclusão)
- 📅 Agendamento de horários
- 👥 Cadastro e listagem de clientes

## 🔐 Autenticação

A autenticação é baseada em JSON Web Tokens (JWT). Após o login, o token deve ser incluído no header das requisições protegidas.

## 🛠️ Como Rodar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/leoamff/barber-shop-api.git
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Configure o `.env` com as variáveis necessárias (exemplo abaixo):
   ```
   DB_HOST=localhost
   DB_USER=postgres
   DB_PASS=senha
   DB_NAME=barber_shop
   JWT_SECRET=seusegredoaqui
   ```

4. Execute as migrations e inicie o servidor:
   ```bash
   npx sequelize db:migrate
   npm run dev
   ```
