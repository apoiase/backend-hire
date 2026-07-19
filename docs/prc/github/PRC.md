# PRC — GitHub (backend-hire)

- Org: `apoiase`, repo GH-nativo (não é mirror de Bitbucket).
- Branch default: `master`. Branch desta task: `big-picture/NA-598-backend-hire`.
- Remotos: só `origin` (`git@github.com:apoiase/backend-hire.git`).
- Repo-template de teste de contratação backend: candidatos fazem fork e
  trabalham em branch `release/[NOME]` própria — nunca há push direto aqui.

## Checklist

- [ ] **PRC-GH1**: sem nenhum workflow de CI/CD (`.github/workflows/` não
  existia antes deste combo) — nada validava o fork do candidato antes da
  avaliação manual. Fora de escopo consertar (repo-template, não produto).
- [x] Gate consultivo adicionado por este combo
  (`.github/workflows/quality-gates.yml`, `continue-on-error` em todo step)
- [ ] PRC-GH2: sem PR template, sem CODEOWNERS — aceitável para um repo-template
  cujo fluxo real é fork, não PR contra este repo.
- [ ] PRC-GH3: branch default `master` (não `main`) — nomenclatura legada,
  sem urgência de correção (repo estático).
- [x] Gitleaks (árvore + histórico completo, 2 commits): 0 findings
