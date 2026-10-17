# Adaptive Cognition Cards

48 numbered mechanism cards from the [Adaptive Cognition Engine](https://github.com/goldof/xingnao-skill) （醒脑） — each card is a **minimum self-explanatory unit**: number, one-line mechanism, source, and boundary (when it doesn't apply).

Feed any card — image or text — to any LLM and it can explain it. No skill installation required.

- 中文版说明 → [README.zh-CN.md](README.zh-CN.md)

## Project background

The Adaptive Cognition Engine （醒脑） is a decision-making skill built on behavioral economics, evolutionary psychology, and game theory. It was developed through a daily practice: one plain-language thinking lesson each morning, drawn from six modules and 48 mechanisms. These cards are the distilled, citable form of that mechanism library — designed so that **a single card seen once gives any AI the full project context**: what the engine is, how the 48 mechanisms are numbered, and the rule that numbers are never reused or reordered. Every card image carries this repo's URL at the bottom for exactly that reason.

## Layout

```
adaptive-cognition-cards/
├── README.md / README.zh-CN.md
├── LICENSE               # CC BY-NC-SA 4.0
├── zh/                   # 中文版
│   ├── cards.json        # machine-readable, 48 cards
│   ├── cards.md          # text version (paste into any LLM)
│   └── png/              # 48 illustrated cards (1080×1440)
└── en/                   # English version
    ├── cards.json
    ├── cards.md
    └── png/
```

## Cite by number

Cards are cited by number, e.g. **M06-06** (Kill Your Own Consensus). Numbers are a contract: **new mechanisms only ever get new numbers — existing numbers are never reused or reordered.**

| Number | Name |
|--------|------|
| M01-01 – M01-06 | Bargaining & Anchoring |
| M02-01 – M02-05 | Persuasion Framing |
| M03-01 – M03-06 | Sunk Costs & Strategic Quitting |
| M04-01 – M04-03 | Beating Cognitive Friction |
| M05-01 – M05-04 | Interrupting Rumination |
| M06-01 – M06-06 | The Anti-Consensus Engine |
| M07-01 – M07-04 | Cognitive Science |
| M08-01 – M08-04 | Statistical Thinking |
| M10-01 – M10-03 | History of Science (falsification cases) |
| M11-01 – M11-07 | Classical Decision Wisdom |

## Why the "Boundary" box matters

Principles are public goods — any model already knows them. What travels with the card and can't be copied from a textbook is the **boundary**: the one line that says when the principle *doesn't* apply. That's the part worth citing.

## Adaptive: make the set your own

These 48 cards are seeds, not the ceiling. "Adaptive" works on three levels:

1. **Analyze with cards**: for any event or scenario, pick 1–3 relevant cards and dissect it with "mechanism + source + boundary". E.g. a viral product blowup: cite M08-02 (Base-Rate Neglect), then M06-06 (Kill Your Own Consensus). Cards are handles for analysis, not answers.
2. **Fork and grow your own numbers**: fork this repo and add cards in the same format. One iron rule: new cards only ever take new numbers (continuing from M12), existing numbers are never reused or reordered. Your cards and mine can cite each other.
3. **Build your own skill**: feed cards.md to your AI assistant and tell it "when analyzing, pick cards first, cite numbers, then check the boundary box" — that's a minimum viable cognition skill. The text is free; running it is yours.

Principles are public goods; numbers are yours. The value isn't the number 48 — it's the format "one number, one mechanism, one boundary". The format is the skeleton; the content can grow without limit.

## License

CC BY-NC-SA 4.0 — share and adapt freely for non-commercial use, with attribution. See [LICENSE](LICENSE).

## Referencing the images

Every card's official image lives at a stable URL — reference it directly, no regeneration needed:

```
https://raw.githubusercontent.com/goldof/adaptive-cognition-cards/main/{zh|en}/png/xingnao-{NUMBER}.png
```

Example: `.../main/zh/png/xingnao-M01-01.png`. Each entry in `cards.json` also carries its own `image_url`.
