# Changelog

## 1.0.0 — 2026-10-23

- First stable release, based on the beta.5 feature set: Canvas courses, local material search, assignment/feedback previews and per-request AI source selection.
- Keep browser ChatGPT sign-in as an eligibility-dependent preview and API keys as an explicit, separately billed choice.
- Keep the smaller base installer and verified optional PowerPoint page support. Preserve existing data, profile and credential identity.
- Correct the in-app distribution label and publish installation, upgrade, privacy and support guidance for the stable channel. Updates remain manual.
- Complete ad-hoc integrity signature; no Apple Developer ID or notarization. Second-Mac installation and fresh real-account AI access remain unverified.

## 0.9.0-beta.5 — 2026-10-23

- Remove the complete Office engine from the main installer. Offer verified, cancellable first-use PowerPoint page support (298 MB download, about 798 MB installed), shared across local data spaces.
- Keep PDF, plain text and Word text reading independent of the optional component. Count installed document support separately in local storage.
- Preserve ChatGPT/API connections, data compatibility and explicit private-material sharing. Stop prevents postponed work from restarting after installation.

## 0.9.0-beta.4 — 2026-10-23

- Restore Continue with ChatGPT in both the local test and public build, using direct browser authorization and account-provided model access.
- Keep the API-key option and explicit separate billing; authorization, eligibility or quota errors do not silently switch connections.
- Clarify the subscription eligibility error. Preserve course data, credentials, internal application identity and all existing reading/selection behavior.
- Retain the complete ad-hoc bundle seal from beta.3. Apple Developer ID and notarization are still unavailable.

## 0.9.0-beta.3 — 2026-10-21

- Repair the whole macOS bundle signature and resource seal; preserve the official Office engine and reading binaries.
- Enforce complete signature integrity for every beta, packaging audit and DMG creation; distinguish this from missing Developer ID/notarization.
- Add rejection checks for the old invalid package and modified sealed resources.
- No change to saved data, per-Send private selection or API-only policy.

Beta.2 had an incomplete application signature and should not be installed. Its artifacts and launch-issue notice are retained for traceability.

## 0.9.0-beta.2 — unsigned API-only pre-release

- Uses your own API key with explicit separate billing. ChatGPT subscription login and inference are disabled in the public build; legacy connection files remain untouched.
- Replaces the development presentation engine with the official Apple Silicon LibreOffice 26.2.6.3 release, pinned to the publisher's checksum and source revision.
- Adds missing Chromium/Python/native/font notices, native transitive inventories, exact source access and Liberation font sources.
- Retains the Folio name/icon, existing data compatibility, personal feedback selection, window layouts, course-date fixes and top-to-bottom answer generation from the local review builds.

Apple Silicon / macOS 14+. Unsigned and unnotarized. Some managed Macs may prevent installation. API key/billing/model access is supplied by each tester. Source availability and AI speed vary; some Canvas annotations and external grading-system feedback need imported exports. The first native file picker can still be slow on some Macs. Current Calendar inference needs a successful refresh. Important answers and dates should be checked against the original sources.

## Earlier local review builds

0.9.0-beta.1 was used for private local reviews, including the Folio rename, personal submission/feedback reading, source categories, responsive windows, Calendar date association and answer streaming order. It was not a public release.
