---
name: french-armenian-speaker
description: >
  Pronunciation guide system for French, specifically designed for speakers of Armenian, Russian, and Spanish.
  Use this skill whenever the user asks to learn French pronunciation, read French text aloud, break down French sounds,
  or build a pronunciation widget for any French text. Also trigger when asked to annotate French lyrics, poetry,
  or spoken word with phonetic guides. This skill encodes a custom three-alphabet system built for this language
  profile — do NOT improvise the sound mappings, always follow this skill.
---

# French Pronunciation for Armenian + Russian + Spanish Speakers

This skill encodes a custom phonetic system for learners who speak Armenian, Russian, and Spanish.
It uses all three alphabets — each doing only the job it's uniquely suited for.

---

## The Three-Alphabet System

### 1. Armenian ղ — for EVERY French R

The French R is a **voiced uvular fricative** — a gh friction sound made at the very back of the throat.

- **Use ղ** for every single French R, without exception
- NOT Armenian Ռ (too hard, almost a trill)
- NOT Armenian Ր (too soft, nearly disappears)
- NOT Russian Р (too sharp, too frontal — the most common mistake)
- NOT Spanish R (tongue tap — completely wrong direction)

The sound is the same as Armenian ղ as in **Ղազախ** or **ղեկ** — that gh rumble. Same as Arabic غ for those with exposure.

**Examples:**
- rêve → **ղԷՎ** (NOT РЭВ — that R would be wrong)
- Paris → **pa-ղi**
- prendre → **ղПОНДР** (ղ opens it, not a P-R cluster like Spanish)
- avoir → **a-ղWAղ** (ղ at start AND end)
- bonjour → **bon-ЖУղ**

### 2. Russian Cyrillic — for Ж, nasals, and vowel anchors

**Ж** → every French J sound and soft G (je, j'imagine, partagé, bonjour)
- French J = exactly Russian Ж. Already owned by any Russian speaker.
- je → **ЖУ**, j'imagine → **ЖА**-ma-**ЖИН**, partagé → pa-ղ-ta-**ЖЕ**

**Nasal vowels** — the hardest part of French for any learner:
- **АН** → French "an/en" nasals (mouth open, hum into nose): enfant, dans, avant
- **ОН** → French "on" nasal (lips slightly rounded): bon, fond, mon
- **КЮН / ЮН** → French "un" nasal — use Ю not У, it's a rounded front vowel closer to the French sound
  - quelqu'un → kel-**КЮН** (NOT КУН)
  - un rêve → **ДЮН** ղԷՎ (NOT ДУН — Ю is closer to the French U-nasal)
- **АН** → French "in/ain/ein" nasals: main, pain, vin

**Other Russian anchors:**
- РИСК, МОНД, СВИТ — words near-identical to Russian
- РЬ for the French soft R+Y combination (sérieux → seh-**РЬЁ**)

### 3. Spanish — for free vocabulary and vowel shapes

When a French word is near-identical to its Spanish equivalent, label it blue and note the shortcut.
- devenir ≈ devenir (ES)
- responsable ≈ responsable (ES)
- indifférence ≈ indiferencia (ES) — almost free
- manière ≈ manera (ES)

---

## Key French Sounds With No Direct Equivalent

### The French U (ü sound)
No clean anchor in any of the three languages. Closest approximation:
- Say Russian И but round your lips like you're whistling
- Write as **Ü** in the pronunciation line to flag it needs special attention
- humains → **Ü-МАН**

### Silent Letters — the French Betrayal
French endings are mostly decorative. Always flag these explicitly:
- Final T → always silent (conclut, est, fait)
- Final S → almost always silent (pas, les, des)
- Final E → ghost breath, barely there (lettre → let-ruh, just exhale)
- H → always silent (humains → **Ü-МАН**, not H-Ü-МАН)
- Final R in -er verbs → silent (parler → paղ-**ЛЕ**, not paղ-**ЛЕR**)

### The French Liaison (linking)
When a word ending in a silent consonant is followed by a vowel, the consonant reactivates:
- les humains → **leh-zÜ-МАН** (the S of les links to humains)
- Always note liaisons explicitly in the pronunciation line

---

## Output Format

When producing a pronunciation guide, always build it as an interactive HTML widget using the visualizer tool.

### Pronunciation line format
Write the pronunciation line using the three-alphabet system inline:
- Armenian letters (ղ) in **green** for R sounds
- Russian Cyrillic in **red** for Ж, nasals, and vowel anchors
- Spanish hints in **blue**
- Silent letter warnings in **yellow/note pills**

### Per-line structure
For each French line or phrase:
1. **French text** — original, serif font, large
2. **Pronunciation line** — colour-coded three-alphabet system, mid-size
3. **Meaning** — English translation, muted
4. **Pills** — specific sound notes, anchored to the three languages

### Legend
Always include a legend at the top of any widget:
- green / Armenian → ղ for every French R
- red / Russian → Ж, nasals, vowel anchors
- blue / Spanish → near-free words
- yellow → silent letters and traps

### Footer rule
Always end the widget with a one-sentence reminder of the core system.

---

## Common French Words — Pre-Annotated

| French | Pronunciation | Notes |
|--------|--------------|-------|
| rêve | **ղԷՎ** | ղ = Armenian gh, ԷՎ clean |
| je | **ЖУ** | Russian Ж, exactly |
| aujourd'hui | oh-**ЖУR**-**ДВИ** | learn as one block, never split |
| au fond | oh-**ФОН** | nasal ФОН, "deep down" |
| quelqu'un | kel-**КЮН** | nasal КЮН, Ю not У |
| d'un | **ДЮН** | Ю not У — rounded front vowel |
| un | **ЮН** | same — Ю not У |
| avoir | a-**ղWAղ** | ղ both sides |
| bonjour | bon-**ЖУղ** | Ж + ղ at end |
| partagé | paղ-ta-**ЖЕ** | ղ middle, ЖЕ end |
| prendre | **ղПОНДР** | starts with ղ |
| suite | **СВИТ** | exactly English "sweet" |
| âme | **ДАМ** | soul — like Russian дама |
| sérieux | seh-**РЬЁ** | Russian soft РЬ+Ё |
| manière | ma-**ղyЕR** | ղ replaces the R |
| défendre | deh-**ФАНДղ** | final R = ղ, barely voiced |
| s'engager | sahn-ga-**ЖЕ** | Russian ЖЕ landing |
| poursuivre | pooղ-**СВИВР** | UI collapses to СВИ |
| humains | **zÜ-МАН** | H silent, liaison from les |
| mystérieusement | mees-teh-**ղyuhz**-**МОН** | ղ in middle, МОН nasal end |

---

## Rules to Never Break

1. **Never use Russian Р for French R.** Always ղ. The whole system breaks if this slips.
2. **Always use Ю not У for the French un nasal.** ДЮН not ДУН.
3. **Always mark silent letters** — never assume the learner will know. Explicit pill every time.
4. **Flag liaisons** — they're invisible in writing and trip up every learner.
5. **One alphabet per job** — don't mix Armenian and Russian for the same sound type.
6. **R at end of words** — always ղ, often barely voiced. Don't skip it, don't overdo it.

---

## When to Use This Skill

- Any French text the user wants to read aloud
- French lyrics, poetry, or spoken word
- Single words or phrases the user encounters and wants to pronounce correctly
- Building pronunciation reference widgets for French content to study repeatedly
- Any time the user asks "how do I pronounce X in French"

Always produce the full widget with colour-coded pronunciation lines. Never just write a flat phonetic string — the colour coding is what makes this system work.
