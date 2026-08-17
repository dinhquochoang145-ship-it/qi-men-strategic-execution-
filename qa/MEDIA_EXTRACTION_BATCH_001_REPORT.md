# Media Extraction Batch 001 Report

## Scope

Atomic claim extraction batch completed on 2026-08-17 during the ATOMIC CLAIM EXTRACTION phase.

Allowed sources reviewed:

- VIDEO-001: What is Qi Men Dun Jia (QIMEN)?
- VIDEO-002: How to Read a Qi Men Dun Jia Forecasting Chart
- VIDEO-003: QiMen Strategy: Maximizing Your Wealth, Health & Career [Ask Joey Yap]
- VIDEO-004: The QiMen Explorer Basic Walkthrough
- VIDEO-005: How to Ask the Right Questions And Get What You Want

Excluded sources:

- Books
- Courses
- Web articles
- Webinars
- Podcasts
- Third-party uploads
- Any media source outside VIDEO-001 through VIDEO-005

No normalization, deduplication, project-rule derivation, or cross-source merging was performed.

## Source Access And Timestamp Review

| Source ID | Canonical URL | Official Provenance | Speaker | Access Result | Transcript / Caption Availability | Timestamp Quality | Claims Extracted | Blocker |
|---|---|---|---|---|---|---|---:|---|
| VIDEO-001 | https://www.youtube.com/watch?v=WRlNdOhnsy0 | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 13 | None |
| VIDEO-002 | https://www.youtube.com/watch?v=8hDp8lT2oto | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 7 | None |
| VIDEO-003 | https://www.youtube.com/watch?v=sJa2rHjC9CM | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 7 | None |
| VIDEO-004 | https://www.youtube.com/watch?v=kQB7rRJ_Vqo | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 14 | None |
| VIDEO-005 | https://www.youtube.com/watch?v=RZncklyM6Jc | Official Joey Yap YouTube channel (`UCYUxdK9N2GtTBVTTsBcRxAw`) | Joey Yap | Public and accessible by yt-dlp metadata check | English (Original) automatic captions downloaded as VTT and JSON3 | Real YouTube caption timestamps; no estimates | 7 | None |
| TOTAL |  |  |  |  |  |  | 48 |  |

## Claims Extracted Per Source

| Source ID | Claims Extracted | Output File |
|---|---:|---|
| VIDEO-001 | 13 | extracted/VIDEO-001.md |
| VIDEO-002 | 7 | extracted/VIDEO-002.md |
| VIDEO-003 | 7 | extracted/VIDEO-003.md |
| VIDEO-004 | 14 | extracted/VIDEO-004.md |
| VIDEO-005 | 7 | extracted/VIDEO-005.md |
| TOTAL | 48 |  |

## Zero-Claim Sources

None. All five videos had accessible timestamped captions and contained extractable Qi Men teaching, explanation, method, boundary, application principle, or source-relevant factual instruction.

## Claims Skipped For Insufficient Support

- Video titles, thumbnails, channel descriptions, metadata, and promotional subscription language were not converted into SOURCE FACT.
- Caption text with likely automatic-caption errors was not used when the intended terminology or context could not be established from surrounding captioned speech.
- Generic motivational advice and ordinary software account/login instructions were not extracted unless directly tied to Qi Men chart structure or source-relevant instruction.
- Case-reading conclusions were not generalized beyond the case unless Joey Yap stated the broader principle.

## Ambiguities

- The captions are YouTube automatic captions. They provide real timestamps but occasionally render Qi Men terms inconsistently, such as "human," "chiman," or similar variants. Claims preserve clear Joey Yap terminology only where the surrounding context supports it.
- VIDEO-003 and VIDEO-005 are live Q&A recordings. Several extracted claims are case-specific and should be treated cautiously during normalization.
- VIDEO-004 is a software walkthrough. Extracted claims were limited to chart components, training references, forecasting purpose, and directional/application statements; locked or paid software content was not accessed.

## Citation Limitations

- No official human-edited transcript was found or used.
- Citations use source ID, speaker, title, real caption timestamp range, and canonical YouTube URL.
- The downloaded caption files were used only as review aids and were not added to the repository.

## QA Confirmation

- Every extracted claim includes a Do Not Infer field.
- Every extracted claim cites one of VIDEO-001 through VIDEO-005.
- Every claim uses a real timestamp or timestamp range from the downloaded caption representation.
- No timestamps were estimated.
- No books, courses, web articles, webinars, podcasts, third-party uploads, or non-batch media sources were used.
- No claims were inferred from titles, descriptions, thumbnails, metadata, model memory, or third-party summaries.
- No claims were normalized or merged.
