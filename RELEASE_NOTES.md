# Folio 0.9.0-beta.3 — bundle signature repair, API-only beta

Fixes the incomplete application bundle signature in beta.2 that could cause a damaged-app warning even when the download checksum matched. Electron frameworks/helpers and the outer app now have a complete ad-hoc signature. The packaging and installer checks require whole-bundle signature integrity; the separate official Office engine is preserved unchanged.

**This is an unsigned-by-Apple test build: it is not Developer ID-signed and has not been notarized.** Ad-hoc integrity does not grant automatic Gatekeeper approval. macOS may still block first launch; follow the per-app steps in [Getting started](https://github.com/Bensssonxx/folio-releases/blob/main/GETTING_STARTED.md) only if you trust the verified download. Do not disable global security protections. Stop and report a persistent damaged/malware warning.

Apple Silicon, macOS 14+. Bring your own API key with separate API billing. ChatGPT subscription login remains disabled. Existing data, internal identity and legacy credentials are preserved; quit the old app before opening this version. No changes to course/feedback selection, AI context or reading behavior.

The installer includes the same official LibreOffice 26.2.6.3 engine, third-party notices and source access. Folio implementation source remains private. Local synthetic acceptance does not substitute for a second Mac or fresh real API account.
