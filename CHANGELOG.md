# Changelog

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/).
Versionamento semântico.

Mudanças em `shared/rubric.md` são sempre *breaking* na prática: placares gerados
com rubricas diferentes não são comparáveis. Toda alteração de dimensão, de âncora
ou de corte de portão sobe a versão **minor** no mínimo, e a entrada aqui deve dizer
explicitamente se placares antigos continuam válidos.

## [Não lançado]

### A fazer
- Referências de `proposal-evidence` (assumption mapping, desenho de experimento)
- Referências de `proposal-shape` (templates de PRD, Shape Up pitch, PR/FAQ)
- Referências de `proposal-expand` (SCAMPER, How Might We)
- Revisar a rubrica depois de 5 propostas reais: remover dimensões que não
  discriminarem nada

## [0.1.0] — 2026-09-15

Primeira versão. Placares a partir daqui usam a rubrica v1.

### Adicionado
- `shared/rubric.md` — rubrica v1 com 7 dimensões (0–5), escada de força de
  evidência e três portões de decisão
- `templates/decision-log.md` — registro por rodada, entradas imutáveis
- `skills/proposal-attack` — completa: premortem (Klein), quatro riscos (Cagan),
  steelman, inversão, caça a vieses, ordenação por letalidade × custo de verificação
- `skills/proposal-evidence`, `skills/proposal-shape`, `skills/proposal-expand` —
  rascunhos com descrição calibrada e fluxo definido, sem `references/`
- Estrutura de plugin instalável: `.claude-plugin/plugin.json` e `marketplace.json`

### Notas
- Nenhuma skill foi testada em disparo real no Claude Code antes deste lançamento.
- `${CLAUDE_PLUGIN_ROOT}` tem falha conhecida de expansão em arquivos markdown; as
  skills trazem fallback para localizar `shared/rubric.md` manualmente.
