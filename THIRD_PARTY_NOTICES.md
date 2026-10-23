# Third-party software

Folio's application source is private. Third-party components retain their own copyright, licenses and corresponding-source rights. Their terms are not restricted by Folio's application license.

The installed app's Contents/Resources/notices folder contains a dependency inventory, full collected license texts, Electron/Chromium acknowledgments, Python/OpenSSL notices, model provenance, Office LICENSE/LICENSE.html/NOTICE, source-access records and native transitive notices. Source-lock inventories can include build-only and non-macOS packages; they are not a claim that every listed crate is linked into the runtime.

Components include Electron/Chromium, Angular, RxJS, PDF.js, KaTeX/fonts, the Python runtime and frozen sidecar, PyInstaller's runtime with its bootloader exception, pypdf, Pillow, APSW/SQLite, sqlite-vec, NumPy, ONNX Runtime, tokenizers, jieba, certifi, multilingual-e5-small, Canvas/Skia and its codecs/font libraries, and the separate LibreOffice presentation engine.

License highlights and source access:

- LibreOffice 26.2.6.3 is an unmodified official The Document Foundation Apple Silicon release. Its exact official source archives and external-source catalog are listed in SOURCES.md and the installed notice records. Its embedded signature does not sign or notarize Folio itself.
- The Liberation Sans 1.07.4 fonts supplied by PDF.js use GPLv2 with the Liberation font exception, not the SIL license of later Liberation releases. Their full license/exception and preferred SFD source archive accompany the installer.
- The MPL-covered Rust modules and certifi have exact source archives included with their notices. Their source rights do not publish Folio's independent private files.
- Canvas/Skia notices include the upstream project, Rust crate sources, FreeType and the relevant image/text libraries. FreeType attribution and its full license are included.
- The model's pinned card declares MIT. Its original card, asset hashes and upstream MIT license are included. KaTeX and its font sources retain the upstream MIT notice.

See [Sources](SOURCES.md) for exact versions, links and archive hashes. This index does not replace the full component licenses inside the installer.

Portions of this software are copyright © The FreeType Project (www.freetype.org). All rights reserved.

In beta.5, LibreOffice is optional support downloaded directly from the publisher after consent. Its official licenses remain in the downloaded component; source links and notices remain available here.
