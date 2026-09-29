<p align="center">
  <picture><source media="(prefers-color-scheme: light)" srcset="assets/banner-pt-light.svg" /><img src="assets/banner-pt.svg" alt="Gabriel Fornaza da Silveira — Desenvolvedor Backend · .NET · Engenharia de Dados" width="100%" /></picture>
</p>

<p align="center">
  <picture><source media="(prefers-color-scheme: light)" srcset="assets/typing-pt-light.svg" /><img src="assets/typing-pt-dark.svg" alt="Desenvolvedor backend · .NET / C# · SQL Server — ETL orientado a configuração e integrações de dados — Agentes distribuídos, orquestração DAG, WebSocket — Desenvolvimento assistido por IA com Claude Code" /></picture>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/gabriel-fsilveira/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge" alt="LinkedIn" /></a>
  <a href="mailto:gabrielfornaza@yahoo.com.br"><img src="https://img.shields.io/badge/E--mail-3D59A1?style=for-the-badge" alt="E-mail" /></a>
  <img src="https://img.shields.io/badge/Florian%C3%B3polis%2C%20SC%20%C2%B7%20Remoto-1A1B27?style=for-the-badge" alt="Florianópolis, SC · Remoto" />
</p>

<p align="center">
  🌐 <a href="README.md">English</a> · Português
</p>

---

## 👋 Sobre mim

Sou **desenvolvedor backend** focado em **.NET / C#** e **SQL Server**. Desde 2023 trabalho remotamente para a **[DataSelf](https://www.dataself.com)** (Santa Clara, Califórnia), em um time internacional e com rotina assíncrona.

A maior parte do meu trabalho está na interseção entre backend e dados: **pipelines de ETL orientados a configuração**, **cargas incrementais**, **integrações com APIs de terceiros** (CRMs, ERPs, pagamentos) e os **serviços distribuídos** que executam tudo isso. Gosto de entender o sistema de ponta a ponta, da chamada HTTP até o data warehouse, e costumo ser quem investiga aquele bug estranho em produção.

Uso o **Claude Code** todos os dias para desenho de solução, implementação, code review, testes e documentação.

- 🎓 Bacharelado em Sistemas de Informação — **UFSC** (conclusão prevista em dez/2026)
- 🌎 Português (nativo) · Inglês (avançado, leitura e escrita técnica no dia a dia)

## 🛠️ O que eu construo no trabalho

- **Engine genérica de ETL para APIs REST**: construí e mantenho, como principal responsável, uma engine orientada a configuração em JSON que extrai dados de APIs SaaS, como HubSpot e ClickUp, e os carrega em um data warehouse em SQL Server. Para adicionar uma fonte nova, basta configurar, sem mudar código.
- **Cargas incrementais**: modos Load All, Replace, Upsert por PK e Append dirigidos por metadados, com watermark automático, sobre uma camada que trata OAuth 2.0, paginação por cursor/página/offset e rate limiting.
- **Plataforma de orquestração (do zero)**: construí o backend de uma nova plataforma de orquestração de pipelines, com agentes de execução distribuídos, gateway WebSocket em tempo real e agendamento em DAG com logs ao vivo e trilha de auditoria.
- **Confiabilidade e segurança**: correções de integridade de dados em cargas incrementais, ambientes de teste reproduzíveis com Docker, automação de testes de interface (FlaUI) e testes de segurança de APIs.

## 🧰 Stack

<table>
  <tr>
    <td><b>Backend</b></td>
    <td>
      <picture><source media="(prefers-color-scheme: light)" srcset="assets/stack-backend-light.svg" /><img src="assets/stack-backend-dark.svg" height="40" alt="C#, .NET, Python, FastAPI" /></picture>
      <br /><sub>ASP.NET Core · Entity Framework Core · LINQ · REST · WebSocket · CQRS · Clean Architecture</sub>
    </td>
  </tr>
  <tr>
    <td><b>Dados</b></td>
    <td>
      <picture><source media="(prefers-color-scheme: light)" srcset="assets/stack-data-light.svg" /><img src="assets/stack-data-dark.svg" height="40" alt="SQL Server, PostgreSQL, MongoDB" /></picture>
      <br /><sub>SQL Server / T-SQL · data warehouse (esquema estrela) · ETL / CDC · SqlBulkCopy · pandas</sub>
    </td>
  </tr>
  <tr>
    <td><b>DevOps e Cloud</b></td>
    <td>
      <picture><source media="(prefers-color-scheme: light)" srcset="assets/stack-devops-light.svg" /><img src="assets/stack-devops-dark.svg" height="40" alt="Docker, Linux, Azure, Git, GitHub, GitHub Actions, Bash, PowerShell" /></picture>
    </td>
  </tr>
  <tr>
    <td><b>Frontend</b></td>
    <td>
      <picture><source media="(prefers-color-scheme: light)" srcset="assets/stack-front-light.svg" /><img src="assets/stack-front-dark.svg" height="40" alt="React, TypeScript, Tailwind CSS" /></picture>
    </td>
  </tr>
  <tr>
    <td><b>Ferramentas</b></td>
    <td>
      <picture><source media="(prefers-color-scheme: light)" srcset="assets/stack-tools-light.svg" /><img src="assets/stack-tools-dark.svg" height="40" alt="Visual Studio, VS Code, Postman, Godot" /></picture>
      <br /><sub>xUnit · Moq · FlaUI · Swagger / OpenAPI · SSMS · Claude Code</sub>
    </td>
  </tr>
</table>

## 🚀 Projetos em destaque

### 🎬 [Reprise](https://github.com/GabrielfSilveiraDev/reprise)
Rastreador de séries auto-hospedado construído sobre um **log append-only de exibições**: progresso, episódios reassistidos, sequências e estatísticas são todos derivados dos eventos, nunca guardados como estado mutável.
- API em .NET 10 com Vertical Slice + CQRS, EF Core e PostgreSQL, multi-tenant por query filters globais
- Importador idempotente do export de dados do TV Time, com modo dry-run e relatório de conferência
- Catálogo enriquecido pelo TMDB e pelo TVmaze, atualizado por um worker em segundo plano
- Cliente React 19 com tipos da API gerados do contrato OpenAPI; testes de integração com Testcontainers e E2E com Playwright

`C#` `.NET 10` `ASP.NET Core` `EF Core` `PostgreSQL` `React` `TypeScript` `Docker`

### 🏠 GestAluguel · [API](https://github.com/GabrielfSilveiraDev/GestAluguelAPI) · [Web](https://github.com/GabrielfSilveiraDev/GestAluguelFrontEnd)
Plataforma multi-tenant de gestão de aluguéis: apartamentos, inquilinos, contratos, faturas mensais e portal de autoatendimento do inquilino.
- Clean Architecture com CQRS (MediatR), EF Core + SQL Server e isolamento por locador via query filters globais
- Pagamentos com geração nativa de Pix Copia e Cola, gateway Asaas (subcontas e split de pagamento) e webhook de pagamento
- 58 testes xUnit; CI/CD com GitHub Actions para o Azure App Service; front-end em React 19 publicado na Vercel

`C#` `.NET` `SQL Server` `MediatR` `Azure` `React` `TypeScript`

### 📊 Pipeline de dados de remuneração pública (TCC) · [Scrapers](https://github.com/GabrielfSilveiraDev/TCC) · [Dashboard](https://github.com/GabrielfSilveiraDev/TCC-FrontEnd)
Pipeline de ponta a ponta a partir dos portais de transparência de **7 Tribunais de Contas Estaduais**: web scraping → normalização → data warehouse em SQL Server (esquema estrela) → API REST em FastAPI → dashboard em React. *(O código do data warehouse e da API ainda não é público.)*
- Hierarquia de scrapers orientada a objetos (requests com retry/backoff e Selenium headless), com execuções retomáveis e idempotentes
- Matriz no GitHub Actions (estado × ano) que roda em paralelo na nuvem os scrapers mais lentos
- Dashboard analítico em React + TypeScript com paginação no backend, comparativos por estado e cargo e histórico de remuneração por pessoa

`Python` `Selenium` `SQL Server` `FastAPI` `React` `TypeScript` `GitHub Actions`

### 🎮 CronoArena <sub>(repositório privado)</sub>
Projeto pessoal: protótipo de roguelike de ação top-down em **Godot 4**, com 6 campeões jogáveis, arenas procedurais geradas por seed e pixel art 100% gerada por código. Inclui um modo de smoke test headless que exercita todos os campeões e joga uma partida completa até o chefe.

`Godot` `GDScript`

## 📈 Atividade no GitHub

<p align="center">
  <picture><source media="(prefers-color-scheme: light)" srcset="assets/cards/streak-light.svg" /><img src="assets/cards/streak-dark.svg" height="165" alt="Sequência de contribuições" /></picture>
  <picture><source media="(prefers-color-scheme: light)" srcset="assets/cards/top-langs-light.svg" /><img src="assets/cards/top-langs-dark.svg" height="165" alt="Linguagens mais usadas" /></picture>
</p>

<p align="center">
  <picture><source media="(prefers-color-scheme: light)" srcset="assets/cards/snake-light.svg" /><img src="assets/cards/snake-dark.svg" alt="Cobrinha comendo o gráfico de contribuições" /></picture>
</p>

<p align="center"><sub>A maior parte do meu trabalho profissional fica em repositórios privados da empresa; essas contribuições entram na contagem do gráfico acima.</sub></p>

<img src="assets/footer.svg" width="100%" alt="" />
