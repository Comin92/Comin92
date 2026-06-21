<h1 align="center">👋 Olá, eu sou o Jefferson</h1>

<p align="center">
Desenvolvedor orientado a negócios & IA — transformo regras de negócio complexas em sistemas full-stack robustos, com foco em qualidade, performance e segurança 🔐
</p>

---

## 🧠 Quem sou eu

Quase 10 anos resolvendo problemas técnicos no centro de operações críticas — ERPs, FinTechs e Telecom — antes de migrar para desenvolvimento full-stack guiado por engenharia de prompt avançada (Claude, Gemini, GPT).

Isso muda o que eu trago pra mesa: não chego só sabendo escrever código, chego entendendo **a regra de negócio por trás dele** — fluxo de logística, regra fiscal de varejo/atacado, arquitetura de rede de telecom, produto financeiro de cooperativa de crédito. Hoje aplico essa bagagem para arquitetar, construir e **auditar a segurança** de sistemas reais, em produção, usados por clientes pagantes.

- **Domínio de negócio:** ERP (logística, varejo/atacado, franquias), Telecom, FinTech cooperativo
- **Como desenvolvo:** Prompt engineering avançado + arquitetura de software assistida por IA — sem perder rigor técnico em validação, testes e segurança
- **Stack:** TypeScript, React, Next.js, Node.js (Fastify/Express), PostgreSQL, Prisma, Supabase, Redis, Docker, Kubernetes, integrações com Google (Calendar/Gmail/Drive), WhatsApp (Evolution API), Stripe

---

## 🚀 Projetos em destaque

> Repositórios privados (sistemas em produção, com dados reais de clientes) — descrição e métricas abaixo são geradas a partir do código-fonte real.

### 🏋️ M&M Studio Pro
SaaS completo de gestão para estúdios e personal trainers: prescrição de treinos, avaliações físicas com bioimpedância, agenda inteligente, controle financeiro (incluindo permuta de serviços) e RBAC granular com 100+ permissões. Integrações reais com Google Calendar/Gmail/Drive e WhatsApp (Evolution API). **Em produção, ativamente usado.**

`TypeScript` `Fastify` `React` `PostgreSQL/Supabase` `Docker` `Coolify`

- 205 testes unitários + 144 testes E2E
- RLS (Row Level Security) completo no banco, conformidade LGPD
- ~1.050 commits autorais · ~84.000 linhas de código · ativo desde jan/2025

### 🎮 ClashMix
Plataforma full-stack para organização de partidas competitivas de CS2: balanceamento automático de times (algoritmo snake draft + otimização), fluxo completo de pick/ban de mapas (MD1/MD3/MD5), chat em tempo real via WebSocket e integração com APIs externas (Dathost, Leetify).

`Next.js 15` `React 19` `Prisma` `Socket.io` `PostgreSQL`

- Algoritmo de balanceamento com busca exaustiva (252 combinações) em milissegundos
- Auditoria de segurança completa realizada (ver seção 🔒 abaixo)
- ~400 commits autorais · ~92.000 linhas de código · ativo desde nov/2025

### 🦷 Odontofin (contribuição)
SaaS de gestão odontológica (prontuário clínico, agendamento, financeiro) — **colaborador no projeto** (33 de 52 commits), com foco em otimização crítica de performance.

`React` `Fastify` `Prisma` `Redis` `Supabase RLS`

- Redução de 60–70% no payload de API via queries seletivas (eliminação de `SELECT *`)
- Latência de 1.5–2.2s reduzida para menos de 500ms com cache Redis (TTL adaptável, fallback automático)

### ⚽ Dashboard Brasileirão
Dashboard de classificação do Campeonato Brasileiro com cálculo automático de critérios de desempate, tema claro/escuro e pipeline DevOps completo.

`JavaScript` `Docker` `Kubernetes` `GitHub Actions`

- CI/CD com build multi-arquitetura (amd64/arm64) e versionamento automático
- Deploy em Kubernetes com 2 réplicas

---

## 🔒 Segurança como prática, não como discurso

Recentemente conduzi uma auditoria de segurança completa nos meus próprios projetos antes de qualquer divulgação pública — porque código em produção com dados reais de clientes exige isso. Alguns achados reais que identifiquei e corrigi:

- Removida rota backdoor que resetava senha de contas admin para um valor fixo
- Corrigida validação de CSRF que existia no código mas nunca era de fato executada (token forjável passava)
- Fechado vetor de spoofing de identidade em conexões WebSocket (chat privado)
- Identificados e removidos segredos reais (chaves de API, credenciais de banco) do histórico completo do Git via `git-filter-repo`
- Identificados e removidos dados pessoais sensíveis de clientes do versionamento (conformidade LGPD)
- Corrigido bypass de verificação de senha em fluxo de troca de senha

Ferramentas usadas: `gitleaks`, `git-filter-repo`, revisão manual de auth/CORS/CSRF/rate-limiting.

---

## 📊 Métricas reais (atualizadas automaticamente)

> Os repositórios dos projetos acima são privados, então o gráfico de contribuições padrão do GitHub não reflete o volume real de trabalho. O card abaixo é gerado por uma GitHub Action própria com acesso autorizado aos meus repositórios privados — atualiza todo dia.

![Metrics](./github-metrics.svg)

| Projeto | Commits autorais | Linhas de código | Período |
|---|---|---|---|
| M&M Studio Pro | ~1.050 (90%) | ~84.000 | jan/2025 – hoje |
| ClashMix | ~400 (99%) | ~92.000 | nov/2025 – hoje |
| Odontofin | 33 (63%, colaborador) | ~50.000 (total do projeto) | 2025 – hoje |
| Dashboard Brasileirão | 8 (100%) | ~440 | ago/2025 – hoje |

---

## 📫 Contato

<div align="center">

<a href="https://www.linkedin.com/in/jefferson-douglas-comin-1880b593">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="mailto:jdc.delete@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<a href="https://github.com/Comin92">
  <img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</div>

---

## 🚀 Tecnologias

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

</div>

---

⚠️ README atualizado em 2026-06-20.
