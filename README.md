<h1 align="center">Pedro Vale de Lima Bezerra</h1>

<p align="center">
  <b>Desenvolvedor de Software · Back-end com Python · Interesse em Engenharia de IA</b><br>
  Engenharia de Software na Fametro · Manaus, AM
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white" alt="Flask">
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase">
</p>

---

## 🧑‍💻 Sobre mim

Sou desenvolvedor de software com foco em **back-end**, experiência em projetos **full stack** e interesse em **Engenharia de Inteligência Artificial**. Curso Engenharia de Software na Fametro, com conclusão prevista para dezembro de 2028.

No back-end, minha linguagem preferida é **Python**. Também trabalho com Node.js e TypeScript, e já atuei em projetos que passam por banco de dados, regras de negócio, APIs, web e mobile.

- 🔭 Desenvolvendo o **TocaAqui**, um marketplace para contratação de músicos, da modelagem do banco e das regras de autorização até as telas web e mobile
- 🤖 Uso agentes de programação (Codex e Claude) e prompting estruturado no dia a dia, e estou me aprofundando em aplicações com LLMs
- ⚙️ Trabalho com processo: issues, branches, pull requests, integração contínua e testes automatizados
- 🎹 Fora do código, sou tecladista

## 🛠️ Tecnologias

| Área | Tecnologias |
| --- | --- |
| **Back-end** | Python · Flask · Node.js · NestJS · APIs REST |
| **Linguagens** | Python · TypeScript · JavaScript · SQL · Java · C |
| **Banco de dados e BaaS** | PostgreSQL · PostGIS · Supabase · Firebase |
| **Autenticação e autorização** | Supabase Auth · Firebase Auth · JWT · RBAC · Row Level Security |
| **Front-end e mobile** | React · Next.js · React Native · Expo · HTML · CSS |
| **Qualidade** | Git · GitHub Actions · Vitest · testes automatizados · integração contínua |
| **IA** | Desenvolvimento assistido por IA · prompting estruturado · agentes de programação · API da OpenAI |

## 🚀 Projetos em destaque

### 🎹 TocaAqui: marketplace de músicos
> *Repositório privado: produto em desenvolvimento*

Plataforma brasileira para contratar músicos e profissionais da música, com app web, painel administrativo e app mobile.

- **Banco e autorização:** PostgreSQL no Supabase com migrations versionadas, políticas de Row Level Security, funções RPC transacionais e testes de RLS
- **Regras de negócio** isoladas em um pacote de domínio: cálculo de taxas, checkout em sandbox, ledger imutável e webhooks idempotentes
- **Arquitetura:** monorepo em TypeScript (npm workspaces) com web e admin em Next.js, app mobile em Expo/React Native e pacotes compartilhados de domínio, validação e cliente de API
- **Qualidade:** CI no GitHub Actions com lint, typecheck, testes (Vitest), build e auditoria de dependências; fluxo com issues, pull requests e Conventional Commits
- **Documentação** de arquitetura, produto e segurança (threat model e matriz de autorização)

### 🎧 [Conversor de Áudio](https://github.com/blackoutt444/conversor-de-audio)

API em **Python/Flask** que baixa o áudio de um vídeo a partir do link e converte para MP3, WAV, OGG, FLAC ou AAC com **yt-dlp** e **FFmpeg**.

- Testes automatizados com conversão real pelo FFmpeg, validação de entrada e proteção contra path traversal
- Integração contínua no GitHub Actions (Python 3.12 e 3.13)

### 📋 Corretor Fácil
> *Repositório privado*

App mobile em **React Native/Expo** para corretores de planos de saúde, com cotação, busca de rede credenciada e sugestões de plano geradas por um **LLM** (API da OpenAI).
