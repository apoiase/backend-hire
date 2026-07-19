# PRC — AWS (backend-hire)

Repo sem deploy AWS — enunciado de teste de contratação, sem `serverless.yml`,
sem SDK, sem referência a recurso em código de produto (o README cita AWS/Lambda
só como stack de referência esperada do candidato). Validado contra o
inventário da task NA-598 (Steampipe `sa_automation_ro`): **0 recursos**
com nome `backend-hire`/`backend_hire` (ver `docs/prc/scan/2026-07-18-scan.md`).

## Checklist

- [x] Nenhum recurso AWS órfão associado ao repo (confirmado no inventário)
- [x] Nenhuma credencial AWS em código/CI (gitleaks 0 findings)
- [ ] AWS1: se este template algum dia ganhar uma implementação de referência
  própria (branch `solution`?), este PRC deve ser regenerado com validação
  código→realidade
