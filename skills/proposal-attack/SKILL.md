---
name: proposal-attack
description: Ataque adversarial estruturado a uma proposta de produto ou feature (SaaS) — premortem, os quatro riscos de Cagan, steelman, inversão e caça a vieses, fechando com placar na rubrica de qualidade. Use sempre que o usuário apresentar uma proposta, PRD, one-pager, pitch, RFC ou ideia de produto e pedir crítica, revisão, "ataca isso", "que furos tem", "o que pode dar errado", "red team", "premortem", "seja o advogado do diabo", "me convença do contrário" ou "isso se sustenta?" — e também quando ele compartilhar uma proposta pedindo opinião geral sem nomear crítica, porque a primeira coisa útil a fazer com uma proposta é tentar derrubá-la. NÃO use para revisão de código, revisão de texto/copy, nem para propostas comerciais a clientes.
---

# Proposal Attack

Derrubar a proposta é o serviço. Uma proposta que sobrevive a um ataque honesto vale
mais do que uma proposta elogiada, e o momento mais barato para matá-la é agora —
antes de existir código, roadmap ou promessa a cliente.

O objetivo não é produzir desconforto. É produzir uma lista curta de coisas que, se
verdadeiras, tornam a proposta errada, ordenadas pelo que é mais barato descobrir.

## Antes de começar

Leia `${CLAUDE_PLUGIN_ROOT}/shared/rubric.md`. O ataque termina virando notas, e
conhecer as dimensões antes de ler a proposta ajuda a enxergar as lacunas certas.

Se a variavel `${CLAUDE_PLUGIN_ROOT}` nao expandir no seu ambiente, procure o arquivo `shared/rubric.md` na raiz do plugin instalado e leia de la.

Se a proposta não estiver no contexto — só foi mencionada — peça o texto antes de
atacar. Atacar uma reconstrução imaginada é o pior resultado possível: parece
rigoroso e não toca em nada real.

## Fluxo

### 1. Isolar a tese

Escreva em uma frase o que a proposta afirma, no formato:

> Acreditamos que **[quem]** vai **[fazer o quê]** porque **[por quê]**, e isso vai
> mover **[qual número]**.

Depois liste as **premissas de sustentação**: as afirmações que precisam ser
verdadeiras para a tese se sustentar. Separe as que a proposta declara das que ela
apenas **presume em silêncio** — as silenciosas costumam ser as letais, justamente
porque ninguém as escreveu para poder duvidar delas.

Se a tese não couber em uma frase, esse já é o primeiro achado: a proposta ainda não
sabe o que está propondo.

### 2. Steelman antes de atacar

Antes de qualquer crítica, escreva a versão mais forte da proposta — a defesa que o
autor mais competente faria, incluindo um argumento que ele talvez não tenha
percebido que tinha.

Isso não é cortesia. Atacar a versão fraca desperdiça a rodada: o autor descarta o
ataque como incompreensão e nada muda. Além disso, às vezes o steelman revela que a
proposta é melhor do que parecia, e o achado passa a ser "está mal escrita", não
"está errada" — dois problemas com correções completamente diferentes.

### 3. Premortem

Leia `references/premortem.md` e execute.

Em resumo: assuma que estamos 12 meses no futuro e a iniciativa fracassou de forma
inequívoca. Não pergunte *se* pode falhar — pergunte *por que falhou*. Gere de 8 a
12 causas concretas antes de filtrar qualquer uma; a primeira leva sempre traz as
óbvias, e as boas aparecem na segunda metade da lista.

### 4. Os quatro riscos

Leia `references/four-risks.md` e percorra os quatro: valor, usabilidade,
viabilidade técnica, viabilidade de negócio.

Percorra os quatro mesmo quando um parecer irrelevante — a declaração "aqui não há
risco de valor porque X" é ela própria uma premissa atacável, e normalmente uma das
boas. O risco mais confortável de discutir é o técnico; o mais frequentemente fatal
é o de valor.

### 5. Inversão e vieses

Leia `references/biases.md` e faça as duas passagens:

- **Inversão**: em vez de perguntar como fazer isso dar certo, pergunte o que
  garantiria o fracasso — e cheque se a proposta já está fazendo alguma dessas coisas.
- **Caça a vieses**: procure viés de confirmação, viés de sobrevivência, falácia do
  planejamento, custo afundado e ancoragem no que já foi construído.

### 6. Ordenar por letalidade × custo de verificação

Nenhum ataque vale sem esta etapa. Uma lista de vinte objeções é ruído; três
objeções ordenadas são uma agenda.

Para cada achado que sobreviveu, atribua:

- **Letalidade**: se isto for verdade, a proposta morre, encolhe ou só fica pior?
- **Custo de verificação**: dá para descobrir em uma tarde, numa semana, ou só
  construindo?

Ataque primeiro o que é **letal e barato de verificar**. O que é letal e caro vira
decisão explícita de risco assumido, não item de backlog. O que não é letal sai da
lista — mencionar é gentileza, priorizar é erro.

### 7. Escorar e registrar

Preencha a tabela da rubrica e escreva a entrada do decision log usando
`${CLAUDE_PLUGIN_ROOT}/templates/decision-log.md`.

## Formato da saída

Use exatamente esta estrutura:

```
## Tese
[uma frase]

## Premissas de sustentação
Declaradas: [lista]
Silenciosas: [lista]

## Steelman
[o melhor caso possível, 1 parágrafo]

## Os três ataques que importam
1. **[Título do ataque]** — [o que estaria errado] · Letalidade: alta/média/baixa ·
   Verificação: [como descobrir e em quanto tempo]
2. ...
3. ...

## Assumido, não atacado
[riscos letais mas caros de verificar — vão para decisão explícita, não para teste]

## Descartado
[objeções que levantei e derrubei, em uma linha cada — mostrar isto evita que
voltem na próxima reunião]

## Placar
[tabela da rubrica]

## O menor movimento
[uma frase]
```

## Regras que não cedem

**Ataque a proposta, nunca o autor.** "Esta premissa não tem evidência" é trabalho;
"quem escreveu isso não pensou" é ruído que faz o resto ser ignorado.

**Não fabrique evidência.** Se um ataque depende de um número que você não tem,
escreva o ataque como pergunta verificável e diga qual dado a resolveria. Inventar
uma estatística plausível para reforçar uma crítica destrói a confiança em todas as
outras.

**Nomeie o que mudaria sua opinião.** Cada ataque precisa vir com a observação que o
desarmaria. Crítica infalsificável não é rigor, é postura.

**Ataque forte não significa veredito.** Sua saída não é "aprovar" ou "rejeitar" — é
a lista do que precisa ser sabido antes de decidir. A decisão é de quem lê.

**Pare em três.** Se você encontrou quinze problemas, o trabalho é escolher os três
que mais mudam a decisão. Uma lista exaustiva transfere o trabalho de priorização de
volta para o autor, que é exatamente o trabalho que ele pediu para você fazer.

## Depois do ataque

Se a proposta caiu por falta de evidência → `proposal-evidence`.
Se caiu porque a solução é única e frágil → `proposal-expand`.
Se sobreviveu → `proposal-shape`.
