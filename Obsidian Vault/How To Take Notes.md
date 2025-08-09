---
title: Note-Taking Playbook (Obsidian)
tags: 
updated: 2025-08-09
---

# Note-Taking Playbook

**Goal:** short, useful notes you can remember and reuse.

## Quickstart (5 steps)
1. **Make a note** named after the topic/section.
2. **Capture (live):** write 5–8 bullets max (definitions, rules, patterns, pitfalls).
3. **Distill (after):** compress to 3–5 bullets + 1 tiny example or diagram.
4. **Drill:** add 3–10 flashcards (Q/A or cloze).
5. **Do:** one tiny exercise or check (what you’ll implement/solve today).

---

## Core Rules
- One idea per line. Bullets > paragraphs.
- Write only what you’d forget in 48h.
- Link related notes: `[[Term]]`, `[[Formula]]`, `[[API Pattern]]`.
- Tag for search: `#course #topic #type/concept|lecture|paper|problem`.
- When a note gets long, split into smaller concept notes.

**Write:** definitions, formulas, API shapes, steps, pitfalls, minimal examples.  
**Skip:** long quotes, screenshots of text, full code dumps (link to repo/file instead).

---

## Workflow

### Before (1 min)
- Title + tags.
- Write one **guiding question** you want answered.

### During (capture, ≤8 bullets)
- New terms (short defs).
- Key result/algorithm/formula.
- Pattern (shape of steps/calls).
- One pitfall/gotcha.
- One mini example.

### After (3–5 min)
- Trim to **Top 5 bullets (TL;DR)**.
- Add **flashcards** (Q/A or cloze).
- Add **Next actions** (1 small task you’ll do).

### Later (review)
- Review at **1 day → 3 days → 7 days**.
- If a card is hard, rewrite the related line clearer.

---

## Checklists

### Reading (book/paper)
- [ ] TL;DR 3–5 bullets  
- [ ] Assumptions & limits  
- [ ] One figure/equation explained in 2 lines  
- [ ] One application to try

### Lecture
- [ ] Date/topic/source  
- [ ] 3 key claims  
- [ ] 1 confusion → write as a question  
- [ ] “From board to code/homework”: what to implement/solve

### Problem-solving (math/CS)
- [ ] **Given / Goal / Plan / Work / Answer (units)**  
- [ ] Name theorem/formula used  
- [ ] Common mistake to avoid

### Coding/API
- [ ] Pattern/shape of calls  
- [ ] Minimal snippet (shape only)  
- [ ] Common errors + how to detect  
- [ ] Tiny test to prove it works

---

## Formatting Habits
- **Bold** concept word; keep the rest short.
- Put formulas on their own line.
- Use callouts for pitfalls:
> **Pitfall:** state persists; don’t rely on defaults.

---

## Flashcards (inline examples)
```
Q: What is OpenGL primarily?
A: A specification maintained by the Khronos Group.

Cloze: OpenGL is a {{c1::state machine}}; we {{c2::bind objects}} and draw with the {{c3::current state}}.
```
Tag card lines with `#card` if you want to filter them.

---

## Templates (copy these into new notes)

### 1) Concept Note
```markdown
---
title: {{Topic}}
source: {{Book/Lecture/Paper}}
tags: #type/concept #{{CourseOrTopic}}
date: {{date}}
---

## TL;DR (≤5 bullets)
- 

## Why it matters
- 

## Definition / Rule
- 

## Pattern / Algorithm (shape only)
1) 
2) 
3) 

## Example (tiny)
- Input → Output:
- Why it works (1 line):

## Pitfalls
- 

## Flashcards #card
- Q: 
- Cloze: {{c1::...}}
```

### 2) Reading Note (book/paper)
```markdown
---
title: {{Title}}
source: {{Citation or URL}}
tags: #type/reading #{{Field}}
date: {{date}}
---

## TL;DR (3–5 bullets)
- 

## Key claims → evidence
- 

## Diagram/Equation to remember
- 

## Limits / Assumptions
- 

## My takeaways / Applications
- 

## Flashcards #card
- Q:
- Cloze:
```

### 3) Lecture Note
```markdown
---
course: {{Course}}
topic: {{Topic}}
date: {{date}}
tags: #type/lecture #{{Course}}
---

## TL;DR
- 

## Examples from class
- 

## Board → Code / Homework
- 

## Confusions → Questions
- 

## Next actions (today)
- 
```

### 4) Problem / Worked Example
```markdown
---
tags: #type/problem #{{Course}} #{{Topic}}
---

**Given:**  
**Goal:**  
**Plan:**  
1)  
2)  
3)  

**Work:**  
-  

**Answer (with units & check):**  
-  

**Common mistake & fix:**  
-  
```

### 5) Coding / API Pattern
```markdown
---
tags: #type/api #{{Tech}}
---

## Pattern name
- When to use:
- Steps:
```c
// shape only
fnCreate(&id);
fnBind(TARGET, id);
fnConfigure(...);
fnUse(...);
fnUnbind(TARGET);
```
- Pitfalls:
- Minimal test to verify:
```

---

## Example: Good vs Bad (quick)
**Bad:** 3 paragraphs of prose.  
**Good:**  
- **Spec vs impl**  
- **Versioning rule**  
- **State machine**  
- **Action:** update drivers when behavior is weird.

---

## Review Schedule
- Day 1: 10 min on yesterday’s cards  
- Day 3 & 7: skim starred notes  
- Sunday: refine or archive 3 notes

---

## Abbreviations
def = definition, eq = equation, ex = example, pit = pitfall, thrm = theorem, impl = implementation
