# Getting started with Folio

This guide is for the unsigned API-only 0.9.0-beta.2 test build. Requirements: Apple Silicon Mac, macOS 14+, UNC Canvas access and internet for Canvas/AI. No Python, Node.js or terminal setup is needed to run the app.

1. Download and install

Get the DMG and its SHA-256 file from [Releases](https://github.com/Bensssonxx/folio-releases/releases). Compare the download's checksum with the release asset. A checksum checks file integrity; it is not an Apple signature or notarization. Open the DMG, drag Folio to Applications and launch it there.

If macOS blocks this unsigned app, only proceed if you trust its source and integrity. After trying to open it, System Settings → Privacy & Security may offer Open Anyway for this app; confirm the next prompt. See [Apple's instructions](https://support.apple.com/en-us/102445). Do not disable Gatekeeper globally. If macOS reports damage or malware, stop and report the exact message. Managed Macs may prevent installation.

2. Connect UNC Canvas

Choose Connect Canvas on Home. In UNC Canvas, open Account → Settings → Approved Integrations → New Access Token. Name it and set an expiration. Paste it only into Folio's password field. Folio uses GET requests, but Canvas may issue a more powerful token. Keep it private and revoke it in Canvas when no longer needed. If personal tokens are disabled, this method is unavailable.

3. Add a course

Choose Add course. Accessible materials prepare on this Mac automatically, independently of Save to Mac. Initial downloads/indexing may take longer. Course materials shows ready, failed, unavailable and unsupported sources. Update checks for changes; retry retries failed preparation.

4. Connect your API account

Open Chat → AI settings. Enter your own OpenAI API key and a model ID available to that API account. API billing is separate from a ChatGPT subscription. No key is provided with the installer. Saving a key does not send course material; review the course sharing message before Enable and send. ChatGPT subscription sign-in is not available in this beta, and existing subscription credentials are preserved without being read or changed.

5. Ask and check

Choose a course and ask a question. Current-status questions query live sources. Selected originals are read directly. Automatic materials uses local keyword/similarity search when you do not know the source. Click a numbered reference to reopen it and check whether it supports the answer. Complete readings can send all selected text and page images across multiple requests.

Choose sources groups Files, Assignments, Announcements and Pages & links. Under Assignments, open My submissions & feedback to preview available personal records. Check only the items you want analyzed and review the staged list before Send. Previewing does not send them. Successful private analyses clear their selection and are excluded from later AI conversation context; select the records again for another analysis.

## Upgrading from CourseVault

Quit the old app before launching Folio. The data folder, restored-profile pointer and credential identity remain compatible; do not move or rename them. The apps cannot share that profile simultaneously. Existing ChatGPT connection files remain stored for a compatible local build; this beta uses a separate API connection. Refresh Calendar to verify previously inferred dates. Keep a backup and the previous app until you have checked the upgrade.

## Recovery and support

Settings shows local storage and the data folder. Removing a course hides it without erasing its files. Backup exports app-owned data without credentials; user-selected external folders need separate backups. Restore makes a verified new copy; activate it explicitly and reconnect the same Canvas account.

Expired Canvas tokens require reconnecting. API errors require checking the account's key, billing, model access and limits. Stop remains available during long answers; network/model time varies. Unsupported/inaccessible sources are disclosed. A changed original can invalidate an old reference.

Report version/build, error category and reproduction steps with synthetic data in [Issues](https://github.com/Bensssonxx/folio-releases/issues). Do not post credentials, private course materials or full chats. Follow [Security](SECURITY.md) for vulnerabilities.
