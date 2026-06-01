# 🍔 Stack Burgers — Backend

API REST desenvolvida com Spring Boot para o sistema de pedidos da lanchonete Stack Burgers.

---

## 📋 Requisitos

Antes de rodar o projeto, certifique-se de ter instalado:

- [Java 17](https://www.oracle.com/java/technologies/javase/javase17-archive-downloads.html)
- [MySQL 8.0](https://dev.mysql.com/downloads/mysql/)
- [Maven](https://maven.apache.org/download.cgi) (ou use o Maven Wrapper incluído no projeto)

---

## ⚙️ Configuração do Banco de Dados

O projeto se conecta ao MySQL com as seguintes configurações padrão:

| Configuração | Valor padrão |
|---|---|
| Host | localhost |
| Porta | 3306 |
| Banco | stackburgers |
| Usuário | root |
| Senha | root |

> O banco de dados **stackburgers** é criado automaticamente na primeira execução.

### Se a sua senha do MySQL for diferente de `root`:

**Windows (Prompt de Comando):**
```
set DB_PASSWORD=suasenha
```

**Windows (PowerShell):**
```
$env:DB_PASSWORD="suasenha"
```

**Linux / Mac:**
```
export DB_PASSWORD=suasenha
```

---

## ▶️ Como Rodar

**1. Clone o repositório:**
```
git clone https://github.com/seu-usuario/stackburgers-backend.git
cd stackburgers-backend
```

**2. Execute o projeto:**
```
./mvnw spring-boot:run
```

Ou abra no IntelliJ IDEA e clique em **Run**.

**3. Acesse a API:**
```
http://localhost:8080/api
```

---

## 🌐 Principais Endpoints

| Método | Rota | Descrição |
|---|---|---|
| GET | /api/hamburgeres/disponiveis | Lista hambúrgueres disponíveis |
| GET | /api/bebidas/disponiveis | Lista bebidas disponíveis |
| POST | /api/clientes | Cadastra novo cliente |
| GET | /api/clientes | Lista todos os clientes |
| POST | /api/pedidos | Cria novo pedido |
| GET | /api/pedidos/cliente/{id} | Lista pedidos de um cliente |
| PATCH | /api/pedidos/{id}/status | Atualiza status do pedido |
| PATCH | /api/pedidos/{id}/cancelar | Cancela um pedido |

---

## 🗄️ Dados de Exemplo

Na primeira execução, o sistema carrega automaticamente:

- 4 hambúrgueres
- 4 bebidas
- 1 cliente de demonstração: `cliente@demo.com` / `cliente123`

---

## 🛠️ Tecnologias Utilizadas

- Java 17
- Spring Boot 3.2.0
- Spring Data JPA / Hibernate
- MySQL 8.0
- Lombok
- Maven

---

## 👨‍💻 Frontend

O frontend está disponível em um arquivo HTML único, sem necessidade de instalação.
Basta abrir o arquivo `index.html` no navegador com o backend rodando.
