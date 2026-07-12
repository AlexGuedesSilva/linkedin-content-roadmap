# Série IAM Platform

## Descrição

Acompanha a construção prática de uma plataforma de Identity and Access Management, conectando decisões de domínio, arquitetura, persistência, segurança e evolução operacional.

## Objetivo

Documentar, em sequência, as decisões técnicas e os aprendizados necessários para construir uma IAM Platform modular, segura e testável.

## Tecnologias e assuntos

Java, Spring Boot, DDD, Clean Architecture, arquitetura modular, persistência, autenticação, autorização, tokens, auditoria e testes automatizados.

## Conteúdos

| Nº | Tema | Status | Localização |
|---:|---|---|---|
| 01 | Por que construir uma IAM Platform? | Publicado | [Arquivo](published/01-por-que-construir-uma-iam-platform.md) |
| 02 | Por que IAM? | Publicado | [Arquivo](published/02-por-que-iam.md) |
| 03 | Escolhendo a arquitetura: Modular Monolith, Clean Architecture e DDD | Publicado | [Arquivo](published/03-escolhendo-a-arquitetura-modular-monolith-clean-architecture-e-ddd.md) |
| 04 | Estrutura dos módulos | Publicado | [Arquivo](published/04-estrutura-dos-modulos.md) |
| 05 | Modelando o domínio | Publicado | [Arquivo](published/05-modelando-o-dominio.md) |
| 06 | Entity vs Value Object | Publicado | [Arquivo](published/06-entity-vs-value-object.md) |
| 07 | Por que usar Records para Value Objects? | Publicado | [Arquivo](published/07-por-que-usar-records-para-value-objects.md) |
| 08 | Rich Domain Model | Publicado | [Arquivo](published/08-rich-domain-model.md) |
| 09 | Repository Pattern | Publicado | [Arquivo](published/09-repository-pattern.md) |
| 10 | Persistence Adapter | Publicado | [Arquivo](published/10-persistence-adapter.md) |
| 11 | Domain Entity vs JPA Entity | Publicado | [Arquivo](published/11-domain-entity-vs-jpa-entity.md) |
| 12 | Mapper entre domínio e persistência | Publicado | [Arquivo](published/12-mapper-entre-dominio-e-persistencia.md) |
| 13 | Por que o domínio não possui `@Entity`? | Publicado | [Arquivo](published/13-por-que-o-dominio-nao-possui-entity.md) |
| 14 | RegisterUserUseCase | Publicado | [Arquivo](published/14-registeruserusecase.md) |
| 15 | PasswordHasher como porta | Publicado | [Arquivo](published/15-passwordhasher-como-porta.md) |
| 16 | UserIdGenerator como abstração | Publicado | [Arquivo](published/16-useridgenerator-como-abstracao.md) |
| 17 | Primeira versão funcional da IAM Platform | Publicado | [Arquivo](published/17-primeira-versao-funcional-da-iam-platform.md) |
| 18 | Flyway e versionamento do banco de dados | Publicado | [Arquivo](backlog/18-flyway-e-versionamento-do-banco-de-dados.md) |
| 19 | LoginUserUseCase | Backlog | [Arquivo](backlog/19-loginuserusecase.md) |
| 20 | Emissão de JWT | Backlog | [Arquivo](backlog/20-emissao-de-jwt.md) |
| 21 | JWT com RS256 | Backlog | [Arquivo](backlog/21-jwt-com-rs256.md) |
| 22 | Endpoint JWKS | Backlog | [Arquivo](backlog/22-endpoint-jwks.md) |
| 23 | Refresh Token | Backlog | [Arquivo](backlog/23-refresh-token.md) |
| 24 | Rotação de Refresh Token | Backlog | [Arquivo](backlog/24-rotacao-de-refresh-token.md) |
| 25 | Logout e revogação | Backlog | [Arquivo](backlog/25-logout-e-revogacao.md) |
| 26 | Sessões de usuário | Backlog | [Arquivo](backlog/26-sessoes-de-usuario.md) |
| 27 | RBAC | Backlog | [Arquivo](backlog/27-rbac.md) |
| 28 | ABAC | Backlog | [Arquivo](backlog/28-abac.md) |
| 29 | Auditoria de eventos | Backlog | [Arquivo](backlog/29-auditoria-de-eventos.md) |
| 30 | API Keys | Backlog | [Arquivo](backlog/30-api-keys.md) |
| 31 | Transformando o monólito modular em microsserviços | Backlog | [Arquivo](backlog/31-transformando-o-monolito-modular-em-microsservicos.md) |

## Próximos conteúdos sugeridos

* 19 — LoginUserUseCase
* 20 — Emissão de JWT
* 21 — JWT com RS256
* 22 — Endpoint JWKS

