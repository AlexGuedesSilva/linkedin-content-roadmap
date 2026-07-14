# IAM Platform — 19 — JWT (RS256) + JWKS

## Status

* [x] Ideia registrada
* [x] Conteúdo estudado
* [x] Roteiro definido
* [x] Imagem criada
* [x] Descrição criada
* [x] Revisado
* [ ] Agendado
* [x] Publicado

## Informações

* Série: IAM Platform
* Número: 19
* Tema: Emissão de Access Token com JWT (RS256) + JWKS
* Data de criação: 14/07/2026
* Data de publicação: 14/07/2026
* Link da publicação:https://www.linkedin.com/feed/update/urn:li:activity:7482928529064497152/
  
* Branch ou feature relacionada: 
  feature/token-jwt

* Tecnologias relacionadas: 
Java 21
Spring Boot
JWT
JWKS
Nimbus JOSE + JWT
RSA (RS256)
Clean Architecture
DDD

## Objetivo do post

Explicar de forma didática como funciona a emissão de um Access Token utilizando JWT assinado com RS256, o papel do JWKS na publicação das chaves públicas e como essa implementação foi organizada utilizando Clean Architecture.

## Mensagem principal

Mostrar que JWT é muito mais do que um token de autenticação: ele envolve assinatura digital, criptografia assimétrica, gerenciamento de chaves públicas (JWKS) e uma arquitetura desacoplada que facilita a evolução para microsserviços.

## Aprendizados

* Diferença entre HS256 e RS256

* Estrutura do JWT

* JWKS

* Nimbus JOSE

* RSA

* Clean Architecture aplicada à autenticação

## Pontos que devem aparecer na imagem

* Fluxo completo de autenticação

* JWT (estrutura)

* Claims do JWT

* RS256 × HS256

* Chaves RSA

* JWKS

* Arquitetura (Clean Architecture)

* Segurança

* Detalhes importantes

* Tecnologias utilizadas

## Referências de estudo

* RFC 7519 — JSON Web Token (JWT)

* RFC 7517 — JSON Web Key (JWK)

* RFC 7515 — JSON Web Signature (JWS)

* Nimbus JOSE + JWT Documentation

* Spring Security Reference

* OWASP JWT Cheat Sheet 

## Observações

Foi utilizada a biblioteca Nimbus JOSE + JWT.

A aplicação depende da abstração AccessTokenIssuer.

A implementação concreta Rs256JwtAccessTokenIssuer permanece na infraestrutura.

As chaves RSA são carregadas via configuração.

O endpoint JWKS publica apenas a chave pública.

Base preparada para futura implementação de Refresh Token e OAuth2.
