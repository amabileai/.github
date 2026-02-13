## Descrição

<!-- Descreva brevemente o que este PR faz -->

## Tipo de Mudança

- [ ] `feat`: Nova funcionalidade
- [ ] `fix`: Correção de bug
- [ ] `refactor`: Refatoração (sem mudança de comportamento)
- [ ] `docs`: Documentação
- [ ] `test`: Testes
- [ ] `chore`: Manutenção / configuração

---

## Checklist de Governança AmabileAI

### Pré-requisitos do Projeto
- [ ] Este repositório foi criado a partir do `template-frontend-react`
- [ ] O arquivo `architecture.yaml` existe e está preenchido
- [ ] O Issue Form de **Project Kickoff** foi preenchido (se projeto novo)

### Qualidade de Código
- [ ] Sem uso de `any`, `@ts-ignore` ou `as unknown as`
- [ ] Sem `fetch()` direto — usando `api-client.ts`
- [ ] Testes unitários criados ou atualizados
- [ ] Conventional Commits utilizados em todos os commits
- [ ] ESLint e Prettier passando sem erros

### Arquitetura
- [ ] Nenhum arquivo de governança foi modificado (`.eslintrc.cjs`, `tsconfig.json`, `architecture.yaml`, workflows)
- [ ] Componentes seguem o padrão: `src/components/NomeComponente/NomeComponente.tsx`
- [ ] Hooks seguem o padrão: `src/hooks/useNomeHook.ts`
- [ ] Tipos da API gerados a partir do `openapi.yaml` (não criados manualmente)

### Segurança
- [ ] Sem secrets, tokens ou chaves de API hardcoded
- [ ] Variáveis de ambiente utilizadas para credenciais
- [ ] Supabase RLS aplicado em novas tabelas (se aplicável)

---

## Screenshots (se aplicável)

<!-- Adicione screenshots aqui -->

## Observações

<!-- Informações adicionais para o revisor -->
