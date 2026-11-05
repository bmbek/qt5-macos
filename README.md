# Qt 5.15 for macOS (universal)

GitHub Actions workflow that builds the **open-source Qt 5.15 LTS** sources
published on [download.qt.io](https://download.qt.io/archive/qt/5.15/) for macOS
as universal binaries (arm64 + x86_64), plus a static universal OpenSSL.

Run **Actions → Build Qt 5.15 for macOS (universal) → Run workflow**.
The result is published as a release `qt-<version>-macos-universal` with:

- `qt-<version>-macos-universal.tar.xz` — Qt install prefix (relocatable via `bin/qt.conf`)
- `openssl-<version>-macos-universal.tar.xz` — static `libcrypto.a` / `libssl.a` and headers

Modules: qtbase, qtsvg, qtimageformats, qtdeclarative, qtremoteobjects,
qtwebsockets, qtquickcontrols, qtquickcontrols2, qtgraphicaleffects, qtcharts,
qttools, qttranslations.

## License

Qt is licensed under LGPLv3 / GPLv2 / GPLv3 (see the license files inside the
archive); OpenSSL 3 under Apache 2.0. This repository only contains build scripts.
