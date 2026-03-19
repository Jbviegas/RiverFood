# 🍔 RiverFood API

API desenvolvida com **NestJS** para gerenciamento de um sistema de pedidos de delivery(RiverFood), incluindo autenticação, usuários e estrutura modular escalável.

---

## 🚀 Tecnologias Utilizadas

* **Node.js**
* **NestJS**
* **TypeScript**
* **TypeORM**
* **MySQL / PostgreSQL**
* **JWT (Autenticação)**
* **Passport**
* **Swagger**


---

## 📁 Estrutura do Projeto

```
src/
├── auth/           # Autenticação (JWT, login, guards)
├── usuario/        # Módulo de usuários
├── cliente/        # Módulo de clientes
├── categoria/      # Módulo de categorias
├── produto/        # Módulo de produtos
└── main.ts         # Arquivo principal
```

---

## ⚙️ Configuração do Projeto

### 1. Clone o repositório

```bash
git clone <url-do-repositorio>
cd river-food
```

### 2. Instale as dependências

```bash
Instalação das Bibliotecas:

npm install @nestjs/typeorm@ typeorm@ mysql2 
npm instal class-validator class-transformer

instalação do passport em usuario

npm install --save @nestjs/passport passport passport-local

npm install --save-dev @types/passport-local

npm install --save @nestjs/jwt passport-jwt

npm install --save-dev @types/passport-jwt


Instalação das Bibliotecaspara fazer o Deploy:

Render
npm install --save @nestjs/config

PostgreSQL
npm install --save pg
```

### 3. Configure o banco de dados Local

 type: 'mysql',
      host: 'localhost',
      port: 3306,
      username: 'root',
      password: 'root',
      database: 'db_river_food',

JWT_SECRET=sua_chave_secreta

```

---

## ▶️ Executando o Projeto

```bash
npm run start:dev
```
---

## 🔐 Autenticação

A API utiliza **JWT (JSON Web Token)**.

### Fluxo:

1. Criar usuário
2. Fazer login
3. Receber token JWT
4. Enviar token no header:

```http
Authorization: Bearer seu_token_aqui
```

---

## 📌 Principais Funcionalidades

* ✅ Cadastro de usuários
* ✅ Autenticação com JWT
* ✅ CRUD de clientes
* ✅ CRUD de categorias
* ✅ CRUD de produtos
* ✅ Validação de dados (class-validator)
* ✅ Criptografia de senha (bcrypt)

---

## 📖 Documentação da API

A documentação está disponível no Github:

```
https://github.com/Grupo-03-Turma-JavaScript-13/Docs
```

---

## 🧹 Padrões Utilizados

* Arquitetura em camadas:

  * Controller → recebe requisições
  * Service → regras de negócio
  * Repository → acesso ao banco
* DTOs para validação
* Guards para autenticação

---

## ⚠️ Possíveis Problemas

### Erro de banco não encontrado

```
Unknown database 'db_river_food'
```

✔ Solução: Crie o banco manualmente:

```sql
CREATE DATABASE river_food;
```

---

# 👨‍💻 Autores

**Josue Viegas**, **Lívia Campos**, **Evelyn Lamarca**, **Matheus Moura**, **Erick Santana**, **Renan Ferreira**


---

# 📄 Licença

Este projeto é destinado a **fins educacionais e portfólio**.
---
