# Folio for UNC

Your courses, ready to talk about.

Folio is a local-first Mac workspace for Canvas materials, assignments, instructor feedback and AI conversations. Answers link back to the original material. Saving your own copies is optional.

**0.9.0-beta.3 — ad-hoc signed, unnotarized pre-release (no Developer ID).** This is an early test build for Apple Silicon Macs running macOS 14 or later. AI uses your own API key and separate API billing. ChatGPT subscription sign-in is disabled in this build.

[Download the test installer](https://github.com/Bensssonxx/folio-releases/releases) · [Getting started](GETTING_STARTED.md) · [Privacy](PRIVACY.md) · [Release notes](CHANGELOG.md)

## What you can do

- Browse course files, assignments, announcements and linked pages.
- Open available past submissions and instructor feedback in Folio. Choose individual items for each AI request; previewing alone does not send them.
- Check current information against live sources, read selected originals directly, or find relevant material with local keyword and semantic search.
- Read PDFs, slides, supported document text and saved Notebook output/images. Notebook code is never executed.
- Open answer references to verify the original source and use course dates in full or smaller windows.

You need UNC Canvas access, internet for Canvas/AI and your own supported API account. An API key is billed separately from a ChatGPT subscription. You choose a model available to that API account; model availability and usage limits depend on the provider.

## Installing this beta

The app is not Developer ID-signed or notarized by Apple. macOS may block its first launch. Only if you trust the download and have verified it, follow the per-app instructions in [Getting started](GETTING_STARTED.md). Managed Macs may not permit an exception. No global security-setting changes are required by Folio.

Existing CourseVault users: quit the old app before opening Folio. Existing data and credential identities are preserved. Existing ChatGPT connections remain stored but are not used by this API-only beta. Make a backup before upgrading.

Folio is an independent student project, not an official UNC, Canvas or OpenAI product. Verify AI answers and inferred dates against their sources and follow your course's AI rules. Some Canvas annotations or external-system feedback require importing an exported file. Source coverage and answer speed vary.

This repository contains downloads and public documentation. Folio application source remains private. Third-party notices and required source access are described in [Third-party software](THIRD_PARTY_NOTICES.md) and [Sources](SOURCES.md). Do not upload course files, credentials, chat histories or private diagnostic records here.

The beta.3 bundle has a complete ad-hoc integrity signature. It is not Developer ID-signed or notarized, so macOS does not automatically trust it. The earlier beta.2 package had an incomplete bundle seal and should not be installed.
