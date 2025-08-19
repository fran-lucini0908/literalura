# 📚 LiterAlura - Consumindo uma API de Livros
Projeto de uma aplicação desenvolvida com **Spring Boot** que roda via **terminal** e realiza o consumo da [API pública do Gutendex](https://gutendex.com/), permitindo buscar e armazenar informações de livros em um banco de dados **PostgreSQL**, utilizando **Spring Data JPA** para persistência.

# 🔧 Tecnologias Utilizadas
- Java 17+
- API Gutendex
- Spring Boot
- Spring Web
- Spring Data JPA
- PostgreSQL
- Maven

# 📖 Funcionalidades
- Buscar livro pelo título via API Gutendex
- Listar livros e autores cadastrados no banco de dados
- Filtrar autores por ano de nascimento/morte
- Buscar livros por idioma

# 🛠️ Como executar
1. 📥 Clone o repositório
   ```bash
   git clone git@github.com:mpbmarcio/challenge-literalura.git
   cd literalura
   mvn spring-boot:run
   ```
2. ⚙️ Configure o banco de dados no `application.properties`
   ```properties
   spring.application.name=literalura
   spring.datasource.url=jdbc:postgresql://${DB_HOST}/literalura
   spring.datasource.username=${DB_USER}
   spring.datasource.password=${DB_PASSWORD}
   spring.datasource.driver-class-name=org.postgresql.Driver
   hibernate.dialect=org.hibernate.dialect.HSQLDialect
   spring.jpa.hibernate.ddl-auto=update
   ```
