# Política de Segurança — AmabileAI

## Reportando Vulnerabilidades

Se você encontrar uma vulnerabilidade de segurança em qualquer projeto da AmabileAI, por favor reporte de forma responsável. Não abra uma issue pública.

Entre em contato diretamente com o time de segurança através dos canais internos da organização.

## Padrões de Segurança

Todos os projetos da AmabileAI seguem os seguintes padrões obrigatórios:

1. **Secrets:** Nunca faça hardcode de secrets, tokens ou chaves de API no código-fonte. Sempre use variáveis de ambiente.

2. **Supabase:** Todas as tabelas devem ter Row Level Security (RLS) habilitado. A `service_role_key` nunca deve ser exposta no código do cliente.

3. **Dependências:** Mantenha todas as dependências atualizadas. O Dependabot está configurado para alertar sobre vulnerabilidades conhecidas.

4. **OWASP Top 10:** Todo código é revisado contra as vulnerabilidades do OWASP Top 10 pelo agente `security-reviewer` antes de ser integrado.
