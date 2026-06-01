# 🍔 Stack Burgers

Projeto acadêmico desenvolvido para a disciplina de **Programação Orientada a Objetos**  
Curso: Análise e Desenvolvimento de Sistemas — 3º Semestre

---

## 📁 Estrutura do Repositório

| Pasta | Descrição |
|---|---|
| [`Backend`](./Backend) | API REST desenvolvida em Java com Spring Boot |
| [`Frontend`](./Frontend) | Interface web em HTML, CSS e JavaScript |

---

## 🚀 Como Rodar

### Pré-requisitos
- Java 17
- MySQL 8.0
- Maven

### 1. Clone o repositório
```
git clone https://github.com/DuduRick/stackburgers.git
cd stackburgers
```

### 2. Configure o banco de dados
Certifique-se de ter o MySQL rodando com usuário `root`.  
Se sua senha for diferente de `root`, edite o arquivo:
```
Backend/src/main/resources/application.properties
```

### 3. Rode o backend
```
cd Backend
mvn spring-boot:run
```

A API estará disponível em: `http://localhost:8080/api`

### 4. Rode o frontend
Abra o arquivo `Frontend/stack-burgers-FRONTv2.html` no navegador.

---

## 🛠️ Tecnologias

**Backend**
- Java 17
- Spring Boot 3.2
- Spring Data JPA
- MySQL 8.0
- Maven

**Frontend**
- HTML5
- CSS3
- JavaScript (React via CDN)

---

## 👥 Dados de Teste

| Tipo | E-mail | Senha |
|---|---|---|
| Cliente | cliente@demo.com | cliente123 |

> Os dados são inseridos automaticamente na primeira execução.
