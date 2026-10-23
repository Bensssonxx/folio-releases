# Folio for UNC

Your courses, ready to talk about.

Folio is a local-first Mac workspace for Canvas materials, assignments, instructor feedback and AI conversations. Answers link back to the original material. Saving your own copies is optional.

**Folio 1.0.0 — first stable release for Apple Silicon Macs running macOS 14 or later.** The app has an ad-hoc integrity signature, without Apple Developer ID or notarization. Continue with ChatGPT is available as a preview for eligible accounts and workspaces. The API-key option remains separately billed.

[Download Folio 1.0.0](https://github.com/Bensssonxx/folio-releases/releases/tag/v1.0.0) · [Getting started](GETTING_STARTED.md) · [Privacy](PRIVACY.md) · [Release notes](CHANGELOG.md)

## What you can do

- Browse course files, assignments, announcements and linked pages.
- Open available past submissions and instructor feedback in Folio. Choose individual items for each AI request; previewing alone does not send them.
- Check current information against live sources, read selected originals directly, or find relevant material with local keyword and semantic search.
- Read PDFs, slides, supported document text and saved Notebook output/images. Notebook code is never executed.
- Open answer references to verify the original source and use course dates in full or smaller windows.

You need UNC Canvas access, internet for Canvas/AI, and an eligible ChatGPT connection or your own supported API account. An API key is billed separately from a ChatGPT subscription. You choose a model available to that API account; model availability and usage limits depend on the provider.

## Installation and updates

The app is not Developer ID-signed or notarized by Apple. macOS may block its first launch. Only if you trust the download and have verified it, follow the per-app instructions in [Getting started](GETTING_STARTED.md). Managed Macs may not permit an exception. No global security-setting changes are required by Folio.

Existing CourseVault users: quit the old app before opening Folio. Existing data and credential identities are preserved. Existing ChatGPT connections stay on this Mac; you can explicitly choose a connection or sign in again. Make a backup before upgrading.

Folio is an independent student project, not an official UNC, Canvas or OpenAI product. Verify AI answers and inferred dates against their sources and follow your course's AI rules. Some Canvas annotations or external-system feedback require importing an exported file. Source coverage and answer speed vary.

This repository contains downloads and public documentation. Folio application source remains private. Third-party notices and required source access are described in [Third-party software](THIRD_PARTY_NOTICES.md) and [Sources](SOURCES.md). Do not upload course files, credentials, chat histories or private diagnostic records here.

This bundle has a complete ad-hoc integrity signature. It is not Developer ID-signed or notarized, so macOS does not automatically trust it. The earlier beta.2 package had an incomplete bundle seal and should not be installed.

PowerPoint page support is optional: Folio asks before a one-time 298 MB download (about 798 MB installed) from The Document Foundation. PDFs, plain text and Word text work without it. The component is shared across Folio data spaces and stays separate from course databases.

Updates are manual. Version 1.0.0 carries the beta.5 feature set into the stable channel, with corrected in-app release information. Fresh-account AI access and installation on a second Mac have not been independently verified. See [Release notes](RELEASE_NOTES.md) for the tested scope.
