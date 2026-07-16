# IAM Platform — Sumário

Este sumário organiza a série como um livro técnico. A ordem é numérica dentro de cada capítulo, independentemente do status editorial.

## Capítulo 1 — Fundamentos

- [Post 01 — Por que construir uma IAM Platform?](published/01-foundation/01-por-que-construir-uma-iam-platform.md) — **Publicado**
- [Post 02 — Por que IAM?](published/01-foundation/02-por-que-iam.md) — **Publicado**
- [Post 03 — Escolhendo a arquitetura: Modular Monolith, Clean Architecture e DDD](published/01-foundation/03-escolhendo-a-arquitetura-modular-monolith-clean-architecture-e-ddd.md) — **Publicado**
- [Post 04 — Estrutura dos módulos](published/01-foundation/04-estrutura-dos-modulos.md) — **Publicado**

## Capítulo 2 — Identity

- [Post 05 — Modelando o domínio](published/02-identity/05-modelando-o-dominio.md) — **Publicado**
- [Post 06 — Entity vs Value Object](published/02-identity/06-entity-vs-value-object.md) — **Publicado**
- [Post 07 — Por que usar Records para Value Objects?](published/02-identity/07-por-que-usar-records-para-value-objects.md) — **Publicado**
- [Post 08 — Rich Domain Model](published/02-identity/08-rich-domain-model.md) — **Publicado**
- [Post 14 — RegisterUserUseCase](published/02-identity/14-registeruserusecase.md) — **Publicado**
- [Post 16 — UserIdGenerator como abstração](published/02-identity/16-useridgenerator-como-abstracao.md) — **Publicado**

## Capítulo 3 — Persistência

- [Post 09 — Repository Pattern](published/03-persistence/09-repository-pattern.md) — **Publicado**
- [Post 10 — Persistence Adapter](published/03-persistence/10-persistence-adapter.md) — **Publicado**
- [Post 11 — Domain Entity vs JPA Entity](published/03-persistence/11-domain-entity-vs-jpa-entity.md) — **Publicado**
- [Post 12 — Mapper entre domínio e persistência](published/03-persistence/12-mapper-entre-dominio-e-persistencia.md) — **Publicado**
- [Post 13 — Por que o domínio não possui `@Entity`?](published/03-persistence/13-por-que-o-dominio-nao-possui-entity.md) — **Publicado**
- [Post 18 — Flyway e versionamento do banco de dados](published/03-persistence/18-flyway-e-versionamento-do-banco-de-dados.md) — **Publicado**

## Capítulo 4 — Autenticação

- [Post 15 — PasswordHasher como porta](published/04-authentication/15-passwordhasher-como-porta.md) — **Publicado**
- [Post 17 — Primeira versão funcional da IAM Platform](published/04-authentication/17-primeira-versao-funcional-da-iam-platform.md) — **Publicado**

## Capítulo 5 — Tokens e sessões

- [Post 19 — JWT (RS256) + JWKS](published/05-token-and-session/19-jwt-rs256-jwks.md) — **Publicado**
- [Post 20 — Refresh Token](published/05-token-and-session/20-refresh-token.md) — **Publicado**
- [Post 21 — Modelando Refresh Token com DDD](published/05-token-and-session/21-modelando-refresh-token-com-ddd.md) — **Publicado**
- [Post 22 — JWT com RS256](backlog/05-token-and-session/22-jwt-com-rs256.md) — **Backlog**
- [Post 23 — Endpoint JWKS](backlog/05-token-and-session/23-endpoint-jwks.md) — **Backlog**
- [Post 24 — Rotação de Refresh Token](backlog/05-token-and-session/24-rotacao-de-refresh-token.md) — **Backlog**
- [Post 25 — Logout e revogação](backlog/05-token-and-session/25-logout-e-revogacao.md) — **Backlog**
- [Post 26 — Sessões de usuário](backlog/05-token-and-session/26-sessoes-de-usuario.md) — **Backlog**

## Capítulo 6 — Autorização

- [Post 27 — RBAC](backlog/06-authorization/27-rbac.md) — **Backlog**
- [Post 28 — ABAC](backlog/06-authorization/28-abac.md) — **Backlog**

## Capítulo 7 — API Keys

- [Post 30 — API Keys](backlog/07-api-keys/30-api-keys.md) — **Backlog**

## Capítulo 8 — Auditoria

- [Post 29 — Auditoria de eventos](backlog/08-audit/29-auditoria-de-eventos.md) — **Backlog**

## Capítulo 9 — Evolução da arquitetura

- [Post 31 — Transformando o monólito modular em microsserviços](backlog/09-architecture-evolution/31-transformando-o-monolito-modular-em-microsservicos.md) — **Backlog**
