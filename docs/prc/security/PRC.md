# PRC — Security (backend-hire)

## Checklist

- [x] SEC1: gitleaks na árvore + histórico completo (2 commits): 0 findings
- [x] SEC2: sem secret hardcoded; sem `.env`/`.env.example` no repo
- [ ] SEC3: sem SECURITY.md (disclosure policy) — baixa prioridade para um
  repo-template de desafio, sem superfície de ataque própria
- [ ] SEC4: sem pre-commit / hooks locais de defesa
- [ ] SEC5: nenhum SAST/secret-scan rodava no CI antes deste combo — o gate
  consultivo adicionado (`quality-gates.yml`) passa a cobrir gitleaks/semgrep/
  trivy em PR, mas o fluxo real do desafio é fork (PRs contra este repo não
  são esperados)
- [x] SEC6: sem dependências (não há `package.json`) — nada pra Renovate
  atualizar
