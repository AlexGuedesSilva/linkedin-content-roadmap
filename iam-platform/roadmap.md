# IAM Platform — Roadmap técnico

Este roadmap cruza duas dimensões diferentes:

- **Estado editorial:** publicado, em andamento ou backlog.
- **Estado da implementação:** somente o que está documentado no próprio post; conteúdo em backlog não comprova feature implementada.

Quando o arquivo não informa uma branch ou evidência de implementação, a tabela registra isso sem fazer suposições.

## Fase 1 — Foundation

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 01 | [Por que construir uma IAM Platform?](published/01-foundation/01-por-que-construir-uma-iam-platform.md) | Publicado | Não documentada no arquivo |
| 02 | [Por que IAM?](published/01-foundation/02-por-que-iam.md) | Publicado | Não documentada no arquivo |
| 03 | [Escolhendo a arquitetura](published/01-foundation/03-escolhendo-a-arquitetura-modular-monolith-clean-architecture-e-ddd.md) | Publicado | Não documentada no arquivo |
| 04 | [Estrutura dos módulos](published/01-foundation/04-estrutura-dos-modulos.md) | Publicado | Não documentada no arquivo |

## Fase 2 — Identity

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 05 | [Modelando o domínio](published/02-identity/05-modelando-o-dominio.md) | Publicado | Não documentada no arquivo |
| 06 | [Entity vs Value Object](published/02-identity/06-entity-vs-value-object.md) | Publicado | Não documentada no arquivo |
| 07 | [Records para Value Objects](published/02-identity/07-por-que-usar-records-para-value-objects.md) | Publicado | Não documentada no arquivo |
| 08 | [Rich Domain Model](published/02-identity/08-rich-domain-model.md) | Publicado | Não documentada no arquivo |
| 14 | [RegisterUserUseCase](published/02-identity/14-registeruserusecase.md) | Publicado | Não documentada no arquivo |
| 16 | [UserIdGenerator como abstração](published/02-identity/16-useridgenerator-como-abstracao.md) | Publicado | Não documentada no arquivo |

## Fase 3 — Persistence

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 09 | [Repository Pattern](published/03-persistence/09-repository-pattern.md) | Publicado | Não documentada no arquivo |
| 10 | [Persistence Adapter](published/03-persistence/10-persistence-adapter.md) | Publicado | Não documentada no arquivo |
| 11 | [Domain Entity vs JPA Entity](published/03-persistence/11-domain-entity-vs-jpa-entity.md) | Publicado | Não documentada no arquivo |
| 12 | [Mapper entre domínio e persistência](published/03-persistence/12-mapper-entre-dominio-e-persistencia.md) | Publicado | Não documentada no arquivo |
| 13 | [Domínio sem `@Entity`](published/03-persistence/13-por-que-o-dominio-nao-possui-entity.md) | Publicado | Não documentada no arquivo |
| 18 | [Flyway e versionamento do banco](published/03-persistence/18-flyway-e-versionamento-do-banco-de-dados.md) | Publicado | Implementação descrita; branch `feature/identity-database-migration` |

## Fase 4 — Authentication

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 15 | [PasswordHasher como porta](published/04-authentication/15-passwordhasher-como-porta.md) | Publicado | Não documentada no arquivo |
| 17 | [Primeira versão funcional da IAM Platform](published/04-authentication/17-primeira-versao-funcional-da-iam-platform.md) | Publicado | Não documentada no arquivo |

## Fase 5 — Tokens and Sessions

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 19 | [JWT (RS256) + JWKS](published/05-token-and-session/19-jwt-rs256-jwks.md) | Publicado | Implementação descrita; branch `feature/token-jwt` |
| 20 | [Refresh Token](published/05-token-and-session/20-refresh-token.md) | Publicado | Início da feature registrado; branch `feature/token-refresh-session` |
| 21 | [Modelando Refresh Token com DDD](published/05-token-and-session/21-modelando-refresh-token-com-ddd.md) | Publicado | Modelo de domínio descrito; branch `feature/token-refresh-session` |
| 22 | [JWT com RS256](backlog/05-token-and-session/22-jwt-com-rs256.md) | Backlog | Conteúdo planejado; implementação não confirmada |
| 23 | [Endpoint JWKS](backlog/05-token-and-session/23-endpoint-jwks.md) | Backlog | Conteúdo planejado; implementação não confirmada |
| 24 | [Rotação de Refresh Token](backlog/05-token-and-session/24-rotacao-de-refresh-token.md) | Backlog | Feature futura; implementação não confirmada |
| 25 | [Logout e revogação](backlog/05-token-and-session/25-logout-e-revogacao.md) | Backlog | Feature futura; implementação não confirmada |
| 26 | [Sessões de usuário](backlog/05-token-and-session/26-sessoes-de-usuario.md) | Backlog | Feature futura; implementação não confirmada |

## Fase 6 — Authorization

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 27 | [RBAC](backlog/06-authorization/27-rbac.md) | Backlog | Feature futura; implementação não confirmada |
| 28 | [ABAC](backlog/06-authorization/28-abac.md) | Backlog | Feature futura; implementação não confirmada |

## Fase 7 — API Keys

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 30 | [API Keys](backlog/07-api-keys/30-api-keys.md) | Backlog | Feature futura; implementação não confirmada |

## Fase 8 — Audit

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 29 | [Auditoria de eventos](backlog/08-audit/29-auditoria-de-eventos.md) | Backlog | Feature futura; implementação não confirmada |

## Fase 9 — Architecture Evolution

| Post | Conteúdo | Editorial | Implementação / feature |
|---:|---|---|---|
| 31 | [Transformando o monólito modular em microsserviços](backlog/09-architecture-evolution/31-transformando-o-monolito-modular-em-microsservicos.md) | Backlog | Evolução futura; implementação não confirmada |
