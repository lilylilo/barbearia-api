# Barbearia Backend

Este é o backend de um sistema de agendamento para barbearias, desenvolvido com **Java 17** e **Spring Boot 3**.

## 🛠 Tecnologias Utilizadas
- Java 17
- Spring Boot 3
- Spring Data JPA
- PostgreSQL
- Spring Security com JWT
- OpenAPI (Swagger)
- Railway para deploy

## 📂 Estrutura do Projeto

```
📂 barbearia-api
 ┣ 📂 src/main/java/com/seuprojeto/barbearia
 ┃ ┣ 📂 config       # Configurações de segurança e CORS
 ┃ ┣ 📂 controller   # Endpoints REST
 ┃ ┣ 📂 dto          # Data Transfer Objects
 ┃ ┣ 📂 entity       # Entidades do banco de dados
 ┃ ┣ 📂 repository   # Interfaces JPA
 ┃ ┣ 📂 service      # Regras de negócio
 ┃ ┣ 📂 security     # Autenticação com JWT
 ┃ ┗ 📜 BarbeariaApplication.java  # Classe principal
 ┣ 📂 src/main/resources
 ┃ ┣ 📜 application.properties  # Configuração do banco de dados
 ┣ 📜 pom.xml  # Dependências do projeto
```

## 🚀 Como Rodar o Projeto

### 1️⃣ Clonar o Repositório
```bash
git clone https://github.com/seu-usuario/barbearia-api.git
cd barbearia-api
```

### 2️⃣ Configurar o Banco de Dados
No arquivo `application.properties`, configure seu banco de dados PostgreSQL:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/barbearia
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
```

### 3️⃣ Executar a Aplicação
```bash
mvn spring-boot:run
```
A API estará disponível em `http://localhost:8080`.

## 🔥 Endpoints Principais
- `POST /auth/login` – Login e geração de token JWT
- `POST /clientes` – Cadastro de cliente
- `GET /clientes` – Listar clientes
- `POST /agendamentos` – Criar um agendamento
- `GET /agendamentos` – Listar agendamentos
- `POST /servicos` – Criar um serviço

## 📝 Licença
Este projeto está sob a licença MIT.
