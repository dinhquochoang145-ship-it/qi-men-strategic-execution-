# Extraction Completeness Audit

Audit date: 2026-08-17

Scope: every indexed source in `SOURCE_INDEX.md`.

This audit checks whether ATOMIC CLAIM EXTRACTION is complete for the currently verified and accessible corpus. It does not extract new Qi Men claims, normalize claims, merge duplicates, reconcile contradictions, or derive project rules.

## Indexed Sources By Type

| Type | Count |
|---|---:|
| BOOK | 23 |
| COURSE | 18 |
| WEB | 18 |
| WEBINAR | 9 |
| VIDEO | 25 |
| PODCAST | 1 |
| INTERVIEW | 0 |
| TOTAL | 94 |

## Audit Classification Totals

| Classification | Count |
|---|---:|
| EXTRACTED | 34 |
| REVIEWED_ZERO_CLAIMS | 13 |
| BLOCKED_ACCESS | 5 |
| METADATA_ONLY | 37 |
| DISCOVERY_ONLY | 2 |
| UNRESOLVED | 3 |
| DUPLICATE_OR_MIRROR | 0 |
| TOTAL | 94 |

## Classification Assignments

### EXTRACTED

Accessible sources reviewed with atomic claims created.

- WEB-001
- WEB-002
- WEB-003
- WEB-004
- WEB-005
- WEB-006
- WEB-008
- WEB-016
- WEB-018
- WEBINAR-001
- WEBINAR-002
- VIDEO-001
- VIDEO-002
- VIDEO-003
- VIDEO-004
- VIDEO-005
- VIDEO-006
- VIDEO-007
- VIDEO-008
- VIDEO-009
- VIDEO-010
- VIDEO-011
- VIDEO-012
- VIDEO-013
- VIDEO-014
- VIDEO-015
- VIDEO-016
- VIDEO-018
- VIDEO-019
- VIDEO-020
- VIDEO-022
- VIDEO-023
- VIDEO-024
- VIDEO-025

### REVIEWED_ZERO_CLAIMS

Accessible sources reviewed, but no legitimate extractable Joey Yap Qi Men knowledge was extracted.

- WEB-009
- WEB-010
- WEB-011
- WEB-012
- WEB-013
- WEB-014
- WEB-015
- WEB-017
- WEBINAR-003
- WEBINAR-004
- WEBINAR-005
- WEBINAR-007
- VIDEO-021

### BLOCKED_ACCESS

Provenance is verified or sufficiently identified, but source content, transcript, or material is not reliably accessible for extraction.

- COURSE-006
- WEBINAR-006
- WEBINAR-008
- WEBINAR-009
- VIDEO-017

### METADATA_ONLY

Source identity is verified, but only metadata, product listing, course listing, or source-description material is available. These sources are not part of the extracted corpus until full content, official previews, samples, transcripts, manuals, workbooks, or authorized access are acquired.

- BOOK-001
- BOOK-002
- BOOK-003
- BOOK-004
- BOOK-005
- BOOK-006
- BOOK-007
- BOOK-008
- BOOK-009
- BOOK-010
- BOOK-011
- BOOK-012
- BOOK-013
- BOOK-014
- BOOK-015
- BOOK-016
- BOOK-017
- BOOK-018
- BOOK-019
- BOOK-020
- BOOK-021
- BOOK-022
- COURSE-001
- COURSE-002
- COURSE-003
- COURSE-004
- COURSE-005
- COURSE-007
- COURSE-008
- COURSE-009
- COURSE-010
- COURSE-011
- COURSE-012
- COURSE-013
- COURSE-014
- COURSE-015
- COURSE-016

### DISCOVERY_ONLY

Official discovery or index sources that are prohibited as final evidence for extracted Qi Men claims.

- WEB-007
- PODCAST-001

### UNRESOLVED

Provenance, source identity, speaker, or access remains unresolved.

- BOOK-023
- COURSE-017
- COURSE-018

### DUPLICATE_OR_MIRROR

No indexed source ID is classified solely as `DUPLICATE_OR_MIRROR` in this audit.

## Sources With Claims

| Source Type | Source IDs | Claims |
|---|---|---:|
| WEB | WEB-001, WEB-002, WEB-003, WEB-004, WEB-005, WEB-006, WEB-008, WEB-016, WEB-018 | 103 |
| WEBINAR | WEBINAR-001, WEBINAR-002 | 26 |
| VIDEO | VIDEO-001, VIDEO-002, VIDEO-003, VIDEO-004, VIDEO-005, VIDEO-006, VIDEO-007, VIDEO-008, VIDEO-009, VIDEO-010, VIDEO-011, VIDEO-012, VIDEO-013, VIDEO-014, VIDEO-015, VIDEO-016, VIDEO-018, VIDEO-019, VIDEO-020, VIDEO-022, VIDEO-023, VIDEO-024, VIDEO-025 | 208 |
| TOTAL | 34 sources | 337 |

## Reviewed Zero-Claim Sources

- WEB-009: software account, purchase, activation-code, dashboard, or product/terms material only.
- WEB-010: product details and terms-of-use material only; locked or subscription software content was not accessed.
- WEB-011: resource-index page only; linked downloads and assignments were not accessed.
- WEB-012: resource-index and offer page only; linked videos, downloads, and embedded media were not used.
- WEB-013: consultation service overview only.
- WEB-014: business advisory service copy only.
- WEB-015: homepage/service overview with duplicated service-summary copy only.
- WEB-017: seminar/media report with duplicate candidates and promotional or safety-sensitive business language only.
- WEBINAR-003: official-channel and Qi Men relevant, but timestamped spoken content identifies the presenter as Lee, not Joey Yap.
- WEBINAR-004: official-channel and Qi Men relevant, but reviewed timestamped content is led by Joey Yap team/coaches rather than Joey Yap direct teaching.
- WEBINAR-005: official-channel and Qi Men relevant, but reviewed timestamped content is led by Joey Yap team/coaches rather than Joey Yap direct teaching.
- WEBINAR-007: official captions were reviewed, but Joey Yap direct Qi Men teaching was not confirmed from timestamped content.
- VIDEO-021: official captions were reviewed; the recording is Qi Men relevant but promotional/introductory rather than knowledge-bearing.

## Sources Still Blocked

- COURSE-006: locked coaching-call material requires enrolled access or official transcript/replay.
- VIDEO-017: public official video metadata is accessible, but no official subtitles, automatic captions, or reliable timestampable representation were available.
- WEBINAR-006: public official recording is accessible, but no official English captions or reliable timestampable transcript were available.
- WEBINAR-008: official event page only; no public official recording, replay transcript, or timestamped content was available from the indexed page.
- WEBINAR-009: official event pages only; no public official recording, replay transcript, or timestamped content was available from the indexed pages.

## Unresolved Sources

- BOOK-023: indirect official references exist, but no standalone official listing, canonical product page, or source access has been confirmed.
- COURSE-017: official locked JY Academy lesson page exists, but the course container, instructor, and accessible material remain unresolved.
- COURSE-018: official offer-page reference exists, but no standalone official page, accessible material, or author/speaker confirmation has been confirmed for the source itself.

## Duplicate And Mirror Relationships

- WEB-001 has a JoeyYap.com tutorial URL and an official Mastery Academy article-family URL. Claims were extracted once from the canonical reviewed article context.
- VIDEO-001 and the Buzzsprout Ep12 podcast page represent the same recording family. The canonical YouTube video record was extracted; the podcast feed remains discovery/index only.
- PODCAST-001 may index or mirror official YouTube mini-topic recordings. It remains discovery/index only, and extraction must continue to use canonical item-level records.
- Several BOOK records preserve older JoeyYap.com title styling and current official store title styling as title-family notes under stable BOOK IDs.
- COURSE-012 excludes the later 2025 Joe Boey edition; that page is not canonical for Joey Yap direct extraction under COURSE-012.

## Skipped Eligible Sources

None found.

All currently verified accessible sources that were extraction-eligible have either:

- an extracted claim file with atomic claims, or
- a reviewed zero-claim file/report explaining why no legitimate Joey Yap Qi Men knowledge was extractable, or
- a blocker showing reliable source content, transcript, or timestampable review was unavailable.

## Total Atomic Claims Currently Extracted

337 atomic claims.

Count source:

- WEB extraction batches: 103 claims.
- VIDEO extraction batches: 208 claims.
- WEBINAR extraction batches: 26 claims.

## Coverage Check

Every indexed source in `SOURCE_INDEX.md` appears exactly once in one audit classification above.

Classification count total: 94.

Indexed source total: 94.

## Recommendation

A. Extraction phase complete for the currently accessible corpus.

Blocked, unresolved, metadata-only, discovery-only, and duplicate/mirror sources remain outside the current extracted corpus. They may be added later only if official source content, official previews, samples, transcripts, manuals, workbooks, item-level canonical records, or authorized access are acquired and verified.

Do not begin normalization until a separate task explicitly authorizes it.
