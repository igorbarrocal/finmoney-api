# FinMoney API

API REST para gerenciamento financeiro pessoal, desenvolvida com Spring Boot.

## Funcionalidades

- Cadastro e autenticação de usuários (JWT)
- Gerenciamento de categorias de despesas/receitas
- CRUD de transações financeiras
- Filtros avançados para busca de transações
- Dashboard com análise de despesas via IA (OpenAI/Groq)
- Documentação automática via Swagger/OpenAPI
- Suporte a múltiplos bancos de dados (H2 para dev, Oracle para produção)
- Validação e tratamento de erros

## Tecnologias

- Java 17
- Spring Boot 3
- Spring Security
- Spring Data JPA
- Lombok
- H2 Database (dev)
- Oracle Database (prod)
- Swagger/OpenAPI
- JWT (Auth0)
- Spring AI

## Como executar

1. Clone o repositório:
   ```sh
   git clone https://github.com/igorbarrocal/finmoney-api.git
   cd finmoney-api
   ```

2. Configure as variáveis de ambiente em `src/main/resources/application.properties` e `application-prod.properties`.

3. Execute o projeto:
   ```sh
   ./mvnw spring-boot:run
   ```

4. Acesse a documentação Swagger em:  
   [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

## Endpoints principais

- `/login` - Autenticação JWT
- `/categories` - Gerenciamento de categorias
- `/transactions` - Gerenciamento de transações
- `/dashboard` - Análise de despesas via IA

## Testes

Execute os testes com:
```sh
./mvnw test
```

## Licença

Este projeto está sob a licença Apache 2.0.