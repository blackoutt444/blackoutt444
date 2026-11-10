<h1 align="center">Pedro Vale de Lima Bezerra</h1>

<p align="center">
  <b>Desenvolvedor de Software · Foco em Back-end · Engenharia de Software</b><br>
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

Sou desenvolvedor de software com foco em **back-end**, preferência por **Python** e experiência em diferentes camadas de aplicações: APIs, regras de negócio, bancos de dados, web e mobile. Curso Engenharia de Software na Fametro, com conclusão prevista para dezembro de 2028.

Além de Python, trabalho com Node.js, NestJS e TypeScript no back-end, PostgreSQL e Supabase nos dados, e React, Next.js e React Native nas interfaces.

- 🔭 Desenvolvendo o **TocaAqui**, um marketplace para contratação de músicos, da modelagem do banco e das regras de autorização até as telas web e mobile
- ⚙️ Trabalho com processo: issues, branches, pull requests, integração contínua e testes automatizados
- 🧠 Tenho interesse em Inteligência Artificial e estudo a integração de LLMs em aplicações
- 🎹 Fora do código, sou tecladista

## 🛠️ Tecnologias

| Área | Tecnologias |
| --- | --- |
| **Back-end** | Python · Flask · FastAPI · Node.js · NestJS · APIs REST |
| **Linguagens** | Python · TypeScript · JavaScript · SQL · Java · C |
| **Banco de dados e BaaS** | PostgreSQL · PostGIS · Supabase · Firebase |
| **Autenticação e autorização** | Supabase Auth · Firebase Auth · JWT · RBAC · Row Level Security |
| **Front-end e mobile** | React · Next.js · React Native · Expo · HTML · CSS |
| **Qualidade** | Git · GitHub Actions · Vitest · testes automatizados · integração contínua |
| **IA** | Integração com LLM via API da OpenAI (protótipo Corretor Fácil) · RAG com embeddings locais, LLM local com Ollama, saída estruturada validada com Pydantic e avaliação automatizada (cardapio-rag) |

**Ferramentas:** uso agentes de programação (Codex e Claude Code) como apoio para escrever, revisar e testar código. Para mim eles são ferramenta de trabalho, não projetos de IA.

## 🚀 Projetos em destaque

### 🎹 TocaAqui: marketplace de músicos
> *Repositório privado, produto em desenvolvimento. Acesso de leitura para avaliação técnica mediante solicitação.*

Plataforma brasileira para contratar músicos e profissionais da música, com app web, painel administrativo e app mobile.

- **Banco e autorização:** PostgreSQL no Supabase com migrations versionadas, políticas de Row Level Security, funções RPC transacionais e testes de RLS
- **Regras de negócio** isoladas em um pacote de domínio: cálculo de taxas, checkout em sandbox, ledger imutável e webhooks idempotentes
- **Arquitetura:** monorepo em TypeScript (npm workspaces) com web e admin em Next.js, app mobile em Expo/React Native e pacotes compartilhados de domínio, validação e cliente de API
- **Qualidade:** CI no GitHub Actions com lint, typecheck, testes (Vitest), build e auditoria de dependências; fluxo com issues, pull requests e Conventional Commits
- **Documentação** de arquitetura, produto e segurança (threat model e matriz de autorização)
- **Em números:** 24 migrations SQL, 9 suítes de teste de RLS, 21 arquivos de teste com Vitest e 12 pull requests mesclados com CI aprovado

### 🎧 [Conversor de Áudio](https://github.com/blackoutt444/conversor-de-audio) [![CI](https://github.com/blackoutt444/conversor-de-audio/actions/workflows/ci.yml/badge.svg)](https://github.com/blackoutt444/conversor-de-audio/actions/workflows/ci.yml)

API em **Python/Flask** que baixa o áudio de um vídeo a partir do link e converte para MP3, WAV, OGG, FLAC ou AAC com **yt-dlp** e **FFmpeg**.

- Testes automatizados com pytest, incluindo conversão real pelo FFmpeg para todos os formatos
- Integração contínua no GitHub Actions (Python 3.12 e 3.13): o selo ao lado mostra o resultado do último run

### 📋 Corretor Fácil
> *Repositório privado, protótipo de abril de 2025*

App mobile em **React Native/Expo** para corretores de planos de saúde, com cotação, busca de rede credenciada e sugestões de plano geradas por um **LLM** chamado pela API da OpenAI.

### 🍽️ [cardapio-rag](https://github.com/blackoutt444/cardapio-rag) [![CI](https://github.com/blackoutt444/cardapio-rag/actions/workflows/ci.yml/badge.svg)](https://github.com/blackoutt444/cardapio-rag/actions/workflows/ci.yml)

API em **Python/FastAPI** que responde perguntas sobre um cardápio fictício com **RAG**: busca semântica com embeddings locais e resposta de um **LLM local (Ollama)** em JSON validado com **Pydantic**. Roda sem chave de API paga.

- Avaliação automatizada com perguntas de referência: acerto da busca (hit@k e MRR), JSON válido, fidelidade ao contexto, abstenção quando o cardápio não tem a resposta e latência por etapa, com data, commit, modelo e hardware registrados
- Provedores de LLM atrás de uma interface (Ollama, OpenAI, Anthropic e um falso para testes)
- Testes com pytest e LLM simulado, CI no GitHub Actions e imagem Docker
