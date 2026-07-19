# CLAUDE.md — backend-hire

Repositório-template do **teste de contratação para vagas de backend** na
Apoia.se. Não é código de produto: é o enunciado do desafio (README) mais
uma licença MIT — o candidato faz fork, cria a branch `release/[SEU-NOME]` e
implementa a aplicação por conta própria. Nada aqui é implantado em produção.

## Comandos

Não há manifesto de build/teste neste repo (sem `package.json`, sem código).
O candidato define suas próprias ferramentas no fork.

## Arquitetura

- `README.md` — enunciado: apresentação da empresa, stack de referência
  esperada (Node.js, GraphQL, REST, MongoDB, Lambda, AWS) e o desafio em si:
  CRUD (REST ou GraphQL) de uma collection `users`
  (`id`, `firstName`, `lastName`, `dateBirth`).
- `LICENSE` — MIT, copyright APOIA.se.
- `.gitignore` — padrão Node.js/Serverless, antecipando a stack que o
  candidato vai usar (mesmo sem nenhum código commitado aqui).
- Critérios de avaliação: funcionamento, boas práticas, clareza dos commits,
  cobertura mínima de testes.

## Contexto de domínio

Sem termos de negócio da Apoia.se (Fazedor/Apoiador/Repasse) — é um teste de
contratação genérico de backend, não integrado ao domínio de crowdfunding.
Referência completa do domínio, se precisar contextualizar a entrevista:
apoiase-context-layer (ler sob demanda — não duplicar aqui).

## Convenções

- Commits do rollout NA-598 em português natural, primeira pessoa,
  contendo `NA-598` no texto.
- Branch do rollout: `big-picture/NA-598-backend-hire`.
- Fluxo real deste repo é **fork**, não PR contra `master` — um PR aberto
  aqui é só o artefato do rollout de mapeamento (NA-598), não um fluxo de
  contribuição esperado.
- PR só via review humano — nunca merge por API.

## Knowledge graph

- `graphify-out/graph.html` (interativo) · `GRAPH_REPORT.md` (auditoria) —
  grafo pequeno e honesto: 4 nós extraídos do próprio enunciado do README
  (desafio, stack de referência, collection `users`, critérios de avaliação).
- `.understand-anything/knowledge-graph.json` (layers, tour) — query via
  `/understand-chat`.
- `docs/prc/scan/2026-07-18-scan.md` — validação código→realidade: 0 recursos
  AWS com o nome do repo (esperado, repo sem deploy próprio).
