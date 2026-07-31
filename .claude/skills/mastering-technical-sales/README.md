# Mastering Technical Sales — Claude Code Skill

A comprehensive Sales Engineering playbook skill, based on John Care's *"Mastering Technical Sales: The Sales Engineer's Handbook"* (4th Edition, Artech House, 2022).

## What This Skill Does

Provides all **34 chapters** of actionable SE frameworks covering every phase of the technical sales cycle. When triggered, Claude applies named frameworks from the book to your specific situation — not generic advice.

The chapter structure is grounded in the book's actual table of contents. Chapters 1–3 (The Four Roles, The Sales Process, Lead Qualification) are written directly from the source text; the remaining chapters follow the book's framework.

## Frameworks Included

| Category | Key Frameworks |
|----------|---------------|
| Role & Process | Four SE Roles, 10-Stage Sales Process, RFP Go/No-Go |
| Qualification | BANT, MEDDIC, Lead Quality |
| Discovery | Three Behavioral Crimes, BVD Quadrants, 3WM+M, Pain Types |
| Account Planning | Technical Account Plan, Finding a Coach |
| Pitching | RM+3KP, FAB, Attention Curve, Delivery Skills |
| Demos | Demo GPS, Checkpoint Charlie, Remote Demo "4 Knows" |
| Storytelling | Conversational Reference Story, Structure |
| Trust & Q&A | Trust Equation T=(C+R+I)/(S+P), LACE Strategy |
| Value | TCO, ROI, Payback, Time-to-Value, Emotional ROI, FinOps |
| Competition | Five Competitive Strategies, Reversing the Dirt |
| POC | 7-Phase POC Process |
| Executives | Executive Connection, 3-Slide Format, Follow the Money |
| Career | 30/90/180-Day Plan, Brand Statement, DOG Framework, Metrics, SME/Team Selling, SE→Sales |
| Team | Partner Enablement, Seven Sins of Team Selling |

## Installation

This skill lives in the repo at `.claude/skills/mastering-technical-sales/`. Claude Code auto-detects skills in `.claude/skills/`.

To install it globally for all projects, symlink or copy it to `~/.claude/skills/mastering-technical-sales/`.

## Skill Structure

```
mastering-technical-sales/
├── SKILL.md       # Main skill file — all 34 chapters
├── README.md      # This file
└── evals/
    └── evals.json # Test prompts for verification
```

## Source

Based on *Mastering Technical Sales: The Sales Engineer's Handbook*, 4th Edition by John Care (Artech House, 2022, ISBN: 978-1-63081-872-2).
