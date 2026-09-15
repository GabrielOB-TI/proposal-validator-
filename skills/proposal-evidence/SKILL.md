---
name: proposal-evidence
description: Mapeia as premissas de uma proposta de produto ou feature (SaaS) em importância x evidencia, classifica a evidencia existente numa escada de 0 a 5 e desenha o teste mais barato para a premissa mais arriscada (assumption mapping de Bland/Osterwalder, Riskiest Assumption Test, Opportunity Solution Tree). Use quando o usuario perguntar "isso se sustenta?", "como eu testo isso?", "que evidencia temos?", "qual a premissa mais arriscada", "como valido antes de construir" ou quando uma proposta precisar provar algo antes de virar roadmap. NAO use para analise estatistica de experimento ja rodado.
---

# Proposal Evidence

> **Estado: rascunho.** Fluxo definido, referencias ainda nao escritas.

Antes de comecar, leia `${CLAUDE_PLUGIN_ROOT}/shared/rubric.md` — em especial a
escada de forca de evidencia na dimensao D2.

Se a variavel `${CLAUDE_PLUGIN_ROOT}` nao expandir no seu ambiente, procure o arquivo `shared/rubric.md` na raiz do plugin instalado e leia de la.

## Fluxo

1. **Extrair premissas.** Liste tudo que precisa ser verdade, separando desejabilidade
   (alguem quer), viabilidade tecnica (da pra fazer) e viabilidade de negocio (a
   empresa consegue conviver).
2. **Mapear em dois eixos.** Importancia (se for falsa, a proposta morre) x evidencia
   (o quanto ja sabemos). O quadrante importante-e-desconhecido e a agenda; o resto e
   ruido por enquanto.
3. **Classificar a evidencia de cada premissa** na escada de 0 a 5 da rubrica,
   citando a fonte concreta de cada nota.
4. **Desenhar o teste mais barato** para a premissa do topo: o que observar, com
   quantas pessoas, em quanto tempo, e o criterio de aprovacao definido ANTES de
   rodar.
5. **Escorar** na rubrica e registrar no decision log.

## Regra central

O teste precisa ser falseavel. Se nenhum resultado possivel faria a gente mudar de
ideia, nao e um teste — e uma cerimonia.
