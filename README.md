# POE BOTTARI Releases

This repository is the official download, release-note, privacy, and support page for **POE BOTTARI**.

POE BOTTARI is a community-made Windows companion for Path of Exile. It combines local PoB workflows with a Chrome extension that can translate supported build/economy sites on-device, send explicit item and build actions to the locally installed app, and fill user-requested build-aware filters on the official Trade page.

> POE BOTTARI is an unofficial community project. It is not affiliated with, endorsed by, or associated with Grinding Gear Games.

## Download

- Windows installer: [latest GitHub release](https://github.com/seeyouworks/POE-BOTTARI-Releases/releases/latest)
- Chrome extension: [Chrome Web Store](https://chromewebstore.google.com/detail/hdgedfadfonijbdlnonhhapamhnhebil)

The application is distributed as compiled binaries. Source code is not published in this repository.

## Community beta notice

The first public Windows build is prepared as a manually updated community beta. Until an Authenticode-signed production installer is published, Windows may show an **Unknown publisher** warning. Download only from this repository and compare the installer's SHA-256 value with the checksum published in the same release.

Automatic desktop updates are disabled. New versions must be downloaded manually from the latest release page.

## Requirements

- Windows 10 or 11, 64-bit
- Google Chrome 105 or later for the browser extension
- A user-installed Path of Building runtime is not required; the supported PoB runtimes are managed by POE BOTTARI

## Install

1. Download the installer and matching `.sha256` file from the latest release.
2. Verify the checksum if possible:

   ```powershell
   Get-FileHash .\POE-BOTTARI-Setup-community-0.1.13.exe -Algorithm SHA256
   ```

3. Run the installer. The community beta may trigger a Windows reputation warning because it is not yet Authenticode-signed.
4. Launch POE BOTTARI.
5. Install **POE BOTTARI Trade** from the Chrome Web Store.
6. Open the extension popup. Site translation is off by default; turn it on only when you want the displayed fixed PoE site list translated.

## Data and permissions

The extension has no advertising, analytics, arbitrary current-tab access, or external translation service. After the user turns Translation on, reviewed packaged dictionaries and, when available, Chrome's on-device Translator model process visible text only on the device. Explicit item, build, import, recommendation, and trade actions send only the disclosed action data—such as selected item text, equipment category, visible PoB code, or current supported action-page URL—to the locally installed POE BOTTARI app. A returned Trade filter plan is kept in Chrome session storage for at most ten minutes and fills only visible controls; the extension does not submit Search, whisper, or purchase.

See the full [Privacy Policy](PRIVACY.md).

## Support

Use [GitHub Issues](https://github.com/seeyouworks/POE-BOTTARI-Releases/issues) for reproducible bugs and release questions. Do not include account credentials, cookies, POESESSID values, OAuth tokens, private build files, or other secrets.
