# .github — AmabileAI

Este repositório contém os arquivos padrão da organização **AmabileAI** que são herdados automaticamente por todos os repositórios da organização.

## Arquivos Incluídos

| Arquivo | Função |
|---------|--------|
| `PULL_REQUEST_TEMPLATE.md` | Template padrão para Pull Requests com checklist de governança |
| `CONTRIBUTING.md` | Guia de contribuição com regras e padrões obrigatórios |
| `SECURITY.md` | Política de segurança e como reportar vulnerabilidades |
| `.github/ISSUE_TEMPLATE/bug-report.yml` | Template para reportar bugs |
| `.github/ISSUE_TEMPLATE/feature-request.yml` | Template para solicitar features |
| `profile/README.md` | Perfil público da organização no GitHub |

## Como Funciona

Quando um repositório na organização `amabileai` não possui seu próprio arquivo (por exemplo, `PULL_REQUEST_TEMPLATE.md`), o GitHub automaticamente utiliza o arquivo correspondente deste repositório como fallback.

Isso garante que **todos os repositórios** — incluindo os criados sem usar o template oficial — possuam um nível mínimo de governança e padronização.

## Governança Completa

Para governança completa (pipeline de CI/CD, guardrails de código, instruções para IAs), novos projetos devem ser criados a partir do template [`template-frontend-react`](https://github.com/amabileai/template-frontend-react).
