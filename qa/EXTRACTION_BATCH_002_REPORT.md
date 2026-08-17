# Extraction Batch 002 Report

## Scope

Atomic claim extraction batch completed on 2026-08-17 during the ATOMIC CLAIM EXTRACTION phase.

Allowed sources reviewed:

- WEB-008: Joey Yap's Qi Men Dun Jia Tools - About
- WEB-009: Joey Yap's Qi Men Dun Jia Tools - Getting Started
- WEB-010: Joey Yap's Qi Men Dun Jia Tools - QiMen Feng Shui Product / Terms Page
- WEB-011: Joey Yap's QiMen Manifesting - Additional Resources
- WEB-012: Joey Yap's QiMen Manifesting Framework - Additional Resources
- WEB-013: Joey Yap Consulting - Consultation Overview
- WEB-014: Joey Yap Consulting - Business Advisory
- WEB-015: Seize the Moment!
- WEB-016: Empowering Your Business with Qi Men Dun Jia
- WEB-017: Go Forth & Conquer With The Sage Art of War Live Seminar
- WEB-018: Learning the Art of Qi Men with Dato' Joey Yap

Excluded sources for this batch:

- WEB-007
- Books
- Courses
- Videos
- Webinars
- Podcasts
- Third-party sources

No normalization, deduplication, project-rule derivation, or cross-source merging was performed.

## Claims Extracted Per Source

| Source ID | Claims Extracted | Output File |
|---|---:|---|
| WEB-008 | 15 | extracted/WEB-008.md |
| WEB-009 | 0 | extracted/WEB-009.md |
| WEB-010 | 0 | extracted/WEB-010.md |
| WEB-011 | 0 | extracted/WEB-011.md |
| WEB-012 | 0 | extracted/WEB-012.md |
| WEB-013 | 0 | extracted/WEB-013.md |
| WEB-014 | 0 | extracted/WEB-014.md |
| WEB-015 | 0 | extracted/WEB-015.md |
| WEB-016 | 11 | extracted/WEB-016.md |
| WEB-017 | 0 | extracted/WEB-017.md |
| WEB-018 | 3 | extracted/WEB-018.md |
| TOTAL | 29 |  |

## Zero-Claim Sources

- WEB-009: Software account, purchase, activation-code, and dashboard instructions only.
- WEB-010: Product details and terms-of-use page only; locked or subscription software content was not accessed.
- WEB-011: Resource-index page only; linked downloads and assignments were not accessed.
- WEB-012: Resource-index and offer page only; linked videos, downloads, and embedded media were not used.
- WEB-013: Consultation service overview only.
- WEB-014: Business advisory service copy only.
- WEB-015: Homepage/service overview with duplicated service-summary copy only.
- WEB-017: Seminar/media report with duplicate candidates and promotional/safety-sensitive business language only.

## Marketing / Service Pages Rejected From Knowledge Extraction

- WEB-009, WEB-010, WEB-013, WEB-014, and WEB-015 were treated as non-knowledge-bearing for this batch because their Qi Men mentions occur in software, service, legal, brand, or consultation copy.
- WEB-011 and WEB-012 were treated as resource indexes; titles of downloads, assignments, and videos were not promoted into SOURCE FACT.
- WEB-017 included promotional business and investment language; those statements were not extracted.

## Duplicate Candidate Claims

- WEB-008 repeated batch 001 themes about Qi Men placing people in the right place at the right time, time-and-space calculation, 3000-year history, 1080 charts, and complex calculations. These were skipped as duplicates.
- WEB-015 repeated broad service-summary claims about right place/right time, forecasting luck through time and space, and Zhuge Liang. These were skipped as duplicates or service-copy statements.
- WEB-017 repeated claims about ancient military use, right place/time, predicting action outcomes, and modern business use. These were skipped as duplicates or promotional restatements.
- WEB-018 overlapped with WEB-008 on Destiny Chart scope, but retained only high-level course/news-report claims not already represented in the same wording and context.

## Ambiguities

- WEB-008 is a software/product information page. Only explicit technical terminology and Qi Men application statements were extracted; software UI features and marketing superlatives were skipped.
- WEB-012 lists Guardian video links hosted on storage.googleapis.com. Those links were not used because this batch excludes videos and linked media.
- WEB-015 was readable only after bypassing a currently time-invalid certificate chain for the official `https://en.joeyyap.com/` page.
- WEB-018 is an official news/activity page about a course. It was not treated as course material; extracted claims are limited to high-level application scope stated on the accessible web page.

## Citation Limitations

- Web pages do not provide page numbers.
- Citations use source ID, author/speaker or corporate author, title, section/page context, and exact URL.
- WEB-011 and WEB-012 include links to downloads and videos, but linked resources were not accessed or cited as evidence.
- WEB-015 has an access limitation due to the official site's certificate chain being time-invalid during review.

## QA Confirmation

- Every extracted claim includes a Do Not Infer field.
- Every extracted claim cites one of WEB-008 through WEB-018.
- No WEB-007, books, courses, videos, webinars, podcasts, third-party sources, or generic Qi Men knowledge were used.
- No software UI behavior, service listing, enrollment promise, or generic marketing claim was promoted into Qi Men SOURCE FACT.
- No atomic claims were normalized or merged.
