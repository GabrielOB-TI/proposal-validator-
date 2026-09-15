---
name: proposal-shape
description: Consolida material disperso sobre uma proposta de produto ou feature (SaaS) num documento decidivel — PRD, one-pager, pitch no formato Shape Up ou PR/FAQ da Amazon — com escopo, nao-escopo nomeado, criterios de aceitacao verificaveis e a decisao especifica que esta sendo pedida. Use quando o usuario disser "consolida isso", "escreve o PRD", "transforma em one-pager", "monta o pitch", "organiza pra levar pra reuniao" ou quando uma proposta ja atacada e validada precisar virar documento. NAO use para escrever copy de marketing nem documentacao de produto para usuario final.
---

# Proposal Shape

> **Estado: rascunho.** Fluxo definido, templates ainda nao escritos.

Antes de comecar, leia `${CLAUDE_PLUGIN_ROOT}/shared/rubric.md` — as dimensoes D6
(escopo e decidibilidade) e D7 (custo e apetite) sao o alvo desta skill.

Se a variavel `${CLAUDE_PLUGIN_ROOT}` nao expandir no seu ambiente, procure o arquivo `shared/rubric.md` na raiz do plugin instalado e leia de la.

## Escolha do formato

| Formato | Quando |
|---|---|
| One-pager | Decisao de seguir ou nao, cedo, com pouca informacao |
| PRD | Escopo acordado, precisa virar trabalho |
| Pitch Shape Up | Ha apetite fixo de tempo e o escopo deve ceder |
| PR/FAQ | Produto novo, e a duvida e se alguem vai se importar |

Na duvida, pergunte ao usuario em vez de assumir — o formato errado desperdica a
consolidacao inteira.

## Fluxo

1. Identificar a decisao que esta sendo pedida e para quem.
2. Escrever problema, resultado esperado e metrica com linha de base.
3. Escopo **e nao-escopo nomeado** — a lista de nao-escopo nao e opcional.
4. Criterios de aceitacao verificaveis (Given / When / Then).
5. Apetite como teto, riscos assumidos e o que fica irreversivel.
6. Escorar na rubrica e registrar no decision log.
