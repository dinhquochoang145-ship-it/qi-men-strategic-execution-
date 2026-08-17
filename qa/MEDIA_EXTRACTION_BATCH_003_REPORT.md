# Media Extraction Batch 003 Report

## Scope

Atomic claim extraction batch completed on 2026-08-17 during the ATOMIC CLAIM EXTRACTION phase.

Allowed sources reviewed:

- VIDEO-011: QiMen Mini Topic 4: How Come Others Can Manifest And I Can't? Here's Why.
- VIDEO-012: QiMen Mini Topic 5: The QiMen Wealth Spectrum
- VIDEO-013: QiMen Mini Topic 6: The 4 Wealth Strategies Using QiMen
- VIDEO-014: QiMen Mini Topic 7: How to Become Phenomenal
- VIDEO-015: How QiMen Can Help You Forecast The Outcome

Excluded sources:

- Books
- Courses
- Web articles
- Webinars
- Podcasts
- Third-party uploads
- Any media source outside VIDEO-011 through VIDEO-015

No normalization, deduplication, project-rule derivation, or cross-source merging was performed.

## Source Access And Timestamp Review

| Source ID | Canonical URL | Official Provenance | Speaker | Access Result | Transcript / Caption Availability | Timestamp Quality | Claims Extracted | Blocker |
|---|---|---|---|---|---|---|---:|---|
| VIDEO-011 | https://www.youtube.com/watch?v=PMrpww0hglE | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 8 | None |
| VIDEO-012 | https://www.youtube.com/watch?v=TLCyz5HUZLg | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 8 | None |
| VIDEO-013 | https://www.youtube.com/watch?v=PvSHJrND-fs | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 13 | None |
| VIDEO-014 | https://www.youtube.com/watch?v=Kzly69DPT2Q | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 16 | None |
| VIDEO-015 | https://www.youtube.com/watch?v=Y1KZeGCcng4 | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 9 | None |
| TOTAL |  |  |  |  |  |  | 54 |  |

## Claims Extracted Per Source

| Source ID | Claims Extracted | Output File |
|---|---:|---|
| VIDEO-011 | 8 | extracted/VIDEO-011.md |
| VIDEO-012 | 8 | extracted/VIDEO-012.md |
| VIDEO-013 | 13 | extracted/VIDEO-013.md |
| VIDEO-014 | 16 | extracted/VIDEO-014.md |
| VIDEO-015 | 9 | extracted/VIDEO-015.md |
| TOTAL | 54 |  |

## Zero-Claim Sources

None. All five videos had accessible timestamped captions and contained extractable Qi Men teaching, explanation, boundary, application principle, or source-relevant factual instruction.

## Duplicate Candidates

- VIDEO-011 overlaps with VIDEO-006 and VIDEO-010 on manifesting, slumbering mind, deities, and energy language. Batch 003 retained only energy-block and health/wealth block material that was not already extracted.
- VIDEO-012 overlaps with VIDEO-013 on wealth and money blocks. Claims were kept where VIDEO-012 specifically explains the wealth-spirituality spectrum and attachment.
- VIDEO-013 overlaps with VIDEO-009 and VIDEO-010 on manifesting framework and intention. Claims were kept where this source adds the four wealth strategies, Wealth Palace, command detail, and wealth-specific strategy context.
- VIDEO-014 overlaps with VIDEO-008 through VIDEO-010 on intuition, consciousness, and levels of mind. Claims were kept where this source adds the "becoming phenomenal" path, guide limitation, four-level evolution, and letting-go sequence.
- VIDEO-015 overlaps with VIDEO-001, VIDEO-002, and VIDEO-004 on forecasting. Claims were kept where this source adds the application-model classification, Academy-specific classification note, and decision-context list.

## Case-Specific Claims

- VIDEO-011 and VIDEO-012 are framed as general teaching rather than individual chart readings.
- VIDEO-013 contains personal examples about a desired car and receiving wealth through channels such as investments, job, or deals; these were treated as examples, not project rules.
- VIDEO-014 uses Star Wars characters as analogies for consciousness stages; those analogies were not treated as technical Qi Men terms.
- VIDEO-015 uses a job-change example to explain forecasting question framing; the claim remains limited to that example context.

## Ambiguous Terminology

- YouTube automatic captions sometimes render Qi Men as similar-sounding English words such as "achievement," "treatment," or "Chan." Claims avoid relying on those rendered terms unless surrounding context clearly indicates Qi Men.
- VIDEO-013 captions render "Evidential Occurrences" inconsistently. The claim uses the known term only where the surrounding captioned explanation clearly supports it.
- VIDEO-014's "force" language is part of the Star Wars analogy and was not normalized into Qi Men terminology.
- VIDEO-015's "Chan" caption rendering was treated as a caption artifact in a Qi Men video; claims cite the source context and avoid using "Chan" as terminology.

## Rejected Promotional / Unsupported Statements

- QiMen Rally invitations, Telegram/Facebook/community prompts, training access details, and pricing/promotional copy were skipped.
- Jokes, casual banter, generic motivation, and unsupported anecdotes were skipped.
- Metadata, titles, thumbnails, and descriptions were not promoted into SOURCE FACT.
- Wealth and manifesting language was not converted into guarantees, investment advice, trading signals, or project rules.
- Medical or health references were preserved only as source claims with explicit Do Not Infer boundaries.

## Citation Limitations

- No official human-edited transcript was found or used.
- Citations use source ID, speaker, title, real caption timestamp range, and canonical YouTube URL.
- The downloaded caption files were used only as review aids and were not added to the repository.

## QA Confirmation

- Every extracted claim includes a Do Not Infer field.
- Every extracted claim cites one of VIDEO-011 through VIDEO-015.
- Every claim uses a real timestamp or timestamp range from the downloaded caption representation.
- No timestamps were estimated.
- No books, courses, web articles, webinars, podcasts, third-party uploads, or non-batch media sources were used.
- No claims were inferred from titles, descriptions, thumbnails, metadata, model memory, or third-party summaries.
- No claims were normalized or merged.
