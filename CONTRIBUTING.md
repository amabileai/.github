# Guia de Contribuição — AmabileAI

Obrigado por contribuir com os projetos da AmabileAI. Este guia define as regras e padrões que todos os contribuidores devem seguir.

## Regra Fundamental

Todos os projetos da AmabileAI seguem uma arquitetura de governança controlada. O arquivo `architecture.yaml` na raiz de cada repositório é a **fonte da verdade** para todas as decisões técnicas. Nenhuma mudança arquitetural deve ser feita sem atualizar este arquivo e criar um ADR (Architecture Decision Record) correspondente.

## Como Contribuir

### 1. Criando um Novo Projeto

Novos projetos devem ser criados **exclusivamente** a partir do template `template-frontend-react` disponível na organização. Este template já inclui todas as configurações de governança, guardrails para IAs de código, pipeline de CI/CD e instruções para agentes.

Após criar o repositório a partir do template, preencha o Issue Form de **Project Kickoff** para definir as decisões arquiteturais do projeto.

### 2. Trabalhando em um Projeto Existente

Antes de escrever qualquer código, leia os seguintes arquivos na raiz do repositório:

- `architecture.yaml` — Decisões arquiteturais do projeto
- `AGENTS.md` — Padrões e regras para agentes de IA
- `docs/arch/` — Architecture Decision Records (ADRs)

### 3. Padrões de Código

Todos os projetos utilizam TypeScript estrito com as seguintes regras obrigatórias:

- Nunca use `any`, `@ts-ignore` ou `as unknown as`
- Nunca use `fetch()` diretamente; use o cliente HTTP em `src/services/api-client.ts`
- Sempre crie testes unitários para novos componentes e hooks
- Siga a estrutura de pastas definida no template

### 4. Commits

Utilizamos Conventional Commits obrigatoriamente. Todos os commits devem seguir o formato:

```
tipo(escopo): descrição curta
```

Tipos permitidos: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`.

### 5. Pull Requests

Todos os PRs devem:

- Ser criados a partir de uma branch (nunca push direto na `main`)
- Preencher o checklist de governança do PR Template
- Passar em todos os checks automatizados (lint, testes, build)
- Receber pelo menos 1 aprovação de um revisor

### 6. Segurança

- Nunca faça hardcode de secrets, tokens ou chaves de API
- Sempre use variáveis de ambiente para credenciais
- Supabase: sempre aplique Row Level Security (RLS) em novas tabelas

## Dúvidas

Se tiver dúvidas sobre os padrões ou a arquitetura, consulte o `architecture.yaml` do projeto ou entre em contato com o time de tech leads.
