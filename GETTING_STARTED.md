# Getting started with Folio

This guide is for the ad-hoc signed 0.9.0-beta.5 test build. Requirements: Apple Silicon Mac, macOS 14+, UNC Canvas access and internet for Canvas/AI. No Python, Node.js or terminal setup is needed to run the app.

1. Download and install

Get the DMG and its SHA-256 file from [Releases](https://github.com/Bensssonxx/folio-releases/releases). Compare the download's checksum with the release asset. A checksum checks file integrity; it is not an Apple signature or notarization. Open the DMG, drag Folio to Applications and launch it there.

If macOS blocks this app without Developer ID/notarization, only proceed if you trust its source and integrity. After trying to open it, System Settings → Privacy & Security may offer Open Anyway for this app; confirm the next prompt. See [Apple's instructions](https://support.apple.com/en-us/102445). Do not disable Gatekeeper globally. If macOS reports damage or malware, stop and report the exact message. Managed Macs may prevent installation.

2. Connect UNC Canvas

Choose Connect Canvas on Home. In UNC Canvas, open Account → Settings → Approved Integrations → New Access Token. Name it and set an expiration. Paste it only into Folio's password field. Folio uses GET requests, but Canvas may issue a more powerful token. Keep it private and revoke it in Canvas when no longer needed. If personal tokens are disabled, this method is unavailable.

3. Add a course

Choose Add course. Accessible materials prepare on this Mac automatically, independently of Save to Mac. Initial downloads/indexing may take longer. Course materials shows ready, failed, unavailable and unsupported sources. Update checks for changes; retry retries failed preparation.

4. Choose your AI connection

Open Chat → Connect AI (or AI settings). Choose **ChatGPT → Continue with ChatGPT** to authorize Folio in your browser. Review the account and permissions on OpenAI's page; your password is never entered into Folio. Return to Folio and choose a model from the list returned for that account. Access depends on the account, workspace and app eligibility enforced by OpenAI; a subscription alone does not guarantee access. You can cancel, change accounts or sign out in AI settings.

Alternatively choose **API key → Pay separately**, enter your own OpenAI API key and a model ID available to that API account, then explicitly save it to use the API. API billing is separate from a ChatGPT subscription. Folio does not switch to API billing automatically if subscription access fails. No account or key is provided with the installer. Connecting alone does not send course material; review the course sharing message before Enable and send.

5. Ask and check

Choose a course and ask a question. Current-status questions query live sources. Selected originals are read directly. Automatic materials uses local keyword/similarity search when you do not know the source. Click a numbered reference to reopen it and check whether it supports the answer. Complete readings can send all selected text and page images across multiple requests.

Choose sources groups Files, Assignments, Announcements and Pages & links. Under Assignments, open My submissions & feedback to preview available personal records. Check only the items you want analyzed and review the staged list before Send. Previewing does not send them. Successful private analyses clear their selection and are excluded from later AI conversation context; select the records again for another analysis.

## Upgrading from CourseVault

Quit the old app before launching Folio. The data folder, restored-profile pointer and credential identity remain compatible; do not move or rename them. The apps cannot share that profile simultaneously. Existing ChatGPT connections remain on this Mac; choose one explicitly or authorize again if required. Refresh Calendar to verify previously inferred dates. Keep a backup and the previous app until you have checked the upgrade.

## Recovery and support

Settings shows local storage and the data folder. Removing a course hides it without erasing its files. Backup exports app-owned data without credentials; user-selected external folders need separate backups. Restore makes a verified new copy; activate it explicitly and reconnect the same Canvas account.

Expired Canvas tokens require reconnecting. ChatGPT authorization or eligibility errors are shown in AI settings; check the selected account and its connected-app permissions. API errors require checking the account's key, billing, model access and limits. Stop remains available during long answers; network/model time varies. Unsupported/inaccessible sources are disclosed. A changed original can invalidate an old reference.

Report version/build, error category and reproduction steps with synthetic data in [Issues](https://github.com/Bensssonxx/folio-releases/issues). Do not post credentials, private course materials or full chats. Follow [Security](SECURITY.md) for vulnerabilities.

Beta.3 corrected the incomplete bundle signature in beta.2. It does not add Apple Developer ID or notarization. macOS may still require explicit approval for this specific app; no global security setting changes are needed or recommended. A second Mac has not yet verified this release.

## Optional PowerPoint page support

The main installer no longer includes the full Office converter. Opening a PowerPoint slide file asks to download document support: 298 MB from The Document Foundation, about 798 MB installed. You can choose Not now or cancel the progress window. PDF, text and Word text reading remain available. After installation, the same version is reused without another download, including across local data spaces. Settings → local storage includes Document support separately. An internet connection and about 1.5 GB free temporary space are needed for installation; offline use works once installed.

Folio checks the pinned SHA-256, official publisher signature and macOS trust before making this support executable available. A failed verification is never installed. Course files are not uploaded during download. The base application is smaller; installing the optional component later adds its size to your Mac.

Background indexing continues with readable materials while optional support is absent. After installation, failed slide indexes are retried locally; prepared originals are reused.
