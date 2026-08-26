# Product Thinking Quiz

A ten-question quiz on product thinking, based on the
[IDG Product Thinking pathway](https://www.idg.gov.sg/product-thinking/).

**Live:** <https://jethrophuah.github.io/quiz/>

## What it is

One file — `index.html` — with no frameworks, no build step, no backend and no
network requests. Clone it and double-click, or serve it from anywhere static.

Eight graded questions cover the pathway's core material:

| # | Topic | Source guide |
|---|---|---|
| 1 | Problems before solutions | [Understanding the Problem](https://www.idg.gov.sg/guides-and-resources/productthinking1/) |
| 2 | Outcomes over outputs | [Understanding the Problem](https://www.idg.gov.sg/guides-and-resources/productthinking1/) |
| 3 | The Five Whys | [Start With The Whys](https://www.idg.gov.sg/guides-and-resources/productthinking2/) |
| 4 | The 4Cs | [Craft a Clear Problem Statement](https://www.idg.gov.sg/guides-and-resources/productthinking3/) |
| 5 | SMART metrics | [Metrics](https://www.idg.gov.sg/guides-and-resources/productthinking4/) |
| 6 | Leading vs lagging indicators | [Metrics](https://www.idg.gov.sg/guides-and-resources/productthinking4/) |
| 7 | Assumptions and risks | [Assumptions and Risks](https://www.idg.gov.sg/guides-and-resources/productthinking5/) |
| 8 | Customer experience | [A Good Customer Experience](https://www.idg.gov.sg/guides-and-resources/productthinking6/) |

Each answer reveals an explanation and a link back to the guide it came from.
The final screen scores you out of 8, places you in a band, and lists the
questions you missed with their explanations again.

Two bonus questions follow the graded eight. They are scored and reported
separately, so getting them wrong never affects the /8.

## Filling in the bonus round

> **Note:** the two bonus questions currently ship as visible `[bracketed]`
> placeholders. They are meant to be replaced.

Open `index.html` and find the `BONUS ROUND` banner near the end of the
`QUESTIONS` array. Replace every bracketed string and set `answer` to the index
(`0`–`3`) of the correct option:

```js
{
  fun: true,
  topic: "Bonus round",
  question: "Which of these has Jethro actually done?",
  options: ["...", "...", "...", "..."],
  answer: 2,
  explanation: "..."
}
```

Nothing else needs changing — the bonus badge, the separate scoring and the
"Got it" / "Nope" wording all key off the `fun: true` flag.

## Notes

- The answer key is deliberately balanced across positions A–D so the quiz
  can't be gamed by always picking the same letter. If you reorder any
  options, remember to update the explanation text along with them.
- Light and dark themes both supported, following the viewer's OS setting.
- Correct and incorrect are never signalled by colour alone — a ✓ / ✗ glyph
  accompanies each.

Quiz content is adapted from the IDG Product Thinking pathway; the examples,
frameworks and quoted lines are theirs.
