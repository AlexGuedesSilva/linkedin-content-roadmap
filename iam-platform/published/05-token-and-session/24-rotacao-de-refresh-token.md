# IAM Platform — 24 — Refresh Token Rotation

## Status

- [x] Ideia registrada
- [x] Conteúdo estudado
- [x] Roteiro definido
- [x] Imagem criada
- [x] Descrição criada
- [ ] Revisado
- [ ] Agendado
- [ ] Publicado

---

## Informações

- **Série:** IAM Platform
- **Número:** 24
- **Tema:** Refresh Token Rotation
- **Data de criação:** 29/07/2026
- **Data de publicação:**
- **Link da publicação:**
- **Branch ou feature relacionada:** `feature/refresh-token-rotation`

### Tecnologias relacionadas

- Java 17
- Spring Boot
- Spring Security
- JWT
- OAuth 2.0
- Refresh Token
- PostgreSQL
- Flyway
- Clean Architecture
- DDD
- Hexagonal Architecture

---

## Objetivo do post

Explicar o conceito de **Refresh Token Rotation** e demonstrar como essa estratégia fortalece a segurança do fluxo de autenticação ao invalidar o refresh token utilizado e emitir um novo token a cada renovação do access token.

Além do conceito, apresentar como essa prática foi implementada na IAM Platform utilizando **Clean Architecture**, **DDD**, sessões persistidas e armazenamento seguro apenas do hash do refresh token.

---

## Mensagem principal

**Um Refresh Token nunca deve ser reutilizado.**

A cada solicitação de renovação:

- o refresh token recebido é validado;
- o token utilizado é revogado;
- um novo Access Token é emitido;
- um novo Refresh Token é gerado;
- apenas o hash do novo refresh token é persistido;
- o novo token permanece vinculado à User Session.

Essa abordagem reduz significativamente o impacto do comprometimento de tokens e dificulta ataques de replay.

---

## Pontos que devem aparecer na imagem

### Fluxo da rotação

- Cliente solicita renovação
- API valida o Refresh Token
- Revoga o token utilizado
- Gera novo Access Token
- Gera novo Refresh Token
- Persiste apenas o hash
- Retorna o novo par de tokens

### Segurança

- Refresh Token nunca reutilizado
- Mitigação de Replay Attack
- Redução do impacto de token comprometido
- Revogação segura por sessão
- Rastreabilidade das sessões

### Implementação

- Clean Architecture
- DDD
- Use Case dedicado
- Persistência apenas do hash
- User Session
- Processo transacional

---

## Rascunho da descrição

Publicação destinada ao LinkedIn explicando o conceito de Refresh Token Rotation, sua importância para aplicações modernas e como a estratégia foi implementada na IAM Platform seguindo as boas práticas do OAuth 2.0 Security BCP.

---

## Referências de estudo

### Especificações

- OAuth 2.0 Security Best Current Practice (RFC 9700)
- OAuth 2.0 Threat Model and Security Considerations (RFC 6819)
- OAuth 2.1 Draft

### Segurança

- OWASP Session Management Cheat Sheet
- OWASP JSON Web Token Cheat Sheet

### Documentação

- Spring Security
- OAuth 2.0 Authorization Framework

---

## Observações

### Conceitos importantes

- Demonstrar a diferença entre Access Token e Refresh Token.
- Explicar por que apenas o hash do refresh token é armazenado.
- Mostrar que o refresh token utilizado deixa de ser válido imediatamente após a renovação.

### Arquitetura

- Processo implementado através de um Use Case específico.
- Separação entre domínio, aplicação e infraestrutura.
- Persistência desacoplada através de Ports & Adapters.
- Associação entre Refresh Token e User Session.

### Segurança

- Processo executado de forma transacional.
- Revogação e emissão dos novos tokens acontecem na mesma transação.
- Preparação da plataforma para logout seguro e revogação de sessões.
- Base para futuras implementações de detecção de reutilização de refresh tokens.

### Conteúdos relacionados

Próximos posts da série:

- Refresh Endpoint
- Logout
- Revogação de Sessões
- Session Management
- Reuse Detection