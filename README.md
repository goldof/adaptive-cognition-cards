# Adaptive Cognition Cards

48 numbered mechanism cards from the [Adaptive Cognition Engine](https://github.com/goldof/xingnao-skill) （醒脑） — each card is a **minimum self-explanatory unit**: number, one-line mechanism, source, and boundary (when it doesn't apply).

Feed any card — image or text — to any LLM and it can explain it. No skill installation required.

- 中文版说明 → [README.zh-CN.md](README.zh-CN.md)

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

## License

CC BY-NC-SA 4.0 — share and adapt freely for non-commercial use, with attribution. See [LICENSE](LICENSE).

## Referencing the images

Every card's official image lives at a stable URL — reference it directly, no regeneration needed:

```
https://raw.githubusercontent.com/goldof/adaptive-cognition-cards/main/{zh|en}/png/xingnao-{NUMBER}.png
```

Example: `.../main/zh/png/xingnao-M01-01.png`. Each entry in `cards.json` also carries its own `image_url`.
