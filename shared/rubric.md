# Rubrica de Qualidade de Proposta — v1

Régua compartilhada pelas quatro skills do pack. Toda skill termina reescorando a
proposta nestas sete dimensões. O placar é o que torna a evolução visível: sem ele,
cada rodada produz opinião nova em vez de progresso medido.

**Escala**: 0 a 5 por dimensão. Total de 0 a 35.

**Portões de decisão**:

| Faixa | Estado | O que fazer |
|---|---|---|
| 0–20 | Rascunho | Não vale discutir em grupo ainda. Rode `proposal-attack` e `proposal-evidence`. |
| 21–27 | Revisável | Dá para circular para crítica. Ataque as duas dimensões mais baixas. |
| 28–35, nenhuma dimensão < 3 | Pronta para decisão | Pode ir para comitê, PRD ou pitch. |

Uma dimensão em 0 ou 1 bloqueia o portão mais alto mesmo que a soma passe de 28.
Uma proposta com evidência zero e escopo impecável não é uma boa proposta; é uma
boa redação de um palpite.

---

## Como pontuar

Leia a âncora de cada faixa e escolha a que descreve a proposta **como ela está
escrita**, não como o autor a defenderia numa conversa. Se a informação não está no
documento, ela não conta. Quando a proposta ficar entre duas faixas, dê a menor:
rubrica generosa não mede nada.

Registre sempre a **evidência textual** que justificou a nota — a frase, a seção ou
a ausência dela. Nota sem citação é opinião com número na frente.

---

## D1 — Clareza do problema

*Pergunta-teste*: dá para descrever o problema sem mencionar a solução proposta?

- **0–1**: O problema é enunciado como falta da solução ("os usuários não têm um
  dashboard"). Não há quem, nem quando, nem com que frequência.
- **2–3**: Há um problema real nomeado, mas genérico ou sem dono. Falta o segmento
  específico, a situação em que dói, ou a magnitude.
- **4–5**: Problema descrito com segmento, gatilho situacional, frequência e custo
  atual de conviver com ele. Um estranho conseguiria propor três soluções diferentes
  só lendo esta seção.

*O que separa 2 de 4*: em 2 o problema é uma categoria; em 4 é uma cena com pessoas
identificáveis fazendo algo identificável num momento identificável.

---

## D2 — Força da evidência

*Pergunta-teste*: em que degrau da escada abaixo está a evidência mais forte citada?

**Escada de força de evidência** (use o degrau mais alto que a proposta realmente apresenta):

| Degrau | Tipo | Vale |
|---|---|---|
| 0 | Opinião interna, intuição, "todo mundo sabe" | Nada |
| 1 | Analogia de mercado, concorrente faz, relatório de analista | Pouco |
| 2 | Dado de uso do próprio produto, ticket de suporte, telemetria | Médio |
| 3 | Entrevista com cliente sobre comportamento passado | Médio-alto |
| 4 | Teste comportamental — alguém fez algo que custou tempo, dinheiro ou reputação | Alto |
| 5 | Experimento controlado com grupo de controle e efeito medido | Muito alto |

- **0–1**: Só degraus 0 e 1. Ou cita números sem origem rastreável.
- **2–3**: Chega ao degrau 2 ou 3, mas a evidência sustenta o problema e não a
  solução — ou é seletiva (só o que confirma).
- **4–5**: Degrau 4 ou 5 para a premissa mais crítica, com o tamanho da amostra e o
  que **não** foi confirmado declarados abertamente.

*O que separa 2 de 4*: em 2 alguém **disse** que faria; em 4 alguém **fez** algo que
custou caro. Declaração não é comportamento.

---

## D3 — Resultado e métrica

*Pergunta-teste*: daqui a um trimestre, que número diz se isso deu certo — e quem o
olha hoje?

- **0–1**: Sem métrica, ou só métrica de entrega ("lançar em setembro"), ou vaidade
  pura (pageviews, cadastros).
- **2–3**: Métrica de resultado nomeada, mas sem linha de base, sem alvo, ou sem
  dizer em quanto tempo se espera mover.
- **4–5**: Métrica de resultado com valor atual, alvo, prazo e uma métrica de
  contrabalanço que impediria ganhar no papel e perder no produto.

*O que separa 2 de 4*: a linha de base. Alvo sem ponto de partida é ficção;
com ponto de partida, vira aposta verificável.

---

## D4 — Cobertura de risco

*Pergunta-teste*: os quatro riscos de Cagan estão endereçados — valor, usabilidade,
viabilidade técnica e viabilidade de negócio?

- **0–1**: Nenhum risco nomeado, ou só o técnico (o mais confortável de discutir).
- **2–3**: Dois ou três riscos nomeados, mas sem plano de teste para o mais grave.
  Riscos listados como parágrafo de rodapé, não como agenda.
- **4–5**: Os quatro percorridos, o mais letal identificado explicitamente, e um
  teste barato proposto para ele **antes** de qualquer construção.

*O que separa 2 de 4*: em 2 os riscos são declarados; em 4 são ordenados por
letalidade e o primeiro tem data.

---

## D5 — Espaço de solução

*Pergunta-teste*: quantas alternativas reais foram consideradas e por que caíram?

- **0–1**: Uma solução, apresentada como inevitável. Ou alternativas-espantalho,
  óbvias demais para serem sérias.
- **2–3**: Duas ou três alternativas listadas, mas descartadas por afirmação, sem o
  critério que as derrubou.
- **4–5**: Alternativas genuinamente distintas (incluindo "não fazer nada" e a
  versão 10x mais barata), com o critério explícito que selecionou a escolhida.

*O que separa 2 de 4*: o critério. Em 2 o autor diz que descartou; em 4 o leitor
consegue refazer a escolha sozinho e chegar ao mesmo lugar.

---

## D6 — Escopo e decidibilidade

*Pergunta-teste*: um leitor consegue dizer sim ou não sem pedir mais uma reunião?

- **0–1**: Sem fronteira. Tudo é "poderia incluir". Não há o que aprovar.
- **2–3**: Escopo positivo definido, mas sem não-escopo explícito — a parte que
  sempre volta a crescer entre a aprovação e a entrega.
- **4–5**: Escopo, **não-escopo nomeado**, critérios de aceitação verificáveis e a
  decisão específica que está sendo pedida a quem lê.

*O que separa 2 de 4*: a lista de não-escopo. É a seção mais barata de escrever e a
mais cara de omitir.

---

## D7 — Custo, apetite e reversibilidade

*Pergunta-teste*: quanto estamos dispostos a gastar antes de desistir, e quão caro é
voltar atrás?

- **0–1**: Sem estimativa, ou estimativa que só existe como prazo de entrega.
- **2–3**: Custo estimado, mas tratado como preço de um escopo fixo em vez de
  apetite — orçamento que vai estourar em vez de teto que corta escopo.
- **4–5**: Apetite declarado como teto de tempo/dinheiro com escopo variável, mais
  uma avaliação honesta de reversibilidade (o que fica preso depois: dados,
  contratos, promessa a cliente, dívida arquitetural).

*O que separa 2 de 4*: apetite é um teto que faz o escopo ceder; estimativa é um
piso que faz o prazo ceder. Só o primeiro protege a decisão.

---

## Formato do placar

Toda skill fecha com esta tabela, sem exceção:

```
| Dimensão | Nota | Evidência / lacuna |
|---|---|---|
| D1 Clareza do problema | 3 | Segmento nomeado, sem frequência |
| D2 Força da evidência | 1 | Degrau 1 — só analogia com concorrente |
| D3 Resultado e métrica | 2 | Alvo sem linha de base |
| D4 Cobertura de risco | 2 | Só risco técnico endereçado |
| D5 Espaço de solução | 1 | Solução única |
| D6 Escopo e decidibilidade | 3 | Falta não-escopo |
| D7 Custo e apetite | 2 | Estimativa, não apetite |
| **Total** | **14/35** | **Rascunho** |
```

Seguido de uma linha só: **o menor movimento que mais sobe o placar**.
