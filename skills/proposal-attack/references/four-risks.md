# Os Quatro Riscos

De Marty Cagan (SVPG). A tese: discovery existe para matar estes quatro riscos antes
da entrega, e projetos morrem porque atacaram o risco confortável em vez do letal.

Percorra os quatro sempre. Declarar "aqui não há risco de X porque Y" é útil — o Y
vira uma premissa explícita e atacável, que é exatamente o que se quer.

---

## 1. Risco de valor — as pessoas vão querer isto?

O mais fatal e o menos discutido, porque é o único que não se resolve com competência.

Perguntas de ataque:
- Que comportamento custoso alguém já teve que prova que este problema dói? (Pagar
  por um paliativo, montar uma planilha, ligar para o suporte repetidamente.)
- Qual é a alternativa atual do usuário — incluindo "conviver com o problema"? Por
  que ela é pior o suficiente para justificar mudar?
- Se a proposta diz que clientes pediram: pediram esta solução, ou descreveram um
  problema e alguém traduziu para esta solução? (Cliente pede solução; o trabalho é
  extrair o problema.)
- Quem perde algo se isto for adotado? Feature que não tira nada de ninguém
  geralmente não muda nada.

Sinal de perigo: a justificativa de valor é um número de mercado total ("TAM de
$4bi") em vez de um comportamento observado.

## 2. Risco de usabilidade — as pessoas vão conseguir usar?

Perguntas de ataque:
- Em que momento do dia do usuário isto aparece? Se não há gatilho natural, alguém
  precisa *lembrar* de usar — e não vai.
- Quantos passos até o primeiro valor? Quantos deles exigem que o usuário já entenda
  um conceito novo que a proposta está introduzindo?
- O que acontece com quem entra pela primeira vez e o sistema está vazio?
- Isto exige mudança de hábito de quem? Mudar hábito de quem tem incentivo é difícil;
  de quem não tem, é impossível.

## 3. Risco de viabilidade técnica — dá para construir com o que temos?

O mais confortável de discutir, então cuidado com o tempo gasto aqui em relação aos
outros três.

Perguntas de ataque:
- Qual a parte que ninguém no time já fez antes? É aí que a estimativa está errada.
- Que dependência externa precisa entregar no prazo para isto funcionar?
- O que isto exige em escala que hoje só funciona porque o volume é pequeno?
- O que fica difícil de mudar depois? Decisões de dados e de modelo de permissão são
  as mais caras de reverter.

## 4. Risco de viabilidade de negócio — o resto da empresa consegue conviver?

O mais esquecido. Feature tecnicamente pronta que a organização não consegue vender,
suportar ou cobrar é feature morta.

Perguntas de ataque, por função:
- **Vendas** — muda a conversa de venda? o time precisa aprender algo novo? muda o
  ciclo ou o contrato?
- **Suporte** — quantos tickets novos por mês isto cria? quem responde?
- **Financeiro / preço** — cobra-se por isto? está no plano atual ou cria upgrade?
  canibaliza receita existente?
- **Jurídico / compliance** — toca dado pessoal, residência de dados, requisito
  contratual, setor regulado?
- **Marca e promessa** — se isto for mal feito, o que quebra na percepção do produto?

---

## Ordenação

Depois de percorrer os quatro, nomeie **um** como o mais letal e justifique em uma
frase. Um ataque que devolve quatro riscos de peso igual não ajudou ninguém a decidir
o que fazer na segunda-feira de manhã.
