# Privacy and AI sharing

Updated 2026-10-23 for beta.4.

Folio stores its course catalog, prepared originals, keyword/semantic indexes, chats, attachments and history on this Mac. Personal Save and automatic Chat preparation are separate. External workspace folders stay where you selected them. Backups can contain private course/chat data; protect them.

## Canvas and instructor sites

Folio sends read requests to your configured Canvas school and downloads material your account can access. It may fetch confirmed instructor-site pages and linked documents within its discovery rules. Those services receive normal network request information. The app does not submit assignments, post announcements or modify grades.

## Credentials and AI

Canvas, ChatGPT and API credentials use macOS-backed Electron secure storage in the main process. Keys are not exposed to the web interface or included in profile backups. Disconnection removes the local connection; revoke tokens/keys separately with their provider when needed. Protect your Mac account.

You choose ChatGPT subscription access or your own API key. ChatGPT sign-in opens OpenAI's authorization page in your system browser and uses PKCE, a local loopback callback and encrypted credentials for the selected local profile. OpenAI receives the OAuth registration/authorization request and decides eligibility. Selecting a saved connection may refresh its authorization or available model list. Sign-out attempts remote revocation and clears local tokens; if revocation cannot be confirmed, Folio tells you to review connected-app permissions. No Folio-operated authentication relay is used.

An API key uses separate API billing, outside a ChatGPT subscription. Connection or eligibility errors never silently switch billing to an API key. Availability of the subscription preview is not a claim of OpenAI partner approval or access for every account.

After you enable AI for a course and press Send, Folio sends the question, permitted conversation context, material titles, supporting text and applicable document/page images to the displayed AI connection. Complete reading may send complete selected originals over multiple requests. Previewing or attaching alone does not send them. A changed account/provider/model can require consent again. Turn sharing off in AI settings or disconnect to prevent future requests. Content already sent cannot be recalled. Provider retention, account controls and billing are governed by its terms; Folio does not promise zero provider retention.

## Personal submissions and feedback

Opening, downloading into the separate personal-material cache or previewing a personal record does not send it to AI. Check individual submissions, attempts, feedback, rubric criteria/points or scores, then review the staged sources before Send. Only those staged private sources participate in the request. Success clears the selection; Stop or failure retains it for retry. Private analyses remain visible locally and are excluded from later model context, summaries and planning. Imported feedback follows the same rules.

New private-analysis history is stored separately so older builds cannot inadvertently send it. Earlier history is preserved; separate conversations later created in an older build are not automatically merged. Private originals and analyses can appear in credential-free local backups.

## Retention and diagnostics

Removing a course or disconnecting Canvas preserves course data. Deleting a conversation removes its history, but shared cached originals can remain. Restoring preserves both old and restored data until you remove a copy. For complete removal, export what you need, quit Folio, remove its app-owned data/backups and revoke provider credentials. Uninstalling the app alone does not remove its data. Do not delete external workspace folders accidentally.

Folio has no built-in advertising or product analytics collector. Local diagnostics can contain paths, questions and source details; review before sharing. OS crash reporting, Electron and connected services have their own policies. Updates are obtained manually from [Releases](https://github.com/Bensssonxx/folio-releases/releases). Do not place credentials, private course files or full chats in public issues.
