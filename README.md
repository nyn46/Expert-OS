# Expert OS

Turn any public expert's body of work into a source-grounded operating system you can invoke later as a reusable reasoning lens.

## Trigger examples

```text
Create Expert OS for Alex Hormozi
Build Expert OS for Rory Sutherland
Reverse engineer Andrew Huberman
Deep Expert OS for Seth Godin
```

## What it does

Expert OS:

1. Builds a primary-source corpus
2. Extracts atomic claims
3. Deduplicates repeated ideas
4. Builds a taxonomy
5. Reconstructs core beliefs, frameworks, rules, processes, and metrics
6. Finds contradictions and changes over time
7. Audits evidence and criticism
8. Creates situation → advice mappings
9. Packages the result as a reusable callable lens

## Agent Reach fallback

If ordinary web access cannot adequately retrieve YouTube or Instagram material, the skill can use [Agent Reach](https://github.com/Panniantong/agent-reach) as an ingestion pattern.

- YouTube → `yt-dlp`
- Instagram → `OpenCLI` with an existing browser session, or official API routes where applicable

Retrieval is not the same as synthesis. The skill still requires source attribution, deduplication, chronology, contradiction tracking, and evidence review.

## Output

The full workflow can produce:

- source ledger
- knowledge map
- mental model library
- framework library
- decision rulebook
- contradiction map
- evolution timeline
- evidence audit
- machine-readable knowledge base
- callable expert lens

See [`SKILL.md`](./SKILL.md) for the complete workflow.
