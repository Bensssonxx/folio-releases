# Folio 0.9.0-beta.5 — smaller installer, optional PowerPoint support

The complete Office engine is now an optional first-use download rather than part of the main application. Opening PowerPoint slide pages asks before downloading 298 MB from The Document Foundation, verifies the pinned checksum, official publisher and macOS trust, then installs about 798 MB in a shared local components folder. Progress has Cancel; Not now keeps it uninstalled. Installation needs about 1.5 GB free temporary space. PDFs, plain text and Word text work without it. Later uses and data spaces reuse the installed version.

This reduces initial installation size. Installing the optional engine later still uses its disk space. Settings shows Document support separately. The converter is not a database; course originals, extracted pages and search indexes have separate storage.

ChatGPT sign-in preview and the explicitly billed API-key option remain. OpenAI decides account/workspace/app eligibility; errors never silently switch to API billing. Existing data and credential identity remain compatible. Quit the old app before installing. Source stays private; this repository contains documentation and installers only.

Apple Silicon/macOS14+. Complete ad-hoc integrity signature, no Apple Developer ID or notarization. macOS may require explicit per-app approval. Validation covers isolated component failure/cancel paths, real official component download and synthetic PPTX/DOCX reading, UI progress/cancel, exact package and offline launch. Fresh real-account authorization and a second Mac remain unverified.

Background indexing continues with readable materials while optional support is absent. After installation, failed slide indexes are retried locally; prepared originals are reused.
