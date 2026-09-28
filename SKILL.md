---
name: expert-os
version: 1.0.0
description: Research, reconstruct, and package an expert's public body of work into a source-grounded operating system that can later be invoked as a reusable decision lens.
triggers:
  - create expert os
  - build expert os
  - expert os
  - reverse engineer expert
  - make a lens for
  - build a persona for
  - study everything by
---

# Expert OS

## Purpose

Expert OS reverse-engineers a public expert's body of work into a reusable operating system.

The goal is not to create a biography, fan summary, quote collection, or imitation.

The goal is to reconstruct:

- core beliefs
- mental models
- frameworks
- formulas
- processes
- decision rules
- heuristics
- metrics
- examples
- contradictions
- evolution over time
- evidence quality
- criticism
- situation → advice mappings
- a callable reasoning lens

The resulting OS should be useful for asking:

> "How would this expert analyze this problem, based on their documented public ideas?"

Always distinguish:

- DIRECT POSITION
- PARAPHRASE
- SYNTHESIS
- INFERENCE

Never present the result as literal impersonation.

---

# Activation

Activate this skill when the user asks to:

- create an Expert OS
- reverse-engineer an expert
- study an expert's whole body of work
- turn an expert into a reusable lens
- build a decision-making persona from public material
- reconstruct an expert's frameworks
- create a skill/persona from an expert's public corpus

Examples:

- `Create Expert OS for Alex Hormozi`
- `Build an Expert OS for Rory Sutherland`
- `Reverse engineer Andrew Huberman`
- `Make me a reusable operating system for Seth Godin`
- `Study Naval and turn his worldview into a callable lens`

---

# Core principle

Do not ask the model to "summarize everything."

Treat this as a corpus-reconstruction problem.

The workflow is:

```text
Expert
  ↓
Public corpus
  ↓
Source ledger
  ↓
Atomic claims
  ↓
Deduplication
  ↓
Taxonomy
  ↓
Frameworks / rules / processes
  ↓
Contradictions / evolution
  ↓
Evidence audit
  ↓
Situation → advice engine
  ↓
Callable Expert OS
```

Do not claim completeness unless the corpus actually supports that claim.

---

# PHASE 1 — Corpus Discovery

Research the expert's public material.

Prioritize:

1. Official YouTube channel
2. Official podcast
3. Books
4. Articles/newsletters
5. Talks
6. Interviews
7. Official website/course material
8. Social posts containing substantive ideas
9. Interviews on other people's channels
10. Primary documents from companies or institutions tied to the expert

Avoid relying primarily on:

- SEO summaries
- quote websites
- fan accounts
- unsourced listicles
- generic AI summaries

Create a source ledger:

| Source | Date | Format | Topic | Primary/Secondary | Importance | Retrieval status |
|---|---|---|---|---|---|---|

If the corpus is too large for a single pass, say so and batch it.

Never pretend the entire corpus was processed if it was not.

---

# PHASE 2 — Fallback ingestion with Agent Reach

If ordinary web retrieval cannot adequately access the expert's YouTube or Instagram material, use Agent Reach as a fallback capability pattern:

https://github.com/Panniantong/agent-reach

Relevant routes:

## YouTube
Use yt-dlp for:
- video search
- subtitle extraction
- transcript retrieval where available

## Instagram
Use OpenCLI with an existing browser login session, or an official Graph API route where applicable.

Important:

Agent Reach is an ingestion layer only.

After content is retrieved, continue with:

- source attribution
- atomic extraction
- dating
- deduplication
- contradiction detection
- evidence assessment

Never claim to have parsed a source unless the underlying content was actually retrieved.

If login/session access is required, do not imply it exists unless it is actually available.

---

# PHASE 3 — Atomic Knowledge Extraction

Do not summarize too early.

Extract ideas at the smallest useful unit.

Capture:

- claims
- principles
- heuristics
- rules
- mental models
- processes
- frameworks
- formulas
- recommendations
- warnings
- exceptions
- tactics
- strategies
- examples
- analogies
- definitions
- predictions
- beliefs
- decision rules
- checklists
- measurements
- thresholds
- routines
- protocols
- sequences
- cause → effect relationships

For each atomic idea record:

**Idea**  
What is being claimed?

**Meaning**  
Plain-English interpretation.

**When it applies**  
Context or conditions.

**When it does NOT apply**  
Exceptions or limits.

**Source**  
Where it came from.

**Date**  
When it was said/published.

**Confidence of attribution**  
High / medium / low.

**Repeated?**  
One-off or recurring?

**Changed over time?**  
Yes / no / unclear.

**Related concepts**  
Links to other ideas.

Preserve granularity.

Do not collapse ten distinct claims into one vague paragraph.

---

# PHASE 4 — Deduplication

Experts repeat ideas constantly.

Do not count repetition as a new idea.

Deduplicate by underlying concept, not wording.

For each repeated idea track:

- number of appearances
- earliest known appearance
- latest known appearance
- strongest primary source
- whether wording changed
- whether the underlying meaning changed

Use frequency as evidence of importance, not as a reason to duplicate entries.

---

# PHASE 5 — Build the taxonomy

Organize the expert's body of work into a hierarchy that emerges from the corpus.

Preferred structure:

```text
Domain
  → Subdomain
    → Principle
      → Framework
        → Tactic
          → Example
```

Show the taxonomy as a tree.

Do not force textbook categories if the expert's actual work suggests a different structure.

---

# PHASE 6 — Core beliefs / intellectual primitives

Identify the small number of beliefs that generate many downstream recommendations.

For each:

1. Belief
2. Why the expert appears to believe it
3. Which recommendations emerge from it
4. Which other ideas depend on it
5. Where it recurs
6. Whether the expert ever contradicts it

Then produce:

- worldview in 10 sentences
- worldview in 1 sentence

---

# PHASE 7 — Mental Model Library

For each recurring mental model:

### Name
### Explanation
### Input
### Reasoning process
### Output
### Example
### Failure mode
### Source

Where useful, show relationships between models.

Use diagrams only when they clarify the logic.

---

# PHASE 8 — Framework Library

For every framework:

## Framework name

**Problem it solves**

**Inputs**

**Steps**

**Decision criteria**

**Output**

**Example**

**Common mistakes**

**When NOT to use it**

**Source**

If algorithmic, add pseudocode.

---

# PHASE 9 — Decision Rulebook

Extract IF → THEN logic.

Examples:

- IF X happens → do Y
- IF metric drops below X → investigate Y
- IF customer says X → respond with Y
- IF choosing between A and B → evaluate C first

Group rules by situation.

The rulebook should be usable in real-world decisions.

---

# PHASE 10 — Processes and Playbooks

For each repeatable process provide:

**Goal**

**Prerequisites**

**Inputs**

**Steps**

**Decision points**

**Failure states**

**Metrics**

**Expected outcome**

**Examples**

**Sources**

Use flowcharts where they materially improve comprehension.

---

# PHASE 11 — Metrics and thresholds

Extract every metric, signal, benchmark, threshold, diagnostic, or measurement the expert cares about.

Use:

| Metric | Why it matters | Good | Bad | Action triggered | Source |
|---|---|---|---|---|---|

Never invent numerical thresholds.

If no explicit threshold exists, write:

**No explicit threshold found.**

---

# PHASE 12 — Contradictions

Actively search for conflicts.

Look for:

- changed advice
- abandoned ideas
- context-dependent differences
- beginner vs advanced advice
- old vs new positions
- public contradictions

Use:

| Topic | Position A | Position B | Dates | Possible explanation |
|---|---|---|---|---|

Do not force reconciliation.

Preserve genuine contradiction.

---

# PHASE 13 — Evolution Timeline

Show how the expert's thinking changed over time.

Include:

- major ideas introduced
- ideas revised
- ideas abandoned
- new frameworks
- changes caused by new evidence
- shifts in priorities
- changes in target audience or role

Distinguish chronology from interpretation.

---

# PHASE 14 — 80/20 + overlooked ideas

Produce two separate lists:

## Highest-leverage ideas
The small number of ideas that explain most of the expert's practical value.

## Overlooked ideas
Important ideas that are less famous, less viral, or less quoted.

Do not confuse popularity with importance.

---

# PHASE 15 — Beginner → Expert Curriculum

Build:

### Level 0 — Knows nothing
### Level 1 — Foundations
### Level 2 — Competent
### Level 3 — Advanced
### Level 4 — Expert
### Level 5 — Independent creator/operator

For each level provide:

- concepts
- skills
- exercises
- things to ignore
- common mistakes
- readiness test

---

# PHASE 16 — Situation → Advice Database

Create a retrieval layer:

> If I am facing [problem], what would this expert tell me to examine?

For each situation provide:

1. likely diagnosis
2. questions the expert tends to ask
3. relevant principles
4. relevant framework
5. recommended process
6. sources

Always label whether the advice is:

- Directly stated
- Strong synthesis
- Weak inference

---

# PHASE 17 — Expert Simulator / Callable Lens

Derive the expert's reasoning style without impersonating them.

Create:

### When presented with a problem, they tend to ask:
1.
2.
3.
4.
5.

### They prioritize:
1.
2.
3.

### They are skeptical when:
1.
2.
3.

### Their default decision logic:
[process]

### Their characteristic blind spots:
[limitations]

Then define invocation triggers.

Examples:

- `Hormozi`
- `Ask Rory`
- `Call Musk`
- `Use the Naval lens`
- `What would [EXPERT] examine here?`

When invoked later, re-read the current conversation through this lens.

Do not pretend the expert personally reviewed the situation.

---

# PHASE 18 — Knowledge Graph

Map:

- parent concepts
- child concepts
- dependencies
- reinforcing loops
- conflicts
- causal chains

Use Mermaid where useful.

Do not create decorative graphs.

---

# PHASE 19 — Formula Library

Extract every explicit formula, equation, score, model, or quantitative relationship.

For each:

**Formula**

**Variables**

**Meaning**

**Example**

**Limitations**

**Source**

If metaphorical rather than mathematically rigorous, label it as such.

Never invent formulas.

---

# PHASE 20 — Example Library

Build a searchable example database:

| Situation | Example | Principle demonstrated | Outcome | Source |
|---|---|---|---|---|

Separate:

- anecdote
- case study
- controlled evidence
- company claim
- marketing claim
- independently verified evidence

---

# PHASE 21 — Claim Audit

Classify important claims:

🟢 Strongly supported  
🟡 Plausible / mixed evidence  
🔴 Weakly supported / disputed  
⚪ Opinion / heuristic / personal experience  

For scientific or empirical claims distinguish:

- expert's claim
- underlying evidence
- broader consensus
- uncertainty

Do not treat authority as evidence.

---

# PHASE 22 — Criticism and counterarguments

Find serious critiques.

Prefer:

- primary research
- domain experts
- credible practitioners
- documented failures
- competing schools of thought

For each:

**Expert's claim**

**Criticism**

**Evidence supporting expert**

**Evidence challenging expert**

**Current state of evidence**

Do not manufacture false balance.

---

# PHASE 23 — Cheat Sheets

Create concise reference sheets for:

- Principles
- Frameworks
- Decision rules
- Processes
- Metrics
- Mistakes
- Questions
- Recommended actions
- Warnings
- Contradictions
- Important examples

These are retrieval aids, not substitutes for the source-grounded database.

---

# PHASE 24 — Accessibility layer

Assume the reader is intelligent but not already expert.

For complex ideas provide:

**ELI5**

**Normal explanation**

**Expert explanation**

Define jargon immediately.

Avoid needless complexity.

---

# PHASE 25 — Machine-readable knowledge base

Export a structured schema.

Minimum recommended shape:

```json
{
  "expert": "",
  "domain": "",
  "sources": [],
  "principles": [],
  "mental_models": [],
  "frameworks": [],
  "processes": [],
  "decision_rules": [],
  "metrics": [],
  "claims": [],
  "contradictions": [],
  "examples": [],
  "criticisms": [],
  "situations": [],
  "lens": {}
}
```

Recommended object fields:

```json
{
  "id": "",
  "type": "",
  "title": "",
  "summary": "",
  "source_ids": [],
  "date_first_seen": "",
  "date_last_seen": "",
  "attribution_confidence": "",
  "evidence_status": "",
  "direct_or_inferred": "",
  "related_ids": []
}
```

Design richer schemas when useful.

The knowledge base should be reusable by:

- an AI agent
- RAG system
- chatbot
- database
- app
- personal knowledge system
- multi-expert council

---

# Final deliverables

Produce:

1. Executive Overview
2. Source Ledger
3. Complete Knowledge Map
4. Core Principles
5. Mental Model Library
6. Framework Library
7. Decision Rulebook
8. Process & Playbook Library
9. Metrics Dashboard
10. Contradiction Map
11. Evolution Timeline
12. 80/20 Guide
13. Overlooked Ideas
14. Beginner → Expert Curriculum
15. Situation → Advice Database
16. Expert Simulator / Callable Lens
17. Knowledge Graph
18. Formula Library
19. Example Library
20. Evidence Audit
21. Criticism & Counterarguments
22. Cheat Sheets
23. Machine-readable Knowledge Base

---

# Research rules

## Non-negotiable

Do not hallucinate completeness.

Do not attribute something to the expert without evidence.

Do not convert the model's own knowledge into the expert's opinion.

Distinguish:

> DIRECT POSITION

from:

> PARAPHRASE

from:

> SYNTHESIS

from:

> INFERENCE

If a claim cannot be verified, mark:

**UNVERIFIED**

If sources disagree, preserve disagreement.

Attach sources wherever possible.

Include dates because views evolve.

Prefer primary sources.

Do not repeat the same idea merely because it appeared many times.

Record frequency instead.

Do not make the expert sound smarter, more coherent, or more consistent than the source material supports.

The job is to reconstruct what they actually teach, believe, recommend, measure, revise, and contradict.

---

# Execution rules

Do not cram the entire project into one response when the corpus is large.

First estimate corpus size.

Then propose batches such as:

- Batch 1 — source discovery
- Batch 2 — transcript/content ingestion
- Batch 3 — atomic extraction
- Batch 4 — deduplication
- Batch 5 — taxonomy
- Batch 6 — frameworks
- Batch 7 — rules/processes
- Batch 8 — contradictions/evolution
- Batch 9 — evidence/criticism
- Batch 10 — final synthesis
- Batch 11 — callable lens packaging

Maintain a persistent master knowledge base between batches when the environment supports it.

At the end of each batch report:

**Processed**  
**Remaining**  
**New concepts discovered**  
**Sources covered**  
**Unresolved questions**  
**Next batch**

---

# Fast mode

If the user wants a lighter version, use:

```text
Create a Fast Expert OS for [EXPERT].
```

Fast mode should still:

- use primary sources
- identify core beliefs
- extract major frameworks
- identify contradictions
- create a callable lens

But it may omit exhaustive atomic extraction.

Never call Fast mode exhaustive.

---

# Deep mode

Trigger examples:

- `Deep Expert OS for [EXPERT]`
- `Do the full corpus`
- `Build the complete operating system`

Deep mode requires:

- corpus batching
- source ledger
- atomic knowledge objects
- deduplication
- chronology
- contradiction tracking
- evidence audit
- machine-readable export

---

# Skill packaging

When the user asks to convert the final Expert OS into a reusable skill, create a skill with:

```text
name
description
triggers
purpose
source-grounding rules
core principles
question set
decision logic
failure modes
blind spots
invocation behavior
```

The resulting expert skill should be composable with other expert skills.

Example:

```text
Call HEM
```

may combine separate Expert OS lenses for Hormozi, Rory Sutherland, and Elon Musk without flattening their differences.

---

# Example

User:

`Create Expert OS for Rory Sutherland.`

Expected process:

1. discover primary corpus
2. retrieve talks/interviews/books/articles
3. use Agent Reach if YouTube/Instagram retrieval is incomplete
4. extract atomic ideas
5. deduplicate
6. identify recurring models such as:
   - psychological value
   - reframing
   - signaling
   - uncertainty reduction
   - anti-efficiency traps
   - explore vs exploit
7. find contradictions and limits
8. evidence-audit behavioral claims
9. create situation → advice mappings
10. package as a callable `Rory` lens

Later:

`Rory. Look at this idea.`

The agent should then re-read the current conversation through that source-grounded lens.


---

# GitHub-ready usage and positioning

## One-line positioning

Turn hundreds of hours of an expert's public content into a source-grounded, reusable decision engine.

## Why this exists

Most prompts that ask an AI to "study everything this person has ever said" produce a plausible summary, not a reliable reconstruction of a large public corpus.

Expert OS treats the task as a research pipeline:

```text
discover
→ retrieve
→ extract
→ deduplicate
→ structure
→ challenge
→ version
→ package into a reusable reasoning lens
```

The goal is not to create a biography, fan summary, quote collection, or roleplay persona.

The goal is to reconstruct the system underneath the expert's thinking.

## Architecture

```text
Expert Name
   ↓
Corpus Discovery
   ↓
YouTube / Podcasts / Books / Interviews / Articles / Social
   ↓
Source Ledger
   ↓
Atomic Knowledge Extraction
   ↓
Deduplication
   ↓
Knowledge Taxonomy
   ↓
Mental Models / Frameworks / Decision Rules / Processes / Metrics
   ↓
Contradiction Detection
   ↓
Evolution Timeline
   ↓
Evidence Audit
   ↓
Situation → Advice Database
   ↓
Callable Expert Lens
```

## Recommended modes

### Fast Expert OS

Use when speed matters more than exhaustive coverage.

Must still include:

- core beliefs
- major frameworks
- primary sources
- contradictions
- callable lens

Never call Fast mode exhaustive.

### Deep Expert OS

Use for a full research build.

Requires:

- corpus batching
- source ledger
- transcript/content ingestion
- atomic extraction
- deduplication
- chronology
- contradiction tracking
- evidence audit
- criticism
- knowledge graph
- machine-readable export
- callable lens packaging

## Example usage

```text
Create Expert OS for Alex Hormozi.
```

```text
Deep Expert OS for Rory Sutherland.
Process his talks, interviews, books, articles, and long-form content.
Preserve contradictions and changes over time.
```

```text
Reverse engineer Andrew Huberman's public body of work into a reusable operating system.
```

After the OS is built:

```text
Hormozi. Stress-test this offer.
```

```text
Rory. Look at this product idea.
```

```text
Musk. Tear apart this architecture.
```

The system should re-read the current problem through the reconstructed source-grounded lens.

It must never imply the real person personally reviewed the situation.

## Multi-expert composition

Expert OS lenses should remain composable.

Example:

```text
Hormozi
+
Rory Sutherland
+
Elon Musk
=
HEM
```

Do not average multiple lenses into one generic answer.

Preserve disagreement.

The tension between operating systems is often the most useful output.

## Limitations

Expert OS cannot guarantee completeness unless the relevant corpus has actually been retrieved and processed.

Common limitations:

- unavailable transcripts
- paywalled books
- private material
- deleted posts
- platform restrictions
- incomplete Instagram access
- inaccessible archives
- ambiguous attribution
- experts changing their minds

A polished answer is not evidence of complete research.

Always state what was actually processed.

## Accuracy rules

Never:

- fabricate quotes
- invent sources
- claim exhaustive coverage without evidence
- flatten contradictions
- turn synthesis into direct attribution
- confuse anecdotes with empirical evidence
- assume the expert is correct
- imitate the person as if they are literally present

Always:

- prefer primary sources
- include dates when relevant
- preserve disagreements
- label inference
- challenge unsupported claims
- surface blind spots
- show uncertainty

## Recommended repo structure

```text
expert-os/
├── README.md
├── SKILL.md
├── LICENSE
├── examples/
│   ├── hormozi.md
│   ├── rory-sutherland.md
│   └── musk.md
├── schemas/
│   └── expert-os.schema.json
└── docs/
    ├── methodology.md
    ├── ingestion.md
    └── evidence.md
```

Only `SKILL.md` is required to run the skill.

## Future extensions

Potential extensions include:

- automatic transcript ingestion
- local vector database
- automated source deduplication
- contradiction detection
- claim-confidence scoring
- timeline visualization
- knowledge graph export
- citation explorer
- multi-expert comparison
- automatic Expert OS → skill generation
- council builder
- Obsidian export
- Notion export
- JSONL export
- web UI
- Agent Reach integration helpers

## Final principle

> Do not summarize the expert. Reconstruct the system underneath their thinking.

The desired end state is not:

```text
"Here are 50 lessons from this person."
```

It is:

```text
"I can query the operating system behind hundreds of hours of their public work."
```
