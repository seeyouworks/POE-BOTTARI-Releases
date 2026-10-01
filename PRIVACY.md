# POE BOTTARI Trade Privacy Policy

Effective date: September 30, 2026

POE BOTTARI Trade provides Path of Exile site translation, saved searches and bookmarks, and local POE BOTTARI app integration. The developer does not collect extension usage or page content on a developer-operated server and does not sell user data.

## Information used by the extension

- **Supported pages:** page text, item and build information, search filters, and the page URL are processed for translation, game identification, requested searches/bookmarks, and the selected feature. Saved public character bookmarks can include account and character names from the page URL.
- **Local app actions:** item, craft-import, build-reference, and equipment-recommendation controls pass the relevant item text, visible PoB code, selected equipment category, game/language, and supported page URL to the POE BOTTARI app on the same computer. The app must already be running.
- **Copy and import:** Copy buttons write bookmark or filter share codes to the clipboard. Import uses text you paste into the import field. The extension does not read the system clipboard in the background.

These data are used for the extension's features, rather than advertising or behavioral profiling.

## Local storage and deletion

Language preferences, enabled-site settings, saved Trade filters, poe.ninja bookmarks, and panel settings stay in your browser until you change/delete them, clear extension storage, or remove the extension. Optional troubleshooting records contain bounded status/error metadata, rather than raw item text or PoB codes.

A pending app-generated filter plan is held in browser session storage for at most ten minutes and expires or is removed when completed. It contains filter labels and numeric bounds, not a raw PoB build. Item text and PoB codes used for app actions are not saved by the extension as a history.

## Network requests and permissions

Translation uses packaged dictionaries. Eligible Wiki and poe.how prose can also use Chrome's on-device Translator API; Chrome manages any language-model download. Page text is not sent to the developer or an external translation service.

For a requested Trade item action, the extension may retrieve missing item text from the same official trade service without browser credentials. Opening site links, bookmarks, or supported Trade result URLs makes normal browser requests. The site can receive connection information such as your IP address and applies its own privacy policy.

The extension uses `storage` for local feature data, `scripting` for supported-page features, and `nativeMessaging` for the local app. Translation is off by default. Enabling it requests eleven declared optional origins represented by nine site profiles; turning it off removes those permissions. The extension has no cookies, browsing-history API, or arbitrary-tab access permission and does not run remotely hosted code.

## Your choices

You can turn translation off, remove site permissions, edit/delete saved entries, or uninstall the extension. App actions use their corresponding controls. The extension does not automate whispers or purchases.

## Chrome Web Store Limited Use

The use of information received from Chrome APIs adheres to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/limited-use), including the Limited Use requirements.

This policy will be updated when data handling changes. For questions, use the [POE BOTTARI Releases issue tracker](https://github.com/seeyouworks/POE-BOTTARI-Releases/issues).
