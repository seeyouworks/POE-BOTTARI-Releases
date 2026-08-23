# POE BOTTARI Trade Privacy Policy

Effective date: August 23, 2026

This policy describes how the **POE BOTTARI Trade** Chrome extension handles data. The extension is a local browser companion for Path of Exile build, economy, and trade workflows.

## Data handled by the extension

### Supported-site translation

Site translation is off by default. When the user turns on the displayed Translation control and grants the corresponding optional permissions, the extension uses the current supported-site address to select the correct translation profile, reads visible page text needed for translation, and replaces matching interface and game terms in the page. The extension requests only the eleven exact optional origins represented by the nine fixed Path of Exile site profiles shown in the popup. It has no arbitrary current-tab or `<all_urls>` access.

Reviewed interface, game-term, and numeric dictionaries are packaged with the extension and run on the user's device. On eligible long-form supported pages, Chrome 138 or later may use Chrome's on-device Translator API. Chrome may download and manage the selected language model; the extension does not send page text to the developer or an external translation service and does not download or execute remote JavaScript, WebAssembly, or other code.

The extension stores the selected translation language, the supported-sites master on/off state, and bounded permission-completion state in `chrome.storage.local`. A user-requested Trade filter plan returned by the local app is kept in `chrome.storage.session` for at most ten minutes so a service-worker restart does not lose the pending action. The plan contains Trade filter labels and numeric bounds, not the user's raw Path of Building build, and is removed after completion or expiry.

### Explicit local-app actions

The following data is handled only after the user invokes the corresponding action:

- **Trade-page PoB actions:** the selected trade item's text, current trade-page URL, selected action, and PoE game identifier.
- **Build-aware Trade recommendation:** the selected equipment category plus the PoE game and locale inferred from the current official Trade page. The local app uses its current managed Path of Building state and returns a bounded filter plan. The extension fills only visible Trade controls and does not submit Search, whisper, or purchase. A supported exact-count flow may open the official Trade result URL returned by the local app.
- **Craft item import:** item text pasted into the supported PoE1 item-import field. The local app returns a canonical English representation for the same visible field; the user's source text is left unchanged if conversion fails.
- **Build reference:** the visible PoB import code beside the clicked action and the current supported build-page URL.

This data is sent through Chrome Native Messaging only to the POE BOTTARI application installed on the same computer. It is used only to perform the requested local item conversion, managed Path of Building or Trade-page action, recommendation and filter planning, or reference-build opening. The extension cannot start the desktop application or an arbitrary executable.

When an item does not already expose its clipboard text in the page, the extension may request the item's JSON representation from the same official Path of Exile trade origin. That request omits browser credentials.

## Data not collected

The developer does not receive or retain visible page text, supported-site addresses, selected equipment categories, selected or pasted item text, PoB import codes, translation settings, returned Trade filter plans, or local-app action data handled by the extension. The extension does not persist pasted item text, PoB import codes, or raw Path of Building builds.

The extension does not:

- use analytics, advertising, tracking pixels, or behavioral profiling;
- sell or transfer user data;
- read or store browser cookies, POESESSID values, passwords, OAuth tokens, payment information, or a browsing-history record;
- send page content to an external translation service;
- allow the developer or another human to read data handled locally by the extension.

## Permission purposes

- `nativeMessaging`: send only an explicitly requested item, build, import, recommendation, or trade action to the locally installed POE BOTTARI application and check its local connection state.
- `scripting`: register and run packaged translation and supported-page action scripts only on sites the user enables.
- `storage`: save the selected language, the supported-sites master on/off state, the bounded state needed to complete a permission choice after Chrome closes the popup, and a pending returned Trade filter plan in session storage for at most ten minutes.
- Path of Exile trade-page access: add explicit PoB and filter-planning controls, process the selected item or equipment category only when the user invokes an action, and fill only visible Trade controls.
- Optional site access: translate visible page text and expose supported Craft/build actions only after the user turns on **Translation** and grants the fixed group of exact supported origins. Turning Translation off removes the same origins.

## Sharing and third parties

The extension does not send handled user data to the developer, advertising networks, data brokers, analytics providers, or an external translation service. A Chrome-managed on-device language-model download does not include the page text being translated. Normal browser requests remain subject to the privacy practices of the website the user is visiting. The same-origin official trade-item request described above is made only to provide the user-requested trade action and omits browser credentials.

## Retention and deletion

The developer has no server-side copy of extension data to retain or delete. Item text and PoB import codes used by local-app actions are not stored by the extension after the request. A pending returned Trade filter plan remains only in Chrome session storage for at most ten minutes and is removed after completion or expiry. Users can turn off Translation in the extension popup, remove site permissions in Chrome, clear the extension's storage, or uninstall the extension.

## Chrome Web Store Limited Use

The use of information received from Chrome APIs adheres to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq), including the Limited Use requirements. Data is handled only to provide the extension's disclosed user-facing features.

## Changes

If the extension's data practices change, this policy and the in-product disclosure will be updated before the changed handling is introduced.

## Contact

For privacy or support questions, open an issue in the [POE BOTTARI Releases repository](https://github.com/seeyouworks/POE-BOTTARI-Releases/issues). Do not post credentials, private build data, or other secrets.
