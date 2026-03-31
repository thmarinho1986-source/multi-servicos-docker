# 🐳 Multi-Serviços com Docker Compose

## 📋 Descrição

Este projeto demonstra a criação de um ambiente com múltiplos serviços utilizando **Docker Compose**, integrando dois tipos de bancos de dados:

* 🟢 **MongoDB (NoSQL)**
* 🔵 **MySQL (Relacional)**

O objetivo é aplicar conceitos de **containerização, redes Docker e persistência de dados**, comuns em arquiteturas modernas.

---

## 🧱 Arquitetura do Projeto

* 2 containers independentes
* 1 rede compartilhada (bridge)
* Volumes para persistência de dados

---

## 🚀 Como executar

```bash
docker compose up -d
```

---

## 🔎 Verificar containers

```bash
docker ps
```

---

## 🗄️ Serviços

### 🟢 MongoDB

* Host: localhost
* Porta: 27017
* Usuário: admin
* Senha: admin123

---

### 🔵 MySQL

* Host: localhost
* Porta: 3307
* Usuário: user
* Senha: user123
* Banco: app_db

---

## 🌐 Rede

Os containers utilizam uma rede personalizada:

```text
app_network
```

Permitindo comunicação entre serviços.

---

## 💾 Persistência de dados

Volumes utilizados:

* mongo_data
* mysql_data

Mesmo após parar os containers, os dados permanecem.

---

## 🧪 Testes realizados

✔️ Inicialização dos containers
✔️ Conexão com MongoDB
✔️ Conexão com MySQL
✔️ Teste de persistência de dados

---

## 🧠 Conceitos aplicados

* Docker
* Docker Compose
* Banco de dados relacional e não relacional
* Redes Docker
* Volumes (persistência)
* WSL 2

---

## 📸 Demonstração

### 🐳 Containers em execução
![Docker](assets/docker-ps.png)

### 🔵 MySQL funcionando
![MySQL](assets/mysql.png)

### 🟢 MongoDB funcionando
![MongoDB](assets/mongo.png)

## 👨‍💻 Autor

Aluno: Thiago Marinho
Matrícula: 202322140
