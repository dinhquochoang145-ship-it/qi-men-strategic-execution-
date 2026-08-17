# Normalization Plan

Current phase: NORMALIZATION PREPARATION

Corpus: 337 extracted atomic claims from verified accessible official Joey Yap / Mastery Academy web, video, and webinar sources.

This plan defines how to create a normalization layer. It does not normalize claims, merge source claims, delete source claims, reconcile contradictions, or derive project rules.

## Purpose

Normalization will organize overlapping Joey Yap Qi Men teachings into stable canonical knowledge units while preserving every original atomic claim and its source traceability.

The normalized layer must remain a SOURCE FACT layer. Practical interpretations and project rules come later and must not be added during normalization.

## Canonical Knowledge Unit Schema

Each normalized unit must use this schema:

| Field | Requirement |
|---|---|
| Normalized ID | Stable ID using the approved format. |
| Canonical Topic | Short normalized topic label. |
| Canonical Statement | A conservative statement supported by the listed atomic claims. It must not be stronger than the source wording. |
| Supporting Claim IDs | Every atomic claim that supports the unit. |
| Supporting Source IDs | Source IDs represented by the supporting claims. |
| Source Contexts | Source-level contexts preserved from atomic claims, including article, video, webinar, Q&A, software, course/news report, case, or demonstration context. |
| Conditions / Scope | Explicit limits, dependencies, and contexts from the supporting claims. |
| Case-Specific? yes/no | `yes` if the unit depends on an Ask Joey Yap/webinar case, named example, demonstrated chart, or individual scenario; otherwise `no`. |
| Terminology Variants | Source terms and caption variants preserved without silently normalizing meaning. |
| Confidence | Normalized confidence derived from the confidence model below. |
| Contradictions / Tensions | Apparent contradictions, context-dependent differences, unresolved tensions, and reason for not resolving them. |
| Do Not Infer | Combined safety and scope boundary. Must include every important limitation needed to prevent overreach. |
| Notes | Optional handling notes, source-quality notes, or future QA flags. |

## Normalized ID Format

Use:

`NORM-[TOPIC]-[NUMBER]`

Rules:

- `[TOPIC]` is an uppercase stable slug, not a prose title.
- `[NUMBER]` is three digits, assigned sequentially within the topic slug.
- Do not reuse IDs after a unit is accepted.
- If a unit is split later during QA, retire the old unit in the normalized index and assign new IDs rather than silently changing its meaning.

Examples:

- `NORM-FOUNDATIONS-001`
- `NORM-FORECASTING-001`
- `NORM-QUESTION-FRAMING-001`
- `NORM-DEITIES-001`
- `NORM-CASE-BUSINESS-001`

## Topic Taxonomy

The taxonomy below is based on the extracted corpus. Buckets should only be created when at least one supporting claim exists.

| Topic Bucket | Supported? | Corpus Basis | Notes |
|---|---|---|---|
| Foundations | yes | Definitions, historical use, Chinese metaphysics classification, time/space, oracle methods, modern use boundaries. | Good first batch candidate. |
| Forecasting | yes | Forecasting purpose, likely outcome, hour chart, yes/no questions, trajectory, current-status readings, answer/user box relationships. | Must separate general methods from cases. |
| Strategic Execution | yes | Right timing, right action, planning, changing strategy/focus, execution after forecast. | Do not convert into project rules yet. |
| Destiny | yes | Qi Men Destiny, Destiny Chart, Guardian of Destiny, Destiny Palace, personal Qi Men, intuition. | Keep separate from forecasting chart use. |
| Manifesting | yes | Intent, alignment, commands, conquer, four realms, deities/commands, awakened/slumbering mind, energy blocks. | High-risk for overstatement and guarantees. |
| Chart Components | yes | Palaces/boxes, elements, five elements, center exclusion, chart fields, software chart components, palace energy. | Parent bucket for Doors/Stars/Deities/Stems/Formations where useful. |
| Doors | yes | Life Door, Rest Door, Open Door, Harm Door, Door of Destiny. | Many uses are case-specific; do not merge all Life Door claims. |
| Stars | yes | Nine Stars, Star of Destiny, Hero Star, Heavenly Heart. | Thin and sometimes case-specific. |
| Deities | yes | Guardian Deity, Guardian of Destiny, Black Tortoise, Chief, Nine Earth, Nine Heavens, day deity, command deities. | Must preserve Destiny vs forecasting vs manifesting context. |
| Stems | yes, limited | Ten Stems, hour stem, answer/user stem context, D/E/void cases. | Limited corpus; many claims are method/case-specific. |
| Formations | yes, limited | Flying Bird Fall Into Cave, Green Escape, Three Victory Palace. | Mostly case-specific; no broad formation catalog. |
| Timing | yes | Strategic timing, hour/day chart distinction, timed actions, directions/times, current chart timing, timing application. | Do not infer date-selection rules beyond sources. |
| Direction | yes | Eight directions/perspectives, strategic directions, planner directions, facing a direction, property/directional examples. | Must preserve source context and avoid universal direction meanings. |
| Business / Career | yes | Business timing, launches, consulting, sales, career/job choices, partnerships, business models, branding. | Case-heavy and safety-sensitive. |
| Wealth | yes | Wealth spectrum, wealth command, investments, profit/service, wealth palace, opportunities, business wealth blueprint. | Do not convert into investment/trading advice. |
| Property | yes, limited | Qi Men Feng Shui, property opportunity, Open Door, remote viewing/property, house examples. | Mostly examples/cases. |
| Health | yes, limited | Healing support, Rest Door, Nine Earth, health blocks, illness examples, surgery/doctor cases. | Must retain medical safety boundary. |
| Relationships | yes, limited | Relationship decisions, superior/work relationship, partnership harmony/problem cases, love/relationships in manifesting. | Limited and case-specific. |
| Question Framing | yes | Asking the right question, question structure, yes/no framing, poor questions, reformulating/waiting, intention before answer. | Good early normalization topic. |
| Decision Making | yes | Qi Men as decision support, does not decide for user, decision outcome forecasting, strategic choices. | May overlap with Forecasting and Strategic Execution; keep boundaries clear. |
| Cases / Examples | yes | Ask Joey Yap readings, webinar demonstrations, named cases, chart demonstrations, health/property/business examples. | Should be a separate case layer or case topic files, not merged into general rules. |

No empty taxonomy bucket should be created during normalization. If later acquired books/courses add unsupported topics, add new topic files only after source-grounded extraction.

## Merge Rules

Two or more atomic claims may be normalized into one unit only when all of these are true:

1. They state the same underlying teaching.
2. Their scope is compatible.
3. Their conditions do not conflict.
4. Their terminology is equivalent or clearly related in the source context.
5. Their source contexts can be preserved in the normalized unit without flattening meaning.
6. The combined canonical statement can be written without adding new interpretation.
7. Every supporting claim remains cited by Claim ID and Source ID.
8. The resulting Do Not Infer field preserves all important limitations from the source claims.

Examples of acceptable merge candidates:

- Multiple general claims that Qi Men supports decision-making or forecasting likely outcomes, if each is not tied to incompatible methods or specific cases.
- Multiple general claims that Qi Men is connected to time, space, and strategic timing, if no source adds a narrower operational condition.
- Multiple general claims about question framing, if they share the same framing principle and do not differ by yes/no, manifesting, or case context.

## Non-Merge Rules

Do not merge claims when any of these are true:

1. One claim is case-specific and another is general.
2. Meanings differ by application context.
3. Forecasting and destiny uses differ.
4. Forecasting and manifesting uses differ.
5. Source claims conflict or appear to conflict.
6. Terminology similarity is superficial.
7. One source adds materially different conditions.
8. A caption term is ambiguous and another source uses a cleaner but not explicitly equivalent term.
9. A software feature claim and a teaching claim share terms but differ in function.
10. A business, wealth, health, relationship, property, or investment case would become a generalized rule.

Examples of prohibited merges:

- Black Tortoise in a forecasting/work relationship case with Black Tortoise in a Destiny context.
- Rest Door as home/healing in a specific property/doctor case with general health support claims.
- Life Door in business income/property cases with general Life Door meaning.
- D/E or void case timing with any general stem rule.
- Four realms in manifesting with a business-model four-realm explanation unless the source contexts and terminology explicitly align.
- Any investment or wealth case with trading or investment rules.

## Contradiction Handling

Normalization must never silently resolve contradictions.

If claims appear inconsistent, create separate normalized units or add a tension note. Mark the tension as one of:

- Apparent contradiction: source wording appears to disagree.
- Context-dependent difference: statements differ because one is forecasting, destiny, manifesting, software, article, or case context.
- Unresolved tension: evidence is insufficient to decide whether the difference is contextual or contradictory.

Required handling:

- Preserve both supported statements.
- Cite both sets of Claim IDs.
- Do not choose a winner.
- Do not harmonize using general Qi Men knowledge.
- Add a QA flag for later review.

## Case Handling

Ask Joey Yap, webinar Q&A, named demonstrations, chart examples, health examples, property examples, business examples, investment questions, and relationship/partnership cases must be handled as case-specific unless Joey Yap explicitly states a general principle.

Case units should:

- Use `Case-Specific? yes`.
- Include the case domain, such as business, health, property, career, relationship, or investment.
- Preserve the exact chart factor or condition named in the source.
- Include a Do Not Infer field that blocks generalizing the case.
- Avoid becoming a canonical rule for all charts.

Case units may support later general units only when the same general principle is independently stated outside the case or repeatedly stated across compatible case contexts.

## Confidence Model

Normalized confidence is derived from the supporting claims, not from whether the statement sounds plausible.

Use:

### A

High-confidence normalized SOURCE FACT.

Requirements:

- Supported by at least one direct Joey Yap source with confidence A, or multiple compatible B claims with clean context.
- Clear citation and context.
- No unresolved contradiction.
- Not dependent on noisy caption terminology.
- Not overgeneralized from a case.

### B

Moderate-confidence normalized SOURCE FACT.

Use when:

- The claim is supported by direct Joey Yap sources, but captions are imperfect, source context is broad, page context is high-level, or the statement is narrow/case-specific.
- The unit is supported by one clear B claim.
- The unit combines multiple claims with compatible but not identical wording.

### C

Restricted normalized unit.

Use when:

- The source material is direct but the normalized wording depends on limited, noisy, or ambiguous caption context.
- A tension is unresolved.
- A source is case-specific and later users may be tempted to generalize it.

C-level units must not be used for authoritative project rules without later QA and stronger support.

Confidence modifiers:

- Increase confidence when independent source types support the same teaching, such as article plus video plus webinar.
- Increase confidence when the teaching is direct, general, and repeated.
- Decrease confidence for automatic-caption ambiguity.
- Decrease confidence for broad marketing/article language.
- Decrease confidence when a claim is case-specific.
- Decrease confidence when a unit rests on one source only.

## Provenance Rule

Every normalized statement must remain traceable back to original atomic Claim IDs and Source IDs.

Required:

- Never cite only a normalized unit as evidence for source fact.
- Include all supporting Claim IDs in every normalized unit.
- Include all supporting Source IDs in every normalized unit.
- Preserve source contexts and citations in the normalized unit or link to an index that contains them.
- Do not delete, rename, or rewrite files in `extracted/`.

## Safety Boundary

Normalization must not create:

- Trading signals.
- Price predictions.
- Guaranteed outcomes.
- Medical advice.
- Investment advice.
- Legal advice.
- Relationship determinism.
- Claims stronger than source wording.
- Complete methods from partial source statements.
- Technical meanings for terms not defined in the source.

Safety-sensitive normalized units must explicitly state:

- Qi Men does not replace ordinary due diligence, risk management, medical care, legal advice, or investment analysis.
- Case examples do not become universal chart rules.
- Forecasting is not deterministic prediction.
- Manifesting language does not guarantee outcomes.

## Output Architecture

Create both a master index and topic files under `normalized/`.

Recommended files:

- `normalized/INDEX.md`
- `normalized/foundations.md`
- `normalized/forecasting.md`
- `normalized/strategic_execution.md`
- `normalized/destiny.md`
- `normalized/manifesting.md`
- `normalized/chart_components.md`
- `normalized/doors.md`
- `normalized/stars.md`
- `normalized/deities.md`
- `normalized/stems.md`
- `normalized/formations.md`
- `normalized/timing_direction.md`
- `normalized/business_career_wealth.md`
- `normalized/property_health_relationships.md`
- `normalized/question_framing_decision_making.md`
- `normalized/cases_examples.md`
- `normalized/CONTRADICTIONS_AND_TENSIONS.md`

Use `normalized/INDEX.md` as the routing and coverage file:

- List every normalized unit ID.
- Link each unit to its topic file.
- Track supporting source IDs.
- Track whether it is case-specific.
- Track normalized confidence.
- Track QA status.

Topic files should contain the full canonical unit records.

## Normalization Order

Normalize in this order:

1. Foundations: establishes definitions, boundaries, historical use, and non-prediction limits before other units rely on them.
2. Forecasting and Decision Making: central to the corpus and needed to separate outcome forecasting from deterministic prediction.
3. Question Framing: heavily supported and controls how later forecasting/case claims should be interpreted.
4. Strategic Execution, Timing, and Direction: closely related to the project mission but must remain SOURCE FACT rather than PROJECT RULE.
5. Destiny: distinct from forecasting and necessary before deities/Guardian claims are normalized.
6. Manifesting: substantial support but high risk for guarantee language and source-context overreach.
7. Chart Components, Doors, Stars, Deities, Stems, and Formations: normalize only after general context is established; many component claims are case-specific or caption-sensitive.
8. Business / Career and Wealth: normalize after safety boundaries are in place because claims can be mistaken for investment, trading, or guaranteed-outcome rules.
9. Property, Health, and Relationships: normalize later because most support is case-heavy and safety-sensitive.
10. Cases / Examples: create case units last, after general topics exist, so cases can be referenced without becoming general rules.

## QA Gate

Each normalization batch must pass a QA gate before acceptance.

Required checks:

1. Every normalized unit has all required schema fields.
2. Every Supporting Claim ID exists in `extracted/*.md`.
3. Every Supporting Source ID matches the Claim ID prefix.
4. The Canonical Statement is not stronger than any supporting claim.
5. Case-specific claims are not merged into general units.
6. Forecasting, destiny, manifesting, and software contexts remain distinct.
7. Caption ambiguity is captured in Notes or Confidence.
8. Every safety-sensitive unit has an explicit Do Not Infer boundary.
9. Contradictions and tensions are recorded instead of resolved.
10. No extracted claim file is modified.
11. No project rules or practical interpretations are created.
12. Batch report records accepted units, rejected merge candidates, open tensions, and source coverage.

Each batch should create:

- The relevant `normalized/*.md` topic file or update it.
- An update to `normalized/INDEX.md`.
- A QA report under `qa/`, for example `qa/NORMALIZATION_BATCH_001_REVIEW.md`.

## Plan Approval Gate

Do not begin normalization until this plan is approved in a separate user instruction.
