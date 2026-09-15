# proposal-validator

Pack de skills para Claude Code que ataca, valida, expande e consolida propostas de
produto e feature (SaaS).

A aposta do pack: **evoluir não é uma skill, é a rubrica mais o decision log**. Cada
skill termina reescorando a proposta nas mesmas sete dimensões e gravando uma
entrada no log. A evolução emerge do uso, sem custar uma skill extra.

## Instalação

```bash
git clone <seu-repo> proposal-validator
```

No Claude Code, a partir do diretório onde você clonou:

```
/plugin marketplace add ./proposal-validator
/plugin install proposal-validator
```

Ou, depois de publicar no GitHub:

```
/plugin marketplace add SEU_USUARIO/proposal-validator
/plugin install proposal-validator
```

Antes de publicar, troque `SEU_NOME` em `.claude-plugin/plugin.json` e
`.claude-plugin/marketplace.json`.

## Estrutura

```
proposal-validator/
├── .claude-plugin/
│   ├── plugin.json          manifesto do plugin
│   └── marketplace.json     catálogo (permite instalar direto do repo)
├── shared/
│   └── rubric.md            ← a régua. As quatro skills leem este arquivo.
├── templates/
│   └── decision-log.md      ← o histórico. Uma entrada por rodada.
└── skills/
    ├── proposal-attack/     COMPLETA
    │   ├── SKILL.md
    │   └── references/
    │       ├── premortem.md
    │       ├── four-risks.md
    │       └── biases.md
    ├── proposal-evidence/   rascunho
    ├── proposal-shape/      rascunho
    └── proposal-expand/     rascunho
```

## Como usar

As skills disparam por linguagem natural — não é preciso invocá-las pelo nome.

| Você diz | Dispara |
|---|---|
| "ataca essa proposta", "que furos tem", "premortem" | `proposal-attack` |
| "isso se sustenta?", "como eu testo", "qual a premissa mais arriscada" | `proposal-evidence` |
| "que alternativas existem", "estou preso numa solução só" | `proposal-expand` |
| "consolida isso", "escreve o PRD", "monta o pitch" | `proposal-shape` |

Fluxo típico: atacar → buscar evidência para o que caiu → expandir se a solução se
mostrou frágil → consolidar quando sobreviver. Não é linear e não precisa ser: o
placar diz onde está o buraco e, portanto, qual skill chamar em seguida.

## Estado

`proposal-attack` está pronta para uso real. As outras três têm fluxo definido e
descrição calibrada, mas ainda sem as referências — funcionam, com menos
profundidade. A rubrica é v1 e foi feita para ser editada: as dimensões que não
discriminarem nada depois de cinco propostas reais devem sair.
