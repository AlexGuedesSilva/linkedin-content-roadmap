# IAM Platform — Glossário

## ABAC

Modelo de autorização que decide o acesso com base em atributos do usuário, do recurso, da ação e do contexto.

## Access Token

Credencial de curta duração apresentada a uma API para provar que uma chamada foi autorizada.

## Adapter

Implementação que conecta uma porta da aplicação a uma tecnologia externa, como banco de dados, framework ou serviço.

## Aggregate

Conjunto de objetos de domínio tratado como uma unidade de consistência, controlado por uma raiz de agregado.

## Authentication

Processo de verificar quem está tentando acessar o sistema, normalmente por credenciais ou outro fator de prova.

## Authorization

Processo de decidir o que uma identidade autenticada pode fazer sobre determinado recurso.

## Claim

Informação declarada dentro de um token, como identificador do usuário, emissor, público ou prazo de validade.

## Clean Architecture

Estilo arquitetural que mantém regras de negócio independentes de frameworks, interfaces e detalhes de infraestrutura.

## DDD

Domain-Driven Design: abordagem que modela software a partir do domínio, de sua linguagem e de suas regras de negócio.

## Entity

Objeto de domínio definido por uma identidade contínua, mesmo quando seus atributos mudam ao longo do tempo.

## IAM

Identity and Access Management: conjunto de práticas e componentes para gerenciar identidades, autenticação e acesso.

## Identity

Representação de uma pessoa, sistema ou serviço reconhecido pela plataforma.

## JWK

JSON Web Key: representação JSON de uma chave criptográfica e de seus metadados.

## JWS

JSON Web Signature: padrão para assinar digitalmente conteúdo e permitir a verificação de sua integridade e origem.

## JWT

JSON Web Token: formato compacto de token que transporta claims e pode ser assinado ou protegido criptograficamente.

## JWKS

JSON Web Key Set: documento que publica um conjunto de chaves, normalmente as chaves públicas usadas para verificar tokens.

## `kid`

Identificador de chave incluído no cabeçalho de um token para indicar qual JWK deve validar sua assinatura.

## Modular Monolith

Aplicação implantada como uma unidade, mas dividida internamente em módulos com responsabilidades e limites explícitos.

## Port

Contrato definido pelo núcleo da aplicação para entrada de casos de uso ou acesso a capacidades externas.

## RBAC

Modelo de autorização em que permissões são associadas a papéis, e os papéis são atribuídos às identidades.

## Refresh Token

Credencial usada para obter novos access tokens sem exigir que o usuário forneça novamente suas credenciais.

## Replay Attack

Ataque em que uma credencial ou mensagem válida capturada é reutilizada para tentar repetir uma operação autorizada.

## Repository

Abstração que oferece acesso a agregados sem expor ao domínio os detalhes de armazenamento.

## Revocation

Invalidação deliberada de uma credencial ou sessão antes de seu vencimento natural.

## Rotation

Substituição de um refresh token por outro a cada uso, reduzindo o valor de um token antigo que seja reutilizado.

## RS256

Algoritmo de assinatura JWS que combina RSA com SHA-256 e usa chaves diferentes para assinar e verificar.

## Session

Período e estado associados à interação autenticada de uma identidade com o sistema.

## Value Object

Objeto de domínio definido por seus valores, geralmente imutável e sem identidade própria.
