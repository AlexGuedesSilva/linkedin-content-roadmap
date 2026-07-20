# Spring — 04 — Inversão de Controle e Injeção de Dependência

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

* **Série:** Spring
* **Número:** 04
* **Tema:** Inversão de Controle (IoC) e Injeção de Dependência (DI)
* **Data de criação:** 20/07/2026
* **Data de publicação:**
* **Link da publicação:**
* **Branch ou feature relacionada:** —
* **Tecnologias relacionadas:**

  * Spring Framework
  * Spring Boot
  * IoC Container
  * Dependency Injection
  * Spring Beans
  * @Component
  * @Service
  * @Repository
  * @RestController
  * Constructor Injection

---

## Objetivo do post

Explicar um dos conceitos mais importantes do Spring Framework: como o Spring Container assume a responsabilidade de criar, configurar e gerenciar os objetos da aplicação (Beans), além de fornecer automaticamente suas dependências.

O objetivo é mostrar que IoC e DI são os pilares que tornam aplicações Spring mais desacopladas, testáveis, reutilizáveis e fáceis de evoluir.

---

## Mensagem principal

No Spring, você não cria e conecta manualmente os objetos da aplicação.

O Spring Container faz esse trabalho automaticamente através da Inversão de Controle (IoC) e da Injeção de Dependência (DI), permitindo que o desenvolvedor foque nas regras de negócio em vez da infraestrutura.

---

## Pontos que devem aparecer na imagem

* Diferença entre uma aplicação sem IoC e uma aplicação utilizando o Spring Container.
* Explicação visual da Inversão de Controle (IoC).
* Explicação visual da Injeção de Dependência (DI).
* Fluxo do Spring Container:

  * Escaneamento de componentes
  * Registro dos Beans
  * Resolução das dependências
  * Injeção automática
* Exemplo utilizando:

  * Controller
  * Service
  * Repository
* Exemplo de Constructor Injection.
* Principais estereótipos do Spring:

  * @Component
  * @Service
  * @Repository
  * @RestController
* Comparação entre:

  * Constructor Injection (recomendado)
  * Setter Injection
  * Field Injection
* Benefícios:

  * Baixo acoplamento
  * Alta coesão
  * Facilidade de testes
  * Melhor manutenção
  * Reutilização de componentes

---

## Rascunho da descrição

Adicionar posteriormente.

Principais tópicos que deverão ser abordados:

* O que é IoC.
* O que é DI.
* Como o Spring cria os Beans.
* Como ocorre a injeção automática.
* Por que Constructor Injection é recomendada.
* Benefícios para projetos reais.
* Relação entre IoC, DI e Clean Architecture.

---

## Referências de estudo

* Spring Framework Reference Documentation
* Spring Boot Reference Documentation
* Spring Core Documentation (IoC Container)
* Spring Beans Documentation
* "Spring in Action" — Craig Walls
* "Spring Start Here" — Laurentiu Spilca

---

## Observações

* Este post servirá como base para diversos conteúdos futuros da série Spring.
* Fazer referência aos próximos posts sobre:

  * Como o Spring encontra seus Beans.
  * O ciclo de vida dos Beans.
  * Spring Context.
  * @Autowired vs Constructor Injection.
  * O que acontece quando a aplicação Spring Boot inicia.
  * Como funciona o DispatcherServlet.
* Manter um padrão visual semelhante aos demais posts da série, utilizando tema escuro, diagramas didáticos e foco em aprendizagem.
* Evitar excesso de texto na imagem; privilegiar fluxos visuais e exemplos práticos.
