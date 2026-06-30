# Framework de Prática com IA — Análise de Dados & Código (Jupyter)

**Complemento ao:** Método de Estudo com IA (sessões teóricas)
**Foco:** conectar o que você *fez* no código com o que a teoria diz que deveria acontecer.
**Ponto de partida:** dataset do professor, dataset que você buscou, ou sintético.

---

## O problema central que essa framework resolve

Você executa o código, o resultado sai, o notebook roda sem erro — mas fica a sensação de *"fiz funcionar, mas não sei por que funciona"*. Isso acontece porque a prática típica não tem um momento explícito de tradução entre código e teoria.

Essa framework insere esse momento em todo ciclo prático.

---

## O Ciclo Prático (adaptável ao tempo disponível)

```
1. Setup com intenção          (5 min, sem IA)
        ↓
2. Exploração solo             (tempo livre, sem IA)
        ↓
3. Checkpoint de tradução      (10-15 min, com IA)
        ↓
4. Revisão socrática           (10-15 min, com IA)
        ↓
5. Fechamento: "E se?"         (5-10 min, com IA)
```

A Fase 2 é aberta — você define quanto tempo tem. As fases com IA (3, 4, 5) cabem em ~30 min no total e podem vir depois de uma sessão longa de código.

---

## As 5 Fases em Detalhe

### Fase 1 — Setup com intenção (5 min, sem IA)

Antes de abrir o Jupyter, responda por escrito (pode ser comentário no notebook):

```
Tema: [CONCEITO QUE ESTOU PRATICANDO]
Dataset: [FONTE/DESCRIÇÃO]

O que eu espero ver nos dados antes de analisar:
→ [SUA HIPÓTESE]

Qual etapa da teoria eu espero "ver acontecer" nessa análise:
→ [ex: "quero ver a autocorrelação cair depois de diferenciar"]

O que eu ainda não entendo bem e quero que a prática esclareça:
→ [SUA DÚVIDA TEÓRICA ABERTA]
```

Isso parece simples, mas é o que separa "executar código" de "estudar com código".

### Fase 2 — Exploração solo (sem IA)

Trabalhe no Jupyter normalmente. Algumas regras:

- **Não chame a IA para bugs imediatamente.** Dê pelo menos 2 tentativas de resolver sozinho. Quando travar mais de 10 minutos num bug técnico puro (não conceitual), aí sim use IA — mas só para o bug, não para a análise.
- **Anote decisões que você tomou** e não tem certeza se estão certas (ex: "usei n_lags=10 mas não sei se é o certo aqui").
- **Anote resultados que te surpreenderam** — esses são os pontos de ouro para o Checkpoint.

### Fase 3 — Checkpoint de tradução (com IA) ← o coração da framework

Esse é o momento de tradução código → teoria. Use o **Prompt de Tradução** abaixo.

### Fase 4 — Revisão socrática (com IA)

A IA questiona suas decisões analíticas — não o código, mas o raciocínio por trás delas.

### Fase 5 — Fechamento "E se?" (com IA)

Perguntas de perturbação: o que mudaria nos resultados se um pressuposto fosse violado? Isso solidifica a teoria via contrafactual.

---

## PROMPTS

### 🔵 Prompt — Checkpoint de tradução (Fase 3)

> Use ao final de uma etapa significativa da análise (não precisa esperar o notebook inteiro terminar).

```
Acabei de fazer a seguinte etapa da minha análise:
[DESCREVA EM 2-3 FRASES O QUE VOCÊ FEZ NO CÓDIGO]

Resultado obtido:
[COLE O OUTPUT, GRÁFICO DESCRITO, OU MÉTRICA PRINCIPAL]

Decisões que tomei e não tenho certeza se foram certas:
[SUAS ANOTAÇÕES DA FASE 2]

Resultados que me surpreenderam:
[SUAS ANOTAÇÕES DA FASE 2]

REGRA: não me explique a teoria direto. Me pergunte primeiro o que
EU acho que está acontecendo do ponto de vista teórico — por que o
resultado saiu assim, o que o modelo/método "decidiu" por baixo dos
panos. Só depois que eu tentar explicar, corrija o que estiver errado.
```

---

### 🟢 Prompt — Revisão socrática de decisões analíticas (Fase 4)

```
Aqui estão as principais decisões que tomei nessa análise:
[LISTE 3-5 ESCOLHAS: parâmetros, método, transformação, visualização]

Para cada uma, não me diga se foi certa ou errada ainda. Me pergunte
por que eu tomei essa decisão e o que eu esperava que ela fizesse.
Depois que eu responder cada uma, classifique: (a) decisão sólida e
bem justificada, (b) decisão certa mas por razão errada, (c) decisão
que deveria ser revisitada. Para (b) e (c), me diga qual seria a
pergunta certa que eu deveria ter me feito antes de decidir.
```

---

### 🟡 Prompt — Quando travar num bug conceitual (não erro de sintaxe)

> Para bugs técnicos puros (sintaxe, versão de lib), use a IA diretamente. Este prompt é para quando o código roda mas o resultado parece errado ou não faz sentido.

```
Meu código roda, mas o resultado não faz sentido pra mim:

Código relevante:
[TRECHO]

Output atual:
[OUTPUT]

O que eu esperava ver:
[SUA EXPECTATIVA]

Por que acho que está errado:
[SEU RACIOCÍNIO]

Não me dê a correção direto. Me pergunte sobre os pressupostos que
estou fazendo — sobre os dados, sobre o método, sobre o que o
parâmetro X faz. Deixa eu identificar onde meu modelo mental está
errado antes de você confirmar.
```

---

### 🟣 Prompt — Fechamento "E se?" (Fase 5)

```
Terminei a análise de [TEMA/MÉTODO]. Me faça 2-3 perguntas do tipo
"e se" que perturbem os pressupostos que usei:

- "E se a distribuição dos dados fosse X em vez de Y?"
- "E se você tivesse usado o método A em vez do B?"
- "E se esse pressuposto que você assumiu fosse violado?"

Não me dê as respostas. Eu respondo cada "e se" e você só intervém
se meu raciocínio for fundamentalmente errado — e quando intervir,
aponte qual pressuposto teórico eu esqueci, não me dê a resposta pronta.
```

---

### 🟣 Prompt — Revisão do notebook completo (ao final de um exercício longo)

```
Finalizei meu notebook de [TEMA]. Vou te passar um resumo do que fiz:

[DESCREVA O FLUXO: EDA → limpeza → modelo → avaliação, em tópicos]

Principais resultados:
[MÉTRICAS OU CONCLUSÕES]

Faça o papel de orientador de TCC revisando meu trabalho. Não avalie
o código — avalie o raciocínio analítico: as escolhas que fiz fazem
sentido dado o objetivo? Há etapas que pulei que um analista sênior
questionaria? Há algo que eu concluí que os dados não suportam de
fato? Me faça as perguntas difíceis, uma de cada vez.
```

---

## Como integrar com o Guia Teórico (60 min/dia)

A prática não precisa caber no mesmo bloco de 60 min do estudo teórico. A sugestão é desacoplar:

| Tipo de sessão | Quando | Estrutura |
|---|---|---|
| Teórica | Diária (60 min) | Ciclo Sócrates do guia principal |
| Prática | 2-3x por semana (tempo livre) | Esse ciclo — Fases 2-5 depois de trabalhar no Jupyter |

O link entre as duas é a **Fase 1 desta framework**: antes de codar, você escreve qual conceito da sessão teórica está tentando ver na prática. Sem isso, as duas sessões ficam desconectadas.

---

## Dica de fluxo no Jupyter

Crie uma célula Markdown no topo de cada notebook de estudo com o template da Fase 1. Isso vira o seu "contrato de intenção" com o notebook — e também fica registrado se você precisar voltar ao exercício depois.

```markdown
## Setup com intenção

**Conceito praticado:** ...
**Dataset:** ...
**Hipótese antes de analisar:** ...
**O que quero ver a teoria "aparecer" aqui:** ...
**Dúvida teórica que espero resolver:** ...
```