# IAM Platform — 21 — Modelando Refresh Token com DDD

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
* **Número:** 21
* **Tema:** Modelando Refresh Token com DDD
* **Data de criação:** 16/07/2026
* **Data de publicação:** 16/07/2026
* **Link da publicação:**
* **Branch ou feature relacionada:** `feature/token-refresh-session`
* **Tecnologias relacionadas:** Java 21, Spring Boot, Domain-Driven Design (DDD), Clean Architecture, JWT, Spring Security

---

## Objetivo do post

Demonstrar como o Refresh Token pode ser modelado como um conceito de domínio utilizando DDD, antes da implementação de persistência, infraestrutura ou casos de uso.

---

## Mensagem principal

Uma boa arquitetura começa pelo domínio.

Antes de criar tabelas, endpoints ou integrações, é importante modelar corretamente o comportamento e as regras de negócio do Refresh Token, mantendo o domínio independente de frameworks e tecnologias.

---

## Pontos que devem aparecer na imagem

* Estrutura da entidade RefreshToken.
* Value Objects:
  * RefreshTokenId
  * RefreshTokenValue
* Relação com UserId.
* Invariantes do domínio.
* Métodos de comportamento:
  * revoke()
  * isExpired()
  * isActive()
* Método create()
* Método restore()
* Ciclo de vida do Refresh Token.
* Benefícios do Rich Domain Model.
* Princípios de DDD aplicados.

---

## Rascunho da descrição

Após entender o papel do Refresh Token no fluxo de autenticação, o próximo passo foi modelar esse conceito dentro do domínio.

Nesta etapa, o objetivo não foi implementar persistência ou infraestrutura, mas representar corretamente as regras de negócio utilizando Domain-Driven Design.

O modelo foi construído com uma entidade de domínio, Value Objects e comportamentos que protegem suas invariantes, mantendo o domínio totalmente independente de Spring e JPA.

Esse modelo servirá como base para funcionalidades como User Session, Refresh Token Rotation, Logout e Replay Detection.

---

## Referências de estudo

* Domain-Driven Design — Eric Evans
* Implementing Domain-Driven Design — Vaughn Vernon
* RFC 7519 — JSON Web Token
* OAuth 2.0 Security Best Current Practice
* Spring Security Reference Documentation

---

## Observações

* Primeiro commit da feature `feature/token-refresh-session`.
* O domínio permanece completamente desacoplado da infraestrutura.
* O RefreshTokenValue representa o hash persistido do token.
* O token bruto nunca faz parte do domínio.
* Este modelo será evoluído nos próximos commits para suportar:
  * User Session
  * Persistência
  * Refresh Token Rotation
  * Logout
  * Replay Detection