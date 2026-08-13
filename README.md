# Competitive Speech Writer

A reusable agent skill for producing **competition-ready Indonesian speeches** that are:

- evidence-grounded
- natural when spoken
- rhetorically strong
- capable of strategic rhyme
- suitable for Islamic, civic, national, and academic speech contexts
- resistant to generic AI-style writing

## Key Idea

This skill does **not** allow the agent to jump straight from a theme to a finished speech.

It uses:

**Source Pack → Thesis → Argument Map → Speech Draft → Rhyme & Performance Pass → Verification**

A complete competition-ready speech requires **3–5 source materials**.

Sources may include:

- Quran / hadith / tafsir
- books
- journals
- official statistics
- government reports
- laws and regulations
- historical documents
- competition guidebooks

## Repository Structure

```text
competitive-speech-writer/
├── SKILL.md
├── README.md
├── templates/
│   ├── REQUEST_TEMPLATE.md
│   └── SOURCE_PACK_TEMPLATE.md
├── references/
│   └── STYLE_PATTERNS.md
└── examples/
    └── EXAMPLE_REQUEST.md
```

## Installation / Usage

Use `SKILL.md` as the primary instruction file for your agent.

Depending on your coding/agent platform, you can:

- place the repository in your agent's skills folder
- import the `SKILL.md` instructions as a system/project skill
- copy the skill into your preferred agent framework
- keep this repository on GitHub and clone it into projects as needed

## Recommended Input

**Default (Quick Trigger):** one natural message covering both the brief and your sources, e.g. "bikinin pidato tema kemandirian energi, 5 menit, sumbernya UU No. 30/2007, data BPS rasio elektrifikasi, dan QS Al-A'raf 56." No template needed — but the 3–5 sources still have to come from you. If you don't include them, the agent will pause and ask before writing anything. See Section 3B / Section 1 in `SKILL.md`.

**Power-user mode:** use the template in `templates/REQUEST_TEMPLATE.md` to plan out every field (competition, subtheme, audience, tone, special requirements) explicitly ahead of time.

## Important Design Rule

Rhyme is added **after** the substantive argument is built.

The skill prioritizes:

**Meaning → Argument → Naturalness → Rhyme**

not:

**Rhyme → Meaning**

## References

The included `references/STYLE_PATTERNS.md` contains generalized stylistic lessons for competitive speechwriting.

It intentionally does not reproduce full reference speeches.

## License

Add a license that fits your intended use before publishing publicly.
