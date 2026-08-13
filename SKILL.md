---
name: competitive-speech-writer
description: >
  Agent skill for writing competition-ready Indonesian speeches that are
  evidence-grounded, natural when spoken, rhetorically strong, optionally
  Islamic/civic/academic, and capable of strategic rhyme without sacrificing meaning.
---

# Competitive Speech Writer

## Mission

Create speeches that are strong in four layers:

1. **Landasan** — credible sources and accurate claims.
2. **Gagasan** — clear thesis and meaningful argument.
3. **Rasa** — emotion, relevance, and audience connection.
4. **Panggung** — rhythm, delivery, memorability, and performance.

A good speech must work when spoken aloud, not merely when read on paper.

---

# 1. Mandatory Source Gate

Before producing a complete competition-ready speech, require a **Source Pack of 3–5 sources**.

Accepted sources include:

- Qur'anic verses
- hadith
- tafsir
- religious books
- academic books
- journal articles
- official statistics
- government reports
- laws and regulations
- constitutional provisions
- historical documents
- official speeches
- credible institutional reports
- competition guidebooks
- other relevant primary or credible secondary sources

The user may provide sources as:

- uploaded files
- links
- screenshots
- excerpts
- book references
- verse/hadith references
- source notes

If the user's initial request doesn't include at least 3 sources, do NOT draft the speech yet. Stop after acknowledging the brief, and ask the user directly for 3–5 sources before writing anything. You may help by naming what *types* of source would fit this theme/mode (e.g. "buat tema ini biasanya pas kalau ada 1 ayat/hadis, 1 data resmi kayak BPS/kementerian, dan 1 lagi bebas — udah ada yang mau dipakai?") so the user has an easier time listing them. Wait for their reply before moving to Section 2.

**What counts as the user "giving" a source (search/fetch is allowed on these):**
- a link — fetch it and extract the relevant content
- a partial reference — "QS Al-Hujurat soal tabayyun", "hadits tentang lisan", "UU ITE" — search to find the exact verse number, wording, or article
- a named law/report/book without the exact citation — search to pin down the precise number, year, or quote
- anything else where the user has pointed at a specific topic, document, or reference, even loosely

In all of these, the user has already supplied the source — searching or fetching is just completing/verifying what they pointed to, not choosing it. Do this proactively, without a separate "may I search?" step.

**What is NOT allowed:** the agent deciding on its own initiative, with no topic/reference/link from the user at all, which verses/laws/statistics to use for the speech. That still requires either the user naming something first, or (per the paragraph below) the user explicitly asking the agent to find something from scratch — in which case any result is a proposal to confirm, not an accepted source.

If the user explicitly asks you to find a source from scratch (no topic given, e.g. "carikan ayat yang cocok"), you may search and propose 1–2 candidates — present them as a proposal for the user to confirm, not as an already-accepted part of the Source Pack.

Never fabricate references under any circumstance.

Three strong sources are better than five weak or irrelevant sources.

---

# 1B. This Gate Has No Bypass

Section 1 is a hard requirement, not a suggestion. There is no default mode, quick-trigger phrasing, or missing-tool situation that allows the agent to pick which verses/laws/statistics to use with zero direction from the user. Fetching a link or completing a partial reference the user already pointed to (see Section 1) is not a bypass — that's still the user providing the source, just letting the agent do the legwork of retrieving it. The bypass that's not allowed is the agent inventing a topic or reference on its own with nothing from the user to point to.

---

# 2. Source-First Workflow

Never write the speech first and attach references later.

Use this sequence:

**READ SOURCES → EXTRACT IDEAS → MAP SOURCES → DEFINE THESIS → BUILD ARGUMENT → WRITE → RHYME/PERFORMANCE PASS → VERIFY**

For each source, internally determine:

- type
- title/reference
- author/institution
- year if available
- strongest relevant idea
- intended speech function

Possible functions:

- opening hook
- moral foundation
- problem evidence
- historical analogy
- legal foundation
- supporting argument
- solution basis
- closing reflection

Do not display the internal map unless requested.

---

# 3. Source Discipline

Prefer:

1. primary sources
2. official institutions
3. peer-reviewed research
4. recognized books
5. credible secondary analysis

Never:

- fabricate Quran verses
- fabricate hadith
- fabricate laws
- fabricate statistics
- invent book quotations
- create fake experts
- attribute a claim to a source that was not consulted
- distort a source merely to improve rhetoric

When exact quotation wording is uncertain, paraphrase without quotation marks.

For sacred text, legal text, official statistics, and historical claims, accuracy is more important than rhyme.

---

# 3B. Quick Trigger — Format Is Flexible, the Sources Requirement Isn't

`REQUEST_TEMPLATE.md` and `SOURCE_PACK_TEMPLATE.md` are optional aids for users who want to plan everything up front. The agent must never require the user to fill either one out field-by-field — a single natural-language message covering both the brief and the sources is enough, e.g.:

> "Bikinin pidato tema kemandirian energi, 5 menit. Sumbernya: UU No. 30/2007 tentang Energi, data BPS soal rasio elektrifikasi, sama QS Al-A'raf ayat 56 soal larangan bikin kerusakan di bumi."

Extract theme, duration, and the source list directly from a message like that — don't ask the user to reformat it into the template. What "quick trigger" does NOT mean is that sources become optional: if that same message had arrived without any sources listed, Section 1 still applies in full — acknowledge the brief, then ask for the sources before drafting.

If missing brief details (duration, audience, tone) aren't sources-related, fill them with sensible defaults and state the assumption in one line — duration 5–7 minutes, audience = dewan juri dan hadirin, tone matched to the competition type implied by the theme. Only the Source Pack itself is never defaulted or skipped.

---

# 4. Understand the Brief

Identify:

- competition/event
- theme
- subtheme
- speaker
- audience
- duration
- language
- tone
- religious/secular context
- mandatory elements
- judging criteria
- guidebook constraints

If a guidebook is supplied, treat it as a binding constraint.

Ask only when a missing detail materially changes the output.
Otherwise make a reasonable assumption.

---

# 5. One Central Message

Before drafting, define one thesis:

> If the audience remembers only one idea, what should it be?

Every source, story, statistic, joke, analogy, and solution must support this thesis.

Avoid speeches with many ideas but no memorable center.

---

# 6. Default Speech Architecture

## Act I — Attention

### Signature Opening
Use one or more:

- pantun
- vivid scene
- provocative statement
- rhetorical question
- short audience interaction
- contextual humor
- cultural greeting
- striking contradiction

Win attention within the first 20–30 seconds.

Avoid generic openings unless protocol requires them.

## Act II — Connection

Briefly establish:

- greeting
- speaker identity
- title
- issue relevance

Then show the gap between:

**what should happen** and **what is actually happening**.

## Act III — Foundation

Introduce the strongest source:

- Qur'an/hadith for Islamic speeches
- law/constitution/policy for civic speeches
- research/data/theory for academic speeches

Do not merely quote it.
Interpret what it means for the present issue.

## Act IV — Argument

Develop 2–3 escalating arguments.

Recommended pattern:

**CLAIM → SOURCE → INTERPRETATION → REALITY → CONSEQUENCE**

## Act V — Solution

Give 2–4 concrete actions.

Each solution should have:

- memorable name
- clear meaning
- practical action
- explicit connection to the thesis

Avoid vague calls such as “meningkatkan kesadaran” without explaining how.

## Act VI — Climax

Increase rhetorical energy through:

- parallelism
- repetition
- contrast
- strategic rhyme
- shorter sentences
- audience address

## Act VII — Closing

Use:

**REFLECTION → ESCALATION → CALL TO ACTION → CALLBACK → FINAL LINE**

The emotional ending should come before ceremonial closing phrases.

---

# 7. Write for the Ear

Prefer language that is:

- natural when spoken
- easy to breathe through
- expressive but not excessive
- formal enough for the setting
- clear to the intended audience
- distinctive to the speaker

Avoid essay-like sentences that are too long or dense.

Use varied sentence length:

**LONG → MEDIUM → SHORT → PAUSE**

Example pattern:

> Kita membangun teknologi yang semakin cepat, semakin cerdas, dan semakin dekat dengan kehidupan manusia.

> Kemajuan itu luar biasa.

> Tetapi karakter?

> Itu tetap tugas kita.

---

# 8. Performance DNA

A competition speech should contain recognizable performance moments.

Possible elements:

- call-and-response
- rhetorical pause
- brief humor
- emotional silence
- change of tempo
- repeated phrase
- slogan
- regional expression
- dramatic contrast

Use only when they strengthen the message.

Do not turn every paragraph into a performance trick.

---

# 9. Humor Rule

Humor may be used when appropriate.

Good humor:

- fits the event
- is safe for the audience
- feels natural
- gives breathing room
- does not humiliate anyone
- does not destroy a serious emotional moment

Avoid forced memes or jokes that age badly unless intentionally topical.

---

# 10. Cultural Elements

When appropriate, use:

- regional greetings
- pantun
- local expressions
- Indonesian cultural references
- national identity

Use them accurately and intentionally.

Do not add cultural language merely as decoration.

---

# 11. Rhyme Engine

## Fundamental Rule

Prioritize:

**MEANING → ARGUMENT → NATURALNESS → RHYME**

Never sacrifice accuracy or clarity for rhyme.

Do not make the whole speech rhyme.

Use rhyme strategically in:

- opening
- transition
- slogan
- solution formula
- climax
- closing
- pantun

Normal explanatory sections may remain unrhymed.

Recommended progression:

**INFORMATION → RHYTHM → INFORMATION → RHYTHM → CLIMAX**

---

# 12. Rhyme Density

## Low Rhyme

Use for:

- statistics
- source interpretation
- legal discussion
- academic explanation

Prioritize clarity.

## Medium Rhyme

Use for:

- transitions
- argument emphasis
- audience engagement

Example:

> Teknologi bergerak semakin cepat, informasi datang semakin dekat, tetapi tanpa akhlak manusia justru dapat tersesat.

## High Rhyme

Use selectively for:

- opening
- climax
- slogan
- final call

Do not maintain high rhyme for long stretches.

---

# 13. Rhyme Bank

Before writing an important rhyming passage, internally form a small rhyme bank.

Example:

```text
CORE WORD:
inovasi

RHYME FAMILY:
generasi
literasi
kolaborasi
transformasi
adaptasi
kreasi
prestasi

RELATED IDEAS:
kemajuan
masa depan
teknologi
perubahan
penciptaan
```

Only use rhyme words that naturally fit the argument.

---

# 14. Rhyme Techniques

Use any of the following when natural:

### Strong rhyme
Similar final sounds.

### Near/slant rhyme
Sounds are close but not identical.

### Internal rhyme
Sound repetition inside a sentence.

### Parallel rhyme
Repeated grammar plus related endings.

### Semantic rhyme
Repeated structure and meaning, not only sound.

Example:

> Kita memiliki koneksi, tetapi kehilangan komunikasi.  
> Kita memiliki informasi, tetapi kehilangan verifikasi.  
> Kita memiliki teknologi—jangan sampai kehilangan empati.

### Rhyme chain
Use 3–4 related lines, then return to normal speech.

Do not make rhyme feel childish or forced.

---

# 15. Source-to-Rhyme Protection

Never change sacred, legal, or quoted text to make it rhyme.

Correct process:

**SOURCE → EXACT MEANING → INTERPRETATION → RHETORICAL PARAPHRASE → OPTIONAL RHYME**

Example:

> Prinsip tabayyun mengajarkan bahwa berita harus diperiksa sebelum dipercaya.

Then:

> Sebab satu kabar yang tak diteliti dapat berubah menjadi fitnah yang menyakiti.

The rhyme belongs to the interpretation, not the source.

---

# 16. Pantun Mode

When pantun is appropriate, use:

- 4 lines
- lines 1–2 as sampiran
- lines 3–4 as isi
- preferably A-B-A-B or a natural approximation

The isi must connect to the speech theme.

Avoid generic pantun that could be used in any speech.

---

# 17. Rhyme Revision Pass

Write the substantive draft first.

Then perform a dedicated **Rhyme & Performance Pass**.

Look especially at:

1. first 20–30 seconds
2. transition into the problem
3. transition into main argument
4. memorable solution
5. climax
6. final 30–45 seconds

Improve using:

- rhyme
- assonance
- consonance
- parallelism
- repetition
- sentence length
- strategic pauses

Do not rewrite factual meaning just to improve sound.

---

# 18. Anti-Forced-Rhyme Check

Remove rhyme when:

- wording becomes unnatural
- grammar becomes awkward
- meaning becomes vague
- the line exists only to complete a rhyme
- serious content becomes accidentally comedic
- the audience must work too hard to understand it

The audience should think:

> “Pidatonya enak didengar.”

Not:

> “Dia sedang memaksa semua kalimat berima.”

---

# 19. Memorable Concept

Whenever possible, create one memorable concept:

- 3-step formula
- acronym
- repeated phrase
- contrast
- slogan
- three-part action

Examples of structure:

- **SARING — JAGA — BAGIKAN**
- **3M**
- “Kita tidak hanya ... kita harus ...”
- “Iman tanpa inovasi..., inovasi tanpa iman...”

The device must arise from the argument, not replace it.

---

# 20. Islamic Speech Mode

For Islamic/Da'i-Da'iyah speeches, a strong default sequence is:

**Salam → Hamdalah → Shalawat → Greeting → Hook → Qur'an/Hadith → Interpretation → Contemporary Reality → Supporting Scholarship/History → Practical Solution → Social/National Connection → Climax → Closing**

Religion must function as moral and intellectual foundation, not ceremonial decoration.

Possible supporting sources:

- Quran
- hadith
- tafsir
- classical Islamic scholarship
- Islamic history
- credible modern research

---

# 21. Civic / National Speech Mode

Potential sources include:

- Pancasila
- UUD 1945
- laws
- government regulations
- BPS
- ministries
- development documents
- official national statistics
- historical records

Avoid empty nationalism.
Connect patriotic language to responsibility and action.

---

# 22. Academic Speech Mode

Use:

**DATA → HUMAN MEANING → ARGUMENT**

Do not read statistics like a report.

Instead of:

> Data menunjukkan X persen.

Prefer:

> Angka X persen terdengar seperti statistik. Tetapi ketika diterjemahkan ke kehidupan sehari-hari, artinya...

---

# 23. Anti-AI-Slope

Avoid repetitive generic phrases such as:

- di era yang serba digital
- di tengah derasnya arus globalisasi
- tidak dapat dipungkiri
- seiring perkembangan zaman
- marilah kita bersama-sama
- generasi penerus bangsa
- tantangan sekaligus peluang
- masa depan ada di tangan kita

These are not forbidden, but they must not become filler.

Prefer:

- specific imagery
- concrete language
- surprising contrasts
- speaker personality
- natural rhythm

---

# 24. Speaker Voice

The speech must sound like one identifiable person.

Possible voice styles:

- witty
- reflective
- energetic
- intellectual
- religious
- youthful
- patriotic
- calm
- provocative

Maintain one coherent personality.

Do not randomly switch tone.

---

# 25. Duration Control

Default Indonesian competition delivery rate:

**115–135 words per minute**

Suggested targets:

- 3 minutes → 330–390 words
- 5 minutes → 575–675 words
- 7 minutes → 800–945 words
- 10 minutes → 1,150–1,350 words

Reduce prose count when the speech contains:

- Arabic recitation
- audience response
- long pauses
- humor
- ceremonial elements

---

# 26. Performance Markers

If requested, add only useful markers:

- [pause]
- [tatap audiens]
- [lebih tegas]
- [perlahan]
- [senyum]
- [naikkan intonasi]
- [beri ruang respons audiens]
- [hening 2 detik]

Do not annotate every sentence.

---

# 27. Quality Gate

Before finalizing, check:

## Substance
- clear thesis
- claims grounded in sources
- relevant evidence
- meaningful interpretation

## Structure
- strong opening
- logical escalation
- coherent argument
- concrete solution

## Performance
- natural spoken rhythm
- memorable moments
- audience connection
- strategic rhyme

## Originality
- feels specific to this speaker
- not a generic AI speech
- does not copy reference speeches word-for-word

## Closing
- clear emotional resolution
- callback when appropriate
- memorable final line

---

# 28. Source Verification Gate

Before completing the speech, verify:

- 3–5 sources are available
- factual claims match the sources
- quotations are not fabricated
- verse/hadith references are correct based on supplied material
- laws/regulations are not invented
- statistics retain their proper context
- source meaning has not been distorted

If a claim cannot be verified, state uncertainty instead of inventing certainty.

---

# 29. Default User Input

Default: one natural-language message covering brief + sources is enough (see Section 3B). The structured template below is optional, for users who want to plan every field explicitly:

```text
COMPETITION:
THEME:
SUBTHEME:
SPEAKER:
AUDIENCE:
DURATION:
LANGUAGE:
TONE:
SPECIAL REQUIREMENTS:

SOURCE PACK:

SOURCE 1:
[upload/link/reference/excerpt]

SOURCE 2:
[upload/link/reference/excerpt]

SOURCE 3:
[upload/link/reference/excerpt]

SOURCE 4: optional
[upload/link/reference/excerpt]

SOURCE 5: optional
[upload/link/reference/excerpt]
```

The user does not need to explain how each source should be used.
The agent should determine that.

---

# 30. Default Output

Unless requested otherwise, return:

## Title
A strong speech title.

## Speech Script
Complete performance-ready speech.

## Sumber
List every source the user supplied (surah:ayah, hadith collection, law number, report name/year) with enough detail to verify independently, and briefly note how each was used in the speech. If the agent proposed any source that the user then confirmed (per Section 1's optional help), note that it was agent-proposed and confirmed by the user, and add: verify exact wording before using in an actual competition.

## Estimated Duration
Give an approximate spoken duration.

Do not expose internal chain-of-thought.

---

# 31. Editing Existing Speeches

When improving an existing speech, preserve the speaker's strongest identity.

Evaluate:

1. source strength
2. opening
3. thesis
4. audience interaction
5. humor
6. argument sequence
7. rhetorical devices
8. rhyme
9. memorable concept
10. solution
11. climax
12. closing
13. duration

Do not sterilize a lively competition speech into an academic essay.

---

# 32. Core Philosophy

A strong competitive speech should be:

**berisi ketika dibaca,  
berirama ketika dibicara,  
dan membekas ketika panggung telah usai.**

Evidence gives the speech authority.  
Rhetoric gives it energy.  
Personality gives it identity.  
Performance gives it life.
