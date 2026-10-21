# Third-party source access

These are sources for third-party components, separate from Folio's proprietary application source.

## LibreOffice presentation engine

Version: 26.2.6.3, ARM64. Official binary build ID and source tag commit: 8221e31b3ac356a1623c672912a3d2b492f7e3d1. The installed directory is named LibreOfficeDev.app for compatibility with the app's existing lookup; its contents are the official stable release, not a development build.

- [Official ARM64 binary](https://download.documentfoundation.org/libreoffice/stable/26.2.6/mac/aarch64/LibreOffice_26.2.6_MacOS_aarch64.dmg), SHA-256: `94bb3248df074c225490a8a6d1d9dc87c7d6783dbb7a8e9f0d0c3d94348552af`.
- [Core source archive](https://download.documentfoundation.org/libreoffice/src/26.2.6/libreoffice-26.2.6.3.tar.xz), SHA-256: `3a2570aa7087bf8e0cbdf49ac5bd0e452c2025274af99e07882daa104c5685bd`.
- [Dictionary sources](https://download.documentfoundation.org/libreoffice/src/26.2.6/libreoffice-dictionaries-26.2.6.3.tar.xz), SHA-256: `5c0b2acf3d734d2cede32e3b37b5fbdd73dda9a1fbe6b5a00d98f7e234a40c9b`.
- [Exact external-source catalog and build source](https://git.libreoffice.org/core/+/8221e31b3ac356a1623c672912a3d2b492f7e3d1/download.lst). A copy of download.lst and sources.ver accompanies the installer; the catalog records the external source archive versions and checksums. [External source mirror](https://dev-www.libreoffice.org/src/).

## Other components

The installed Contents/Resources/notices/supplements folder includes:

- `fonts/liberation-fonts-1.07.4.tar.gz`: preferred font sources, build scripts and original licensing, obtained from [Debian's original upstream source archive](https://deb.debian.org/debian/pool/main/f/fonts-liberation/fonts-liberation_1.07.4.orig.tar.gz).
- `rust-sources/`: exact MPL-covered cssparser, cssparser-color, cssparser-macros and dtoa-short source crates.
- `python-sources/`: exact certifi source archive.
- `provenance/rust-inventory.json`: pinned crate versions, exact source archive URLs/checksums and notice hashes for Canvas/tokenizers source-lock dependencies.
- `provenance/skia-inventory.json`: Skia commit a9c42c9fce77cd748805df0ec67ef5718800b1e9 and pinned third-party repository/source links.
- `provenance/python-source-access.json`: exact PyPI source links/checksums for pinned Python dependencies where published.
- `office/corresponding-source.json`: the Office binary/source records above.

Python runtime 3.12.8 sources are available from [CPython v3.12.8](https://github.com/python/cpython/tree/v3.12.8); OpenSSL 3.0.15 from [the exact upstream tag](https://github.com/openssl/openssl/tree/openssl-3.0.15). Electron's source and Chromium version mapping are available from [Electron v43.4.1](https://github.com/electron/electron/tree/v43.4.1). Model provenance is pinned to intfloat/multilingual-e5-small revision 614241f622f53c4eeff9890bdc4f31cfecc418b3. Full licenses and hashes remain with their corresponding installed files.
