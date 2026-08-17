# Research Status

## Current Phase

ATOMIC CLAIM EXTRACTION

## Current Task

Begin atomic claim extraction from verified accessible sources.

Extract only from sources approved in `qa/SOURCE_VERIFICATION_REPORT.md`.

## Completed

- Repository created
- AGENTS.md created
- RESEARCH_RULES.md created
- SOURCE_INDEX.md created
- SOURCE_QUEUE.md created
- KNOWLEDGE_SCHEMA.md created
- Research infrastructure setup completed
- Inventory Joey Yap Qi Men books completed
- Inventory official courses and training materials completed
- Inventory official websites completed
- Inventory direct Joey Yap Qi Men media sources completed
- Source verification pass completed
- Atomic extraction batch 001 completed for WEB-001 through WEB-006
- Atomic extraction batch 002 completed for WEB-008 through WEB-018
- Media extraction batch 001 completed for VIDEO-001 through VIDEO-005

## In Progress

- Atomic claim extraction

## Pending

1. Continue atomic claim extraction from remaining verified accessible media sources
2. Normalize extracted claims
3. Deduplicate / cross-source reconciliation
4. QA extracted claims
5. Project-rule derivation

## QA Issues

- BOOK-023 remains unresolved: official Joey Yap descriptions indirectly reference `Qi Men Dun Jia Ten Thousand Year Calendar`, but no standalone official listing or source access was confirmed during verification.
- COURSE-012 verification separated Joey Yap-led Mastery Academy 2013/2014 pages from the later 2025 Joe Boey edition; the 2025 edition is prohibited from extraction under COURSE-012.
- COURSE-013 through COURSE-016 are verified from official Mastery Academy index metadata, but detail pages or workbook/manual access were not resolved during inventory.
- COURSE-017 is a locked JY Academy course-material page; course container, instructor, and content access remain unresolved.
- COURSE-018 is referenced from an official offer page, but no standalone official page, accessible material, or author/speaker confirmation for the source itself was confirmed.
- WEB-001 has a JoeyYap.com mirror and Mastery Academy original; avoid duplicate extraction.
- WEB-010 has partial product/terms access only; locked software content remains inaccessible.
- WEB-011 and WEB-012 reference downloadable or embedded resources, but those materials were not opened or extracted during web-source inventory.
- WEBINAR-007 and VIDEO-025 are provenance/QiMen-relevance verified from official YouTube metadata, but their titles remain non-specific; timestamp-level review is required before extraction.
- WEBINAR-008 and WEBINAR-009 are official event pages with no public recording URL confirmed during media inventory.
- PODCAST-001 is an official discovery/index feed that may contain podcast mirrors or parallel audio for some official YouTube recordings; extract only from canonical item-level records.
- Third-party uploads and channels, including TheFengShuiChannel and other non-Joey Yap uploaders, were treated only as discovery evidence unless official provenance could be independently confirmed.
- Official Telegram/Facebook references may point to time-limited or removed replays; item-level official recording URLs remain unresolved unless listed in SOURCE_INDEX.md.
- Extraction batch 001 created 74 atomic claims from WEB-001 through WEB-006 only; see `qa/EXTRACTION_BATCH_001_REPORT.md` for skipped claims, ambiguities, and citation limits.
- Extraction batch 002 created 29 atomic claims from WEB-008, WEB-016, and WEB-018; WEB-009 through WEB-015 and WEB-017 produced zero-claim files under the knowledge-bearing source-scope rule.
- Media extraction batch 001 created 48 atomic claims from VIDEO-001 through VIDEO-005 using only official Joey Yap YouTube videos with timestamped English (Original) automatic captions; see `qa/MEDIA_EXTRACTION_BATCH_001_REPORT.md` for caption limitations and case-specific ambiguities.

## Next Task

Continue atomic claim extraction from remaining verified accessible media sources.

## Completed Source Inventory Criteria

SOURCE INVENTORY was considered complete for the currently discoverable scope when:

- all major discoverable Joey Yap Qi Men books are listed
- official courses/training materials have been searched
- official web sources have been searched
- official/direct Joey Yap media sources have been searched
- every discovered source has a source ID
- every source has a source type and verification status
- no Qi Men knowledge has been extracted yet
