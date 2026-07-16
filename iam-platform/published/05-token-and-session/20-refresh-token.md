# IAM Platform — 20 — Refresh Token

## Status

* [x] Ideia registrada
* [x] Conteúdo estudado
* [x] Roteiro definido
* [x] Imagem criada
* [x] Descrição criada
* [x] Revisado
* [ ] Agendado
* [x] Publicado

---

## Informações

* **Série:** IAM Platform
* **Número:** 20
* **Tema:** Refresh Token
* **Data de criação:** 16/07/2026
* **Data de publicação:** 16/07/2026
* **Link da publicação:**
* **Branch ou feature relacionada:** `feature/token-refresh-session`
* **Tecnologias relacionadas:** Java 21, Spring Boot, JWT, RS256, Domain-Driven Design (DDD), Clean Architecture, Spring Security

---

## Objetivo do post

Apresentar uma visão geral sobre o funcionamento do Refresh Token, explicando sua finalidade, seu papel no fluxo de autenticação e como ele será modelado dentro da IAM Platform utilizando DDD e Clean Architecture.

---

## Mensagem principal

O Refresh Token não substitui o Access Token. Ele existe para renovar a autenticação de forma segura, permitindo sessões de longa duração sem comprometer a segurança da aplicação. Antes de implementar infraestrutura ou persistência, é importante modelar corretamente esse conceito no domínio.

---

## Pontos que devem aparecer na imagem

* Fluxo completo de autenticação utilizando Access Token e Refresh Token.
* Diferença entre Access Token e Refresh Token.
* Modelo de domínio inicial (`RefreshToken`, `RefreshTokenId` e `RefreshTokenValue`).
* Explicação dos atributos principais (`id`, `tokenHash`, `userId`, `createdAt`, `expiresAt` e `revoked`).
* Comportamentos do domínio (`revoke()`, `isExpired()` e `isActive()`).
* Conceito de Refresh Token Rotation.
* Relação entre Login, Refresh, Logout e Revogação.
* Boas práticas de segurança para armazenamento de Refresh Tokens.
* Comparação entre Access Token e Refresh Token.
* Visão da evolução futura da IAM Platform.

---

## Rascunho da descrição

Após implementar a autenticação utilizando JWT assinado com RS256, iniciei a construção do modelo de domínio responsável pelo Refresh Token.

Nesta etapa o foco não foi persistência ou infraestrutura, mas sim representar corretamente esse conceito dentro do domínio utilizando DDD e Clean Architecture.

O objetivo é construir uma base sólida para as próximas implementações da plataforma, como User Sessions, Refresh Token Rotation, Logout, Logout All e detecção de reutilização de tokens.

---

## Referências de estudo

* RFC 7519 — JSON Web Token (JWT)
* RFC 6749 — OAuth 2.0 Authorization Framework
* RFC 6819 — OAuth 2.0 Threat Model and Security Considerations
* OAuth 2.0 Security Best Current Practice (OAuth 2.0 BCP)
* Spring Security Reference Documentation
* Domain-Driven Design — Eric Evans
* Implementing Domain-Driven Design — Vaughn Vernon

---

## Observações

* Este post marca o início da feature `feature/token-refresh-session`.
* O primeiro commit da implementação é `feat(token): add refresh token domain model`.
* O modelo de domínio foi construído sem dependências de Spring ou JPA, mantendo a independência da camada de domínio.
* O `RefreshTokenValue` representa o hash persistido do token, e não o valor entregue ao cliente.
* Os próximos posts da série abordarão:

  * User Session;
  * Refresh Token Rotation;
  * Logout;
  * Logout All;
  * Persistência de Refresh Tokens;
  * Segurança contra Replay Attack.
