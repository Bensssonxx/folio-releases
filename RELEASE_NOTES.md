# Folio 1.0.0 — first stable release

Folio brings Canvas courses, materials, assignments, available past submissions and instructor feedback into one local Mac workspace. Preview personal records in the app and choose individual items for each AI request. Current-status questions check live sources; selected originals are read directly; local keyword and semantic search helps find material when its location is unknown. Answers link back to their sources.

## Install or upgrade

Apple Silicon Mac, macOS 14 or later. Quit every old Folio or CourseVault copy, open the DMG, drag Folio to Applications and open it there. Existing local data, restored profiles and credential identity are preserved. Reinstalling is not a data reset. Make a local backup before upgrading. Updates are manual through GitHub Releases.

This release has a complete ad-hoc integrity signature, but no Apple Developer ID or notarization. macOS may require per-app approval in Privacy & Security; managed Macs may disallow it. A checksum verifies the downloaded bytes, not Apple trust. Do not disable global security protections or remove security attributes to bypass an error. See [Getting started](GETTING_STARTED.md).

## AI and document support

Continue with ChatGPT remains a preview for accounts, workspaces and apps eligible under OpenAI's service. A subscription alone does not guarantee access. The API-key option is explicitly selected and separately billed; subscription failures never silently switch to API billing. Connecting or previewing a file alone does not send course content. Review each course's sharing settings and AI rules.

PDFs, plain text and Word text work without the optional converter. Opening PowerPoint pages asks before a verified 298 MB download from The Document Foundation (about 798 MB installed, about 1.5 GB temporary free space needed). Not now and Cancel are available. The same version is shared across local data spaces; installation retries failed slide indexes without redownloading originals. Settings counts Document support separately from course databases.

## Validation and known limits

Version 1.0.0 preserves beta.5's reading and AI implementations. That baseline passed 18 optional-component tests, a real official-component download and publisher/trust verification, synthetic PPTX/DOCX reading and failed-index recovery, progress/cancel UI, exact package checks and an isolated final-app offline launch. The stable package additionally verifies release identity, empty-profile onboarding, synthetic upgrade persistence, embedded help, window sizes, bundle integrity and the DMG. These checks use synthetic profiles and no real course or AI requests.

Fresh real-account authorization, answer quality with a real course and installation on a second Mac remain unverified. Some external-system feedback and Canvas annotations require importing an export. The first macOS file picker can be slow on some Macs. Verify AI answers and inferred dates against original sources. Stop and report an integrity, damaged-app or malware warning.

This is an independent project, not an official UNC, Canvas or OpenAI application. This repository contains installers and public documentation only; Folio source remains private. See [Privacy](PRIVACY.md), [Third-party notices](THIRD_PARTY_NOTICES.md), [Sources](SOURCES.md) and [Security](SECURITY.md).
