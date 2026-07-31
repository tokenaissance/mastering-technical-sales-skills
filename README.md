# Mastering Technical Sales — Claude Code Skill

A comprehensive Sales Engineering playbook skill for Claude Code, based on John Care's *"Mastering Technical Sales: The Sales Engineer's Handbook"* (4th Edition, Artech House, 2022).

## What it does

When you face a technical-sales situation, this skill ensures Claude:

- **Applies the book's named frameworks, not generic advice** — Three Behavioral Crimes (Tell/Accept/Guess), BANT/MEDDIC, FAB, RM+3KP, Demo GPS, Checkpoint Charlie, LACE, the Trust Equation, the Five Competitive Strategies, and more
- **Covers the full SE lifecycle** — qualification → discovery → business value → demos → POC → executive engagement → career growth
- **Maps every scenario to a chapter** — all **34 chapters** in 5 parts, from "The Four Roles" to "Final Words", with a lookup table that routes any situation to the right framework
- **Tailors depth to the situation** — a TL;DR + framework for single-topic questions, the full playbook for complex, multi-topic deals
- **Grounds the technical demo in business value** — Time/Money/People quantification, TCO/ROI/Emotional ROI, Follow the Money

## Eval Results

Tested across 5 real-world SE scenarios (first discovery call, CISO/CIO executive presentation, no-decision/status-quo competition, 120-page RFP go/no-go, multi-SE team meeting):

| Scenario | Without Skill | With Skill |
|----------|:---:|:---:|
| First discovery call | 3/5 | **5/5** |
| Executive presentation (CISO/CIO) | 2/4 | **4/4** |
| Status-quo / "no decision" competition | 3/4 | **4/4** |
| 120-page RFP go/no-go | 3/3 | **3/3** |
| Multi-SE team meeting | 2/3 | **3/3** |
| **Overall** | **70%** | **100%** |

The skill's biggest impact is mapping the situation to the book's named frameworks (RM+3KP, the Five Competitive Strategies, the Seven Sins of Team Selling) — without it, Claude gives competent but framework-free advice.

## Installation

### Option 1: Clone + symlink (recommended)

```bash
git clone https://github.com/tokenaissance/mastering-technical-sales-skills.git
ln -s "$(pwd)/mastering-technical-sales-skills/.claude/skills/mastering-technical-sales" ~/.claude/skills/
```

### Option 2: Copy

```bash
git clone https://github.com/tokenaissance/mastering-technical-sales-skills.git
cp -r mastering-technical-sales-skills/.claude/skills/mastering-technical-sales ~/.claude/skills/
```

### Option 3: In-repo (Claude Code)

Claude Code auto-detects skills under `.claude/skills/` in a project. If this repo is one you already work in, the skill is available with no extra step.

After installation, restart Claude Code. The skill triggers automatically when you ask about discovery calls, demos, presentations, objections, RFP responses, POCs, competitive positioning, or any sales engineering scenario.

## Example prompts

```
I'm a new SE and have my first discovery call with an e-commerce prospect tomorrow. What should I ask?

How should I structure a 20-minute security product presentation to a bank's CISO and CIO?

We keep losing deals to "no decision" — the prospect just sticks with the status quo. What strategies should I use?

We got a 120-page RFP and the rep says "just fill it all in." Is it wired? Should we respond?

Four SEs from different product teams are in one customer meeting next week. How do we keep it from being a mess?
```

## Skill structure

```
mastering-technical-sales/
├── SKILL.md       # 34-chapter playbook (5 parts) + framework lookup table
├── README.md      # Skill documentation
└── evals/
    └── evals.json # 5 verification scenarios
```

## The 34 chapters

| Part | Chapters | Key frameworks |
|------|----------|----------------|
| 1. The Role & The Sales Process | 1–4 | Four SE Roles, 10-Stage Sales Process, BANT/MEDDIC, RFP Go/No-Go & Myths |
| 2. Discovery & Business Value | 5–9 | Behavioral Crimes, Pain Types, BVD Quadrants, 3WM+M, Time/Money/People, FAB, Technical Account Plan & Coach |
| 3. Presenting, Demos & Storytelling | 10–16 | RM+3KP, Attention Curve, Delivery Skills, Checkpoint Charlie, Demo GPS, Remote Demo, Whiteboarding, Storytelling |
| 4. Proving Value, Trust & Executives | 17–21 | 7-Phase POC, LACE, Trust Equation, Executive Connection, TCO/ROI/Payback/Emotional ROI |
| 5. Career, Growth & Management | 22–34 | 30/90/180-Day Plan, Brand Statement, Partner Selling, Competitive Tactics, CRM, Compensation, SE→Sales, SME/Team Selling & Seven Sins, Hiring, DOG Framework, Metrics |

## References

- John Care, *Mastering Technical Sales: The Sales Engineer's Handbook*, 4th Edition (Artech House, 2022, ISBN 978-1-63081-872-2)

This skill is a study playbook summarizing the book's frameworks for use with Claude Code. The underlying text is copyrighted by its author; the skill organization and framework summaries are provided for personal and educational use.

## License

MIT (see [LICENSE](LICENSE)).
