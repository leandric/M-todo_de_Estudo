# Método de Estudo com IA — Guia Genérico (60 min/dia)

**Para:** qualquer disciplina ou tema que você esteja estudando de forma acadêmica/autodidata.
**Objetivo:** usar a IA como tutora socrática e geradora de problemas — não como atalho de explicação.
**Formato:** ciclo comprimido para caber em uma sessão diária de 1 hora por tema.

---

## Por que esse método existe

Ler ou ver vídeo é exposição passiva: você reconhece o conteúdo, mas a memória de recuperação fica fraca. O que de fato fixa aprendizado é **esforço de recuperação ativa** — ser forçado a produzir a resposta, não apenas reconhecê-la.

Por isso, a regra de ouro em todos os prompts abaixo é: **a IA nunca entrega a explicação de cara**. Ela pergunta, você responde, ela só corrige quando você de fato travar ou errar a lógica.

---

## O Ciclo de 60 Minutos

```
1. Pré-leitura ativa         (10 min, sem IA)
        ↓
2. Sessão Sócrates            (25 min, com IA)
        ↓
3. Aplicação prática           (15 min, com IA)
        ↓
4. Fechamento / Feynman        (10 min, com IA)
```

Esse é o padrão para a maioria dos temas. Em temas muito teóricos (sem componente prático óbvio), funda a Fase 3 dentro da Fase 2 e use o tempo extra para mais perguntas de verificação.

### Fase 1 — Pré-leitura ativa (10 min, sem IA)
Leia o trecho/veja o vídeo curto no ritmo rápido — não busque entender tudo agora. Anote em duas colunas curtas:
- O que acho que entendi
- O que não fez sentido / onde travei

Isso ativa esquema prévio e dá munição pra Fase 2. **Não pule esta fase** — sem ela, a sessão de IA vira passiva de novo.

### Fase 2 — Sessão Sócrates (25 min, com IA)
Use o **Prompt-Mestre Sócrates**. Cole suas anotações da Fase 1 como contexto inicial. Esta é a fase mais longa porque é onde o entendimento de fato se forma.

### Fase 3 — Aplicação prática (15 min, com IA)
Peça um problema, caso ou exercício curto pra aplicar o que acabou de discutir. Não precisa ser código — pode ser um caso, um cálculo, uma argumentação, dependendo da disciplina.

### Fase 4 — Fechamento / Feynman (10 min, com IA)
Você explica o conceito em poucas frases como se a IA não soubesse nada. Ela aponta lacunas. Termina com 1-2 perguntas de verificação rápida.

---

## PROMPTS GENÉRICOS

> Troque `[TEMA]` pelo assunto do dia. Os exemplos entre parênteses são apenas ilustrativos — apague-os ao usar.

### 🔵 Prompt-Mestre Sócrates (Fase 2 — use em qualquer disciplina)

```
Estou estudando [TEMA] de forma acadêmica/autodidata.

O que eu já entendi (minhas anotações da leitura):
[COLE SUAS ANOTAÇÕES]

O que não fez sentido pra mim:
[COLE SUAS DÚVIDAS]

REGRAS PARA VOCÊ:
1. NÃO me dê a explicação direto. Me faça perguntas progressivas
   (do mais simples ao mais complexo) pra eu construir o raciocínio
   sozinho.
2. Só me corrija quando eu errar de fato — e quando corrigir, aponte
   EXATAMENTE onde minha lógica quebrou, sem repetir a teoria toda.
3. Tenho apenas 25 minutos para esta fase. Seja direto: poucas
   perguntas bem escolhidas, não um questionário extenso.
4. Nos últimos minutos, me dê 2-3 perguntas de verificação que eu
   devo responder sem hesitar antes de seguir.

Comece com a primeira pergunta.
```

### 🔵 Variação — Quando você suspeita que está só reconhecendo padrão, não entendendo

```
Estou estudando [TEMA]. Quero que você seja rigoroso: a cada resposta
que eu der, classifique se foi (a) raciocínio genuíno, (b) reconheci-
mento de padrão sem entendimento real, ou (c) chute. Diga a categoria
antes de seguir para a próxima pergunta, e se for (b) ou (c), me leve
um passo atrás até eu reconstruir o raciocínio sozinho.
```

### 🔵 Variação — Conectar com algo que você já domina (transferência de analogia)

```
Estou aprendendo [TEMA NOVO]. Já tenho domínio sólido de [ÁREA QUE
VOCÊ JÁ CONHECE BEM, ex: "Física", "lógica de programação", "futebol"].

Antes de qualquer explicação formal, me pergunte: isso te lembra de
algo nessa área que eu já domino? Eu tento mapear a analogia sozinho.
Só depois que eu tentar, diga se a analogia é sólida, parcial ou
enganosa — e por quê.
```

### 🔵 Variação — Destrinchar um processo, fórmula ou argumento passo a passo

```
Quero entender a lógica/derivação de [CONCEITO]. Não me mostre o
caminho completo de uma vez. Me dê o ponto de partida (a premissa
básica) e peça que eu proponha o próximo passo. Eu proponho, você
valida ou corrige SÓ aquele passo, e seguimos. Em cada passo errado,
pergunte "por que você acha que esse passo está certo?" antes de
corrigir.
```

---

### 🟢 Prompt — Aplicação prática (Fase 3, qualquer disciplina)

```
Acabei de estudar [TEMA]. Me dê um problema, caso ou exercício curto
(resolvível em 10-15 minutos) que me force a aplicar o conceito na
prática — não apenas recitar a teoria.

Requisitos:
- Contexto realista e específico (não genérico)
- Se fizer sentido para o tema, inclua uma "pegadinha" ou nuance que
  só quem entendeu de fato vai perceber — mas NÃO me diga qual é.
- Me dê só o problema. As etapas de resolução são minhas.

Depois que eu resolver, aponte se identifiquei a nuance e onde meu
raciocínio foi sólido ou frágil.
```

### 🟢 Variação — Problema com viés prático/profissional (quando o tema tem aplicação no seu trabalho/área)

```
Tema: [TEMA]. Quero um caso de aplicação no contexto de [SUA ÁREA,
ex: "dados/engenharia de dados", "negócios", "pesquisa acadêmica"].
Me dê o cenário e o objetivo, sem solução. Depois que eu resolver,
questione minhas escolhas como um revisor sênior questionaria —
não apenas se está certo, mas se foi a abordagem mais adequada.
```

---

### 🟣 Prompt — Fechamento Feynman (Fase 4, qualquer disciplina)

```
Vou te explicar o conceito de [TEMA] em poucas frases, como se você
não soubesse nada do assunto. Seu papel: me interromper toda vez que
eu usar um termo sem definir, pular uma etapa lógica, ou usar uma
analogia capenga. Seja exigente. No final, me diga em uma frase se
você, como "aluna", realmente entendeu ou só ouviu palavras bonitas.

Minha explicação:
[ESCREVA AQUI, 3-5 FRASES]
```

### 🟣 Prompt — Verificação rápida (alternativa mais curta ao Feynman, quando o tempo apertar)

```
Estudei [TEMA] hoje. Me dê 2 perguntas de verificação rápida — uma
conceitual e uma de aplicação. Não me dê o gabarito. Eu respondo as
duas, e só depois você diz o que acertei e por que errei o que errei.
```

---

## Dicas de uso

- **60 minutos é o teto, não a meta.** Se um tema precisar de menos, ótimo — use o tempo sobrando para revisão espaçada de um tema anterior.
- **Resista à vontade de pedir a resposta direto.** Se travar e quiser só a resposta, peça — mas registre mentalmente "não dominei isso" e volte ao tema em outra sessão.
- **Varie o contexto dos problemas práticos** (Fase 3) para não memorizar o cenário em vez do conceito.
- **Um prompt, um tema por sessão.** Não tente cobrir dois assuntos na mesma sessão de 60 min — a profundidade cai.
- **Para temas muito teóricos/abstratos** (filosofia, teoria pura), funda Fases 2 e 3: troque a "aplicação prática" por mais uma rodada de Sócrates com um caso hipotético ou contra-argumento.

---

## Sugestão de bloco único no Google Calendar

| Minuto | Fase |
|---|---|
| 0–10 | Pré-leitura ativa (sem IA) |
| 10–35 | Sessão Sócrates (com IA) |
| 35–50 | Aplicação prática (com IA) |
| 50–60 | Fechamento / Feynman (com IA) |

Um único evento de 60 min por tema/disciplina já cobre o ciclo inteiro — não precisa quebrar em dois blocos no dia.
