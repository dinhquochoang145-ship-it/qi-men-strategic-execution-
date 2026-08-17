# Normalization Plan Review

Review date: 2026-08-17

Scope: `NORMALIZATION_PLAN.md` checked against the current 337-claim extracted corpus and extraction QA reports.

This review does not normalize, merge, delete, or derive project rules.

## Corpus Check

| Check | Result |
|---|---|
| Extracted atomic claims | 337 |
| Extracted source files with claims | 34 |
| Reviewed zero-claim sources | 13 |
| Blocked access sources | 5 |
| Confidence A claims | 260 |
| Confidence B claims | 77 |
| Confidence C claims | 0 |
| Extraction phase status | Complete for currently accessible corpus |

## Taxonomy Review

The proposed taxonomy is supported by the corpus. Support is uneven:

- Strongly supported: Foundations, Forecasting, Strategic Execution, Destiny, Manifesting, Chart Components, Question Framing, Decision Making, Business / Career, Wealth.
- Supported but context-sensitive: Timing, Direction, Doors, Deities.
- Supported but thin or case-heavy: Stars, Stems, Formations, Property, Health, Relationships, Cases / Examples.

No unsupported empty bucket is recommended for immediate normalized output.

## Risky Merge Patterns

### Forecasting vs Manifesting

Risk: claims about forecasting likely outcomes, day/hour chart usage, manifesting, intention, alignment, commands, and action can be flattened into a single "Qi Men gets results" unit.

Required control: keep forecasting and manifesting in separate units unless the source explicitly contrasts them in the same statement.

### Forecasting vs Destiny

Risk: Guardian of Destiny, Destiny Chart, day deity, Destiny Palace, and intuition claims can be merged with forecasting chart claims because they share deities, palaces, or chart terminology.

Required control: preserve whether the source is talking about personal/internal Qi Men, Destiny Chart, or a forecasting chart.

### General Rules vs Cases

Risk: Ask Joey Yap and webinar examples include specific readings involving Life Door, Open Door, Rest Door, Harm Door, Chief, D/E or void, Green Escape, Flying Bird Fall Into Cave, business outcomes, property, surgery, fertility, doctors, and partnerships.

Required control: keep these as `Case-Specific? yes` unless Joey Yap separately states a general principle.

### Component Name Similarity

Risk: terms like Life Door, Rest Door, Open Door, Chief, Black Tortoise, Nine Earth, Nine Heavens, Heavenly Heart, Hero Star, hour stem, D/E, and formations may recur in different contexts with different function.

Required control: merge only when underlying teaching and context match. Do not merge by term alone.

### Four Realms Variants

Risk: the corpus includes several four-realm/four-component statements across manifesting, chart structure, and wealth/business model contexts. Automatic captions also preserve imperfect variants such as "universe, man, Earth, and spirit."

Required control: preserve terminology variants and source context. Do not force all four-realm claims into one canonical unit unless the wording and scope are compatible.

### Wealth, Business, Investment, And Trading Boundary

Risk: business and wealth claims may be misread as profit guarantees, investment advice, trading signals, or market predictions.

Required control: every wealth/business/investment-adjacent normalized unit must include an explicit Do Not Infer boundary against trading signals, investment advice, price prediction, and guaranteed profit.

### Health Boundary

Risk: health-block, healing, doctor, surgery, fertility, chronic pain, and illness-sector claims can be misread as medical guidance.

Required control: health units must stay source-framed and case-specific where applicable; they must explicitly reject medical advice, diagnosis, treatment, or guaranteed healing.

### Caption Quality

Risk: media and webinar claims rely on YouTube automatic captions. Batch reports flagged noisy renderings such as "achievement," "treatment," "chiman," "shimon," "Chan," "D E," "Grain," and other imperfect terms.

Required control: do not normalize ambiguous caption terms into technical vocabulary unless surrounding source context supports the term. Use lower confidence or a terminology note where needed.

### Software And Product Context

Risk: WEB-008 and VIDEO-004 include software walkthrough or product/support context. Software features may be mistaken for general Qi Men doctrine.

Required control: keep software/product claims in chart-component or source-context units and avoid turning UI behavior into technical rules.

### Promotional Or Marketing Language

Risk: extraction reports repeatedly rejected service copy, enrollment promises, CTAs, broad promotional claims, and resource-list titles.

Required control: normalization must not reintroduce rejected marketing language as SOURCE FACT.

## Plan Compliance Review

| Requirement | Review Result |
|---|---|
| Canonical unit schema includes required fields | Pass |
| Stable normalized ID format defined | Pass |
| Taxonomy based on extracted corpus | Pass |
| Merge rules defined | Pass |
| Non-merge rules defined | Pass |
| Contradiction handling defined | Pass |
| Case handling defined | Pass |
| Confidence model defined | Pass |
| Provenance rule defined | Pass |
| Safety boundary defined | Pass |
| Output architecture under `normalized/` proposed | Pass |
| Normalization order defined | Pass |
| QA gate defined | Pass |

## Batch 001 Recommendation

Begin normalization batch 001 only after explicit plan approval.

Recommended first batch:

- Foundations
- Forecasting boundaries
- Decision-making boundaries
- Question-framing principles

Reason: these topics define the boundaries that prevent later component, business, wealth, health, and case-specific normalization from overreaching.

## Open QA Notes

- Stems, Stars, Formations, Property, Health, and Relationships should not be normalized as broad doctrinal systems from the current corpus.
- Case-heavy claims should be routed to `normalized/cases_examples.md` first or clearly marked as case-specific in their topic files.
- Any unit supported only by B-confidence automatic-caption claims should remain B or C unless supported by a cleaner article/video claim.
- No extracted claim files should be touched during normalization.
