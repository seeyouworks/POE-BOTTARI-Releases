# POE BOTTARI Trade Privacy Policy

Effective date: August 5, 2026

This policy describes how the **POE BOTTARI Trade** Chrome extension handles data. The extension is a local browser companion for Path of Exile build, economy, and trade workflows.

## Data handled by the extension

### Supported-site translation

Site translation is off by default. When the user enables one or all supported sites and grants the corresponding optional permissions, the extension uses the current supported-site address to select the correct translation profile, reads visible page text needed for translation, and replaces matching interface and game terms in the page. Translation uses data packaged with the extension and runs on the user's device. Page text and addresses used for translation are not sent to the developer or an external translation service.

The extension stores the selected translation language and per-site on/off settings in `chrome.storage.local`.

### Explicit local-app actions

The following data is handled only after the user invokes the corresponding action:

- **Trade-page PoB actions:** the selected trade item's text, current trade-page URL, selected action, and PoE game identifier.
- **Build-aware trade planning:** item text pasted into the extension popup and the selected UI locale. A jewel recommendation does not read page content.
- **Craft item import:** item text pasted into the supported PoE1 item-import field. The local app returns a canonical English representation for the same visible field; the user's source text is left unchanged if conversion fails.
- **Build reference:** the visible PoB import code beside the clicked action and the current supported build-page URL.

This data is sent through Chrome Native Messaging only to the POE BOTTARI application installed on the same computer. It is used only to perform the requested local item conversion, build/trade planning, managed Path of Building action, or reference-build opening. The extension cannot start the desktop application or an arbitrary executable.

When an item does not already expose its clipboard text in the page, the extension may request the item's JSON representation from the same official Path of Exile trade origin. That request omits browser credentials.

## Data not collected

The developer does not receive or retain visible page text, supported-site addresses, selected or pasted item text, PoB import codes, translation settings, or local-app action data handled by the extension. The extension does not persist pasted item text or PoB import codes.

The extension does not:

- use analytics, advertising, tracking pixels, or behavioral profiling;
- sell or transfer user data;
- read or store browser cookies, POESESSID values, passwords, OAuth tokens, payment information, or a browsing-history record;
- send page content to an external translation service;
- allow the developer or another human to read data handled locally by the extension.

## Permission purposes

- `nativeMessaging`: send only an explicitly requested item, build, import, or trade action to the locally installed POE BOTTARI application and check its local connection state.
- `scripting`: register and run packaged translation and supported-page action scripts only on sites the user enables.
- `storage`: save the selected language, per-site translation settings, and the bounded state needed to complete a permission choice after Chrome closes the popup.
- Path of Exile trade-page access: add explicit PoB controls and process the selected item when the user invokes an action.
- Optional site access: translate visible page text and expose the supported Craft/build actions only after the user enables and grants access to the exact site, individually or through the **All sites** control.

## Sharing and third parties

The extension does not send handled user data to the developer, advertising networks, data brokers, analytics providers, or an external translation service. Normal browser requests remain subject to the privacy practices of the website the user is visiting. The same-origin official trade-item request described above is made only to provide the user-requested trade action and omits browser credentials.

## Retention and deletion

The developer has no server-side copy of extension data to retain or delete. Item text and PoB import codes used by local-app actions are not stored by the extension after the request. Users can turn off individual sites or all sites in the extension popup, remove a site's permission in Chrome, clear the extension's local storage, or uninstall the extension.

## Chrome Web Store Limited Use

The use of information received from Chrome APIs adheres to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq), including the Limited Use requirements. Data is handled only to provide the extension's disclosed user-facing features.

## Changes

If the extension's data practices change, this policy and the in-product disclosure will be updated before the changed handling is introduced.

## Contact

For privacy or support questions, open an issue in the [POE BOTTARI Releases repository](https://github.com/seeyouworks/POE-BOTTARI-Releases/issues). Do not post credentials, private build data, or other secrets.
