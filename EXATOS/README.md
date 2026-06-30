# Framework de Estudo com IA — Exatas (Física & Matemática)

**Complemento ao:** Método de Estudo com IA (guia genérico de 60 min)
**Perfil:** intuição física/geométrica primeiro, formalismo depois.
**Cobre três gaps distintos:** derivação, resolução de problemas novos, interpretação de resultados.

---

## Por que exatas é diferente

Em exatas, há três camadas que precisam estar alinhadas para o aprendizado ser sólido:

```
Intuição          →   "o que está acontecendo fisicamente/geometricamente?"
Formalismo        →   "como a matemática captura isso?"
Resolução         →   "como aplico em problemas que nunca vi?"
Interpretação     →   "o que esse número/resultado significa no mundo real?"
```

A maioria do ensino formal vai direto ao formalismo e pula a intuição. O resultado: você sabe manipular símbolos mas perde o fio quando o problema muda levemente. Essa framework reconstrói as quatro camadas em ordem.

---

## Estrutura por tipo de gap

Identifique qual gap está ativo no tema do dia e escolha o ciclo correspondente. Eles podem ser usados em sequência (para um tema novo do zero) ou isolados (quando você já tem parte do entendimento).

```
TEMA NOVO DO ZERO:
  Ciclo A (intuição) → Ciclo B (derivação) → Ciclo C (problemas) → Ciclo D (interpretação)

GAP ESPECÍFICO:
  Só o ciclo correspondente ao que está travando
```

---

## CICLO A — Intuição física ou geométrica

> Use antes de qualquer fórmula. O objetivo é construir a imagem mental que vai sustentar tudo que vem depois.

### 🔵 Prompt — Construção de intuição (ponto de entrada para qualquer tema)

```
Estou começando a estudar [CONCEITO, ex: "transformada de Fourier",
"tensor de inércia", "espaço de Hilbert"].

REGRA ABSOLUTA: não me mostre nenhuma fórmula ainda.

Primeiro, me faça uma pergunta sobre um fenômeno físico, geométrico
ou cotidiano que esse conceito está tentando descrever ou resolver.
Eu vou tentar articular o que está acontecendo com palavras, sem
matemática. Só depois que eu tentar, me diga se minha intuição está
na direção certa, parcialmente certa, ou apontando pro lugar errado
— e por quê. Só introduza o primeiro símbolo quando a imagem
mental estiver sólida.
```

---

### 🔵 Variação — Quando a intuição está bloqueada por abstração excessiva

> Use quando o conceito é muito abstrato e você não consegue nem formular a imagem mental.

```
Estou travado em [CONCEITO] porque não consigo visualizar do que
se trata. Parece abstrato demais.

Me dê uma analogia do mundo físico concreto (preferencialmente algo
que eu possa imaginar visualmente ou sentir) que capture a essência
do conceito — mesmo que a analogia seja imperfeita. Depois me
pergunte: onde essa analogia falha? Eu tento identificar o limite
da analogia sozinho antes de você apontar.
```

---

### 🔵 Variação — Geometria: quando precisa ver antes de calcular

```
Quero entender geometricamente [CONCEITO, ex: "produto vetorial",
"autovetor", "gradiente"].

Antes de qualquer cálculo: me descreva (ou me peça pra descrever)
o que está acontecendo no espaço. Onde estão os vetores? O que
o resultado representa geometricamente? Qual a direção, magnitude,
orientação? Só depois que eu conseguir descrever isso verbalmente,
me introduza a notação e o cálculo formal.
```

---

## CICLO B — Derivação e formalismo

> Use quando você entende a intuição mas não sabe de onde a fórmula vem — ou quando quer entender por que a matemática tem aquela forma específica.

### 🔵 Prompt — Derivação passo a passo (você propõe cada passo)

```
Quero entender de onde vem [FÓRMULA/EQUAÇÃO/RESULTADO].
Já tenho a intuição física: [DESCREVA SUA INTUIÇÃO EM 1-2 FRASES].

Não me mostre a derivação completa. Me dê só o ponto de partida
(a definição ou premissa mínima) e me peça pra propor o próximo
passo. Para cada passo que eu propor:
- Se estiver certo: confirme e peça o próximo.
- Se estiver errado: não me dê o passo certo. Me pergunte
  "por que você acha que esse passo funciona?" e me deixe
  identificar o erro sozinho. Só mostre o passo correto se eu
  não conseguir depois de 2 tentativas.

Continue até chegar na forma final.
```

---

### 🔵 Variação — Entender por que a matemática tem aquela forma (não só derivar)

```
Sei derivar [FÓRMULA], mas não entendo por que ela tem essa forma.
Por que esse termo aparece? Por que esse expoente? Por que essa
estrutura e não outra?

Não me explique direto. Me pergunte o que eu acho que cada parte
da equação está "fazendo" fisicamente ou geometricamente. Para cada
parte que eu não conseguir explicar, me faça uma pergunta menor que
me ajude a construir a resposta — não me dê a resposta.
```

---

### 🔵 Variação — Verificar se você realmente entendeu a derivação

```
Acabei de estudar a derivação de [FÓRMULA]. Vou te reproduzir de
memória, sem consultar o material:

[ESCREVA A DERIVAÇÃO DE MEMÓRIA, COM LACUNAS SE HOUVER]

Analise: onde minha derivação está correta, onde está imprecisa, e
onde está errada. Para cada erro, não me dê a versão certa — me
pergunte o que eu estava pensando naquele passo. Quero entender
onde meu modelo mental quebrou, não só onde o símbolo está errado.
```

---

## CICLO C — Resolução de problemas novos

> Use quando você sabe a teoria mas trava em problemas que nunca viu. O objetivo é desenvolver estratégia de ataque, não decorar tipos de problema.

### 🟢 Prompt — Problema novo com scaffolding socrático

```
Quero praticar [CONCEITO] resolvendo problemas que nunca vi.

Me dê um problema inédito de dificuldade [BÁSICA / INTERMEDIÁRIA /
AVANÇADA]. Não me dê dica de qual método usar.

Quando eu começar a resolver e travar:
- Não me dê o próximo passo.
- Me pergunte: "O que você sabe sobre o sistema nesse ponto?"
  ou "Que grandeza você precisa encontrar e o que a conecta
  ao que você já tem?"
- Só intervenha com uma dica direta se eu travar no mesmo
  ponto por mais de 2 tentativas.

Quando eu terminar, não me diga só se está certo ou errado.
Me pergunte como eu descreveria a estratégia que usei — quero
articular o método, não só o resultado.
```

---

### 🟢 Variação — Quando você resolveu mas não tem certeza do caminho

```
Resolvi esse problema de [CONCEITO]:

[COLE O PROBLEMA]

Minha solução:
[COLE SUA RESOLUÇÃO]

Não me diga se está certo ainda. Me pergunte por que escolhi cada
abordagem — por que essa lei, esse sistema de coordenadas, essa
simplificação. Para cada escolha que eu não conseguir justificar
bem, classifique: (a) escolha certa e bem justificada, (b) acerto
por intuição sem entender por quê, (c) escolha que deveria ser
revisitada. Para (b) e (c), me faça a pergunta que eu deveria ter
me feito antes de tomar aquela decisão.
```

---

### 🟢 Variação — Treino de identificação de tipo de problema (sem resolver)

> Útil quando você quer desenvolver o "faro" para reconhecer qual ferramenta usar.

```
Me dê 3 enunciados de problemas de [ÁREA, ex: "mecânica clássica",
"equações diferenciais", "eletromagnetismo"]. Não preciso resolver —
quero praticar identificar: qual conceito/lei/método esse problema
está pedindo e por quais pistas no enunciado chego a essa conclusão.

Para cada um, eu identifico o método e justifico. Você me diz se
identifiquei certo e, quando errar, me pergunta qual parte do
enunciado eu não processei corretamente.
```

---

## CICLO D — Interpretação de resultados

> Use quando você chega no número final mas não sabe o que ele significa fisicamente, ou quando o resultado "parece certo" mas você não consegue defendê-lo.

### 🟣 Prompt — Tradução resultado → significado físico

```
Resolvi um problema de [CONCEITO] e cheguei ao resultado:
[SEU RESULTADO, com unidades]

Antes de me dizer se está certo: me pergunte o que esse resultado
significa fisicamente. O que esse número representa no sistema?
Faz sentido em termos de ordem de grandeza? Se eu dobrasse [VARIÁVEL
X], o que deveria acontecer com o resultado — e isso é consistente
com o que a fórmula diz?

Quero verificar minha interpretação antes de verificar o cálculo.
```

---

### 🟣 Prompt — Análise de casos-limite (o teste mais poderoso em Física)

```
Obtive a expressão geral: [SUA FÓRMULA/RESULTADO]

Me faça analisar os casos-limite. Não me diga quais casos testar —
me pergunte: "Que casos extremos você testaria para verificar se
essa expressão faz sentido?" Eu proponho os casos, analiso o que a
fórmula prevê em cada um, e verifico se é fisicamente razoável.
Se eu não propuser um caso-limite importante, me pergunte:
"O que acontece quando [VARIÁVEL] vai a zero / infinito / assume
esse valor especial?" — mas só depois que eu tentar sozinho.
```

---

### 🟣 Prompt — Feynman invertido para exatas (fecha qualquer ciclo)

```
Vou te explicar [CONCEITO] do início ao fim: intuição, matemática
e o que o resultado significa. Você é um aluno curioso que nunca
viu isso, mas com bom senso físico. Seu papel:

1. Me interromper quando eu usar um símbolo sem explicar o que
   ele representa fisicamente.
2. Me perguntar "mas por que não poderia ser diferente?" quando
   eu apresentar uma escolha matemática sem justificar.
3. Me pedir um exemplo concreto se eu ficar abstrato demais.

No final, me diga qual parte da explicação foi sólida e qual
parte soou como "decoreba" — onde eu reproduzi sem entender.

Minha explicação:
[ESCREVA AQUI]
```

---

## Guia de uso rápido — qual prompt escolher

| Situação | Prompt |
|---|---|
| Tema completamente novo | Ciclo A → B → C → D em sequência |
| Sei o nome mas não consigo visualizar | Ciclo A — Construção de intuição |
| Conceito abstrato demais | Ciclo A — Analogia / limite da analogia |
| Sei a intuição, não sei de onde vem a fórmula | Ciclo B — Derivação passo a passo |
| Sei derivar mas não entendo a forma da equação | Ciclo B — Por que essa forma? |
| Travo em problemas novos | Ciclo C — Problema com scaffolding |
| Resolvi mas não sei se o caminho foi correto | Ciclo C — Verificação de estratégia |
| Chego no número mas não sei o que significa | Ciclo D — Tradução resultado → física |
| Quero verificar se a fórmula faz sentido | Ciclo D — Casos-limite |
| Quero fechar o tema e testar se entendi de fato | Ciclo D — Feynman invertido |

---

## Dicas específicas para exatas

- **Nunca aceite uma fórmula sem imagem.** Se você não consegue descrever em palavras o que a equação está dizendo sobre o sistema, a intuição ainda não está sólida. Volte ao Ciclo A antes de continuar.
- **Casos-limite são o teste mais honesto em Física.** Se a sua fórmula não recupera o caso simples que você já conhece quando um parâmetro vai a zero ou infinito, algo está errado — ou no cálculo, ou na intuição.
- **Dimensões e ordens de grandeza antes de calcular.** Antes de desenvolver qualquer conta, escreva as unidades esperadas do resultado e estime a ordem de grandeza. Isso filtra erros conceituais antes de virar erro de conta.
- **Separe erro de conta de erro conceitual.** Se você errou, identifique qual foi. Erro de conta é irrelevante para o aprendizado — erro conceitual precisa de um ciclo completo de revisão.