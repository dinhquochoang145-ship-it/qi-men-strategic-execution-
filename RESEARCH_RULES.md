# Research Rules

## Scope

This repository builds a source-grounded Knowledge Base for:

Qi Men Strategic Execution

The Knowledge Base must represent Joey Yap / Mastery Academy teachings only unless a section is explicitly labeled as project interpretation.

## Source Boundary

Acceptable primary sources:

1. Books authored by Joey Yap
2. Mastery Academy course notes
3. Mastery Academy workbooks
4. Official Joey Yap websites
5. Official Mastery Academy websites
6. Videos where Joey Yap directly teaches
7. Webinars or seminars where Joey Yap directly teaches
8. Podcasts or interviews where Joey Yap directly explains Qi Men
9. Official previews or samples of Joey Yap books/courses

Third-party sources may be used only to discover primary sources.

Never use a third-party interpretation as a Joey Yap SOURCE FACT.

## Research Priority

Accuracy > completeness.

If evidence is incomplete, preserve the gap.

Never fill missing knowledge with:

- general Qi Men knowledge
- another Qi Men school
- model memory
- assumptions
- inferred formation meanings

## Verification

Before extracting knowledge from a source:

1. Confirm source identity.
2. Confirm author/speaker.
3. Confirm relationship to Joey Yap / Mastery Academy.
4. Record the source in SOURCE_INDEX.md.
5. Assign verification status.
6. Add it to SOURCE_QUEUE.md if further work is required.

## Extraction

Knowledge must first be stored as atomic claims in:

`/extracted/`

Follow KNOWLEDGE_SCHEMA.md.

Do not write extracted facts directly into normalized KB files.

## Source Fact vs Interpretation

Always preserve three layers:

### SOURCE FACT

Directly supported by a Joey Yap / Mastery Academy source.

### PRACTICAL INTERPRETATION

Derived reasoning from verified source facts.

Must reference supporting Claim IDs.

### PROJECT RULE

A rule specifically designed for Qi Men Strategic Execution.

Must reference supporting Claim IDs.

A project rule is not automatically a Joey Yap rule.

## Contradictions

If two primary sources appear inconsistent:

- preserve both claims
- cite both
- do not silently reconcile them
- record the issue for later QA

## Missing Evidence

Use:

`UNVERIFIED — chưa đủ căn cứ xác nhận đây là kiến thức Joey Yap.`

or:

`Không có căn cứ rõ trong nguồn Joey Yap hiện thu thập được.`

Never manufacture a complete answer.

## Trading Boundary

Qi Men may support:

- strategic context
- timing
- direction
- execution
- psychology
- decision support
- risk awareness

Qi Men must not be converted into:

- price prediction
- Buy/Sell signals
- guaranteed profit
- removal of stop loss
- increased risk solely because of a Qi Men reading

Trading applications must clearly separate:

1. Joey Yap SOURCE FACT
2. project interpretation
3. existing trading-system decision

## Research Completion

A research task is not complete merely because the agent reports completion.

Completion requires repository artifacts that can be independently inspected.

When applicable, update:

- SOURCE_INDEX.md
- SOURCE_QUEUE.md
- RESEARCH_STATUS.md
- extracted files
- QA reports

## Stop Rule

If the required primary evidence cannot be accessed or verified:

STOP.

Record the gap or blocked source.

Do not compensate by searching for teachings from another Qi Men school.
