# Projeto CRUD de Alunos - FastAPI com PostgreSQL

Este projeto implementa um CRUD (Create, Read, Update, Delete) de Alunos usando FastAPI e PostgreSQL. O objetivo é gerenciar informações de alunos, como nome, email e ID, por meio de uma API RESTful. O projeto foi desenvolvido sem o uso de Pydantic.

## Funcionalidades

- **Criar Aluno**: Adicionar um novo aluno com nome e email.
- **Listar Aluno**: Buscar um aluno pelo ID.
- **Listar Alunos** Busca todos os alunos cadastrados.
- **Atualizar Aluno**: Atualizar o nome e o email de um aluno.
- **Deletar Aluno**: Remover um aluno pelo ID.

## Tecnologias Utilizadas

- **FastAPI**: Framework web de alta performance para construir APIs com Python. 
- **SQLAlchemy**: ORM para manipulação do banco de dados PostgreSQL.
- **PostgreSQL**: Banco de dados relacional utilizado.

## Requisitos

- Python 3.10+ (https://www.python.org/downloads/)
- PostgreSQL (https://www.postgresql.org/download/)
- FastAPI (https://fastapi.tiangolo.com/)
- SQLAlchemy (https://www.sqlalchemy.org/download.html)

   ## Estrutura do Projeto
    -   ├── alunocrud_postgres/
    -   │   ├── venv/                # Ambiente virtual
    -   │   ├── _init_.py
    -   │   ├── main.py              # Principal arquivo contendo a API
    -   │   ├── models.py            # Modelos para o banco de dados
    -   │   ├── crud.py              # Operações CRUD com o banco de dados
    -   │   ├── database.py          # Configuração relacionada ao banco de dados PostgreSQL


## Configuração do Ambiente

1. Navegue até o diretório do seu projeto

   ```bash
   cd seu-repositorio
   ```
   
2. Criação e ativação de um ambiente virtual:

   ```bash
   python -m venv .venv
   ```
   
Ativação no Linux/Mac:

  ```bash
  source .venv/bin/activate

  ```

Ativação no Windows:

  ```bash
  .venv\Scripts\activate

  ```

4. Instalação das dependências:

  ```bash
  pip install fastapi uvicorn sqlalchemy psycopg2

  ```

## Configuração do Banco de Dados

1. Crie um banco de dados PostgreSQL com o nome de sua preferência e configure as seguintes credenciais:

- **Usuário**: Seu nome de usuário
- **Senha**: Sua senha
- **Banco de dados**: Escolha um nome para o banco de dados

### Criando o banco de dados no PostgreSQL

Acesse o PostgreSQL:

  ```bash

  psql -U postgres

 ```

2. Crie o banco de dados:

 ```bash
CREATE DATABASE "Nome do seu DataBase";

 ```
3. Crie o Usuário e defina a Senha:

```bash
   CREATE USER "Seu Usuário" WITH PASSWORD "Sua Senha";
```

4. Conceda Permissões ao seu usuário:

```bash
GRANT ALL PRIVILEGES ON DATABASE "insira seu banco de dados aqui" TO usuario;
```

## Executando a Aplicação

1. Inicie o servidor FastAPI com o comando:

```bash
   uvicorn app.main:app --reload
```

2. Acesse o endereço no navegador:

```bash
  http://127.0.0.1:8000
```

3. Acesse a documentação da API (Swagger) pelo navegador:

```bash
   http://127.0.0.1:8000/docs
```

**Criar, Listar, Alterar, Deletar alunos**

É possivel realizar o CRUD via Swagger
   

   
