# Knowledge Extraction Schema

## Purpose

Define the mandatory structure for every knowledge claim extracted from Joey Yap / Mastery Academy sources.

Do not extract knowledge directly into final KB files.

All knowledge must first exist as atomic claims.

---

## Atomic Claim Format

### Claim ID

Format:

`[SOURCE_ID]-C[NUMBER]`

Example:

`BOOK-001-C001`

Claim IDs must be unique and stable.

### Topic

The concept discussed by the source.

Examples:

- Life Door
- Nine Heaven
- Destiny Palace
- Day Chart
- Hour Chart
- Strategic Direction
- Formation

### SOURCE FACT

Record only what the source actually teaches.

Do not add general Qi Men knowledge.

Do not rewrite inference as fact.

### Exact Terminology

Record terminology used by Joey Yap / Mastery Academy when identifiable.

Include Chinese / English terminology when present in the source.

Do not invent translations.

### Context

State where the teaching applies, if the source specifies it.

Examples:

- Destiny Analysis
- Forecasting
- Strategic Execution
- Date Selection
- Business
- Investment
- General Qi Men

### Conditions

Record explicit conditions, limitations, exceptions, or dependencies stated by the source.

If none are stated:

`Not specified in this source.`

### Example

Record only examples actually provided by the source.

If none:

`No example provided in this source.`

### Citation

Include whenever available:

- Source ID
- Author / Speaker
- Title
- Chapter / Section
- Page
- Timestamp
- URL / Identifier

Never invent missing citation details.

### Confidence

#### A

Direct primary source with clear context and traceable citation.

#### B

Direct primary source, but context or citation precision is incomplete.

#### C

Evidence is incomplete or provenance is not sufficiently verified.

C-level claims must not be promoted into authoritative project rules.

### Do Not Infer

Explicitly record conclusions that this claim does NOT justify.

This field is mandatory.

---

## Knowledge Layers

Atomic extraction should primarily contain SOURCE FACT.

Later stages may create:

### PRACTICAL INTERPRETATION

A reasoned application derived from one or more verified SOURCE FACT claims.

Must cite the supporting Claim IDs.

### PROJECT RULE

A rule created specifically for Qi Men Strategic Execution.

Must cite the supporting Claim IDs and must never be presented as Joey Yap's own statement unless the source explicitly says so.

---

## Extraction Rules

1. One claim = one independently verifiable idea.
2. Do not combine several teachings into one claim merely because they appear on the same page.
3. Preserve important qualifications and conditions.
4. Do not resolve contradictions during extraction.
5. Do not fill gaps from model knowledge.
6. Do not normalize terminology during extraction if doing so changes the source wording.
7. If uncertain, preserve uncertainty.
8. Every claim must remain traceable back to its source.
