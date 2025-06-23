# Trabalho III - Spring Security

## Como executar:

1. Execute a classe `TrabalhoIiiApplication.java`.
2. Acesse o console do H2: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)
   - JDBC URL: `jdbc:h2:mem:trabalho`
   - Username: `sa`
   - Password: (em branco)
3. Use HTTP Basic Authentication:
   - Usuário ADMIN: `admin` / `admin`
   - Usuário USER: `user` / `user`

## Endpoints disponíveis:

- GET `/transacao/cpf?valor={cpf}`
- GET `/transacao/nome?valor={nome}`
- PUT `/transacao/{id}` (ADMIN)
- DELETE `/transacao` (ADMIN)
- DELETE `/transacao/periodo` (ADMIN)

Consultas são liberadas para USER e ADMIN. Alterações e exclusões são apenas para ADMIN.
