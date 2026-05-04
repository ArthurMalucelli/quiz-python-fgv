# Quiz Python · FGV

Treino para mini-prova de Fundamentos de Programação para Negócios (FGV EAESP, CGAE6). Cobre o conteúdo das Aulas 7-14.

**Live:** https://arthurmalucelli.github.io/quiz-python-fgv/

## Conteúdo

182 questões de múltipla escolha. Cada questão vem com gabarito e explicação curta com a regra do Python e a pegadinha quando tem. Compilado dos quizzes 1-7 do semestre, mais extras criadas no mesmo estilo.

| Tópico | Questões |
|---|---|
| tipos | 21 |
| conversao | 20 |
| operadores | 20 |
| listas | 20 |
| strings | 20 |
| condicionais | 20 |
| loops | 20 |
| comparacoes | 21 |
| funcoes | 20 |
| **Total** | **182** |

## Modos

- **Treino**: gabarito e explicação aparecem na hora que você responde.
- **Simulado**: timer configurável, score só no fim, breakdown por tópico e revisão dos erros.

## Filtros

- Por quiz original (1 a 7) ou extras (8).
- Por tópico.
- Quantidade ajustável.
- Embaralhar ordem das questões e das alternativas.

## Atalhos

`A` `B` `C` `D` ou `1` `2` `3` `4` para responder. `←` `→` para navegar.

## Stack

Single HTML estático. Sem build, sem framework, sem dependência de runtime.

- Cabinet Grotesk e Satoshi via Fontshare
- JetBrains Mono via Google Fonts
- Syntax highlighter Python em JS puro

## Rodar local

```bash
git clone https://github.com/ArthurMalucelli/quiz-python-fgv.git
open quiz-python-fgv/index.html
```

## Estrutura

Tudo num arquivo só (`index.html`). O array `QUESTIONS` contém todas as questões no formato:

```js
{
  id: "1.1",
  quiz: 1,
  topic: "tipos",
  q: "enunciado da pergunta",
  code: "snippet de código (opcional)",
  question: "pergunta após o código (opcional)",
  opts: ["A", "B", "C", "D"],
  correct: 2,
  exp: "explicação do gabarito"
}
```

Pra adicionar questão nova, edita o array e dá `git push`. GitHub Pages faz redeploy em ~30s.
