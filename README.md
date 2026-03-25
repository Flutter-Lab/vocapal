# VocaPal Legal/Support Pages (GitHub Pages)

This repository hosts VocaPal's public legal/support pages used in App Store metadata:

- `index.html` -> Support page
- `privacy.html` -> Privacy Policy page

## Current app context (important)

The policy content is aligned with current VocaPal behavior, including:

- Microphone/speech recognition usage for listening mode
- Third-party dictionary/translation providers
- Firebase usage (anonymous analytics, shared dictionary cache, feedback storage)
- In-app feedback collection (text, type, app version, timestamp)
- Optional local backups (export/restore stays on-device)
- Optional daily reminder notifications and user control settings

## Recommended deployment

Use a separate public repository, for example `vocapal-legal`.

1. Create a public GitHub repository.
2. Copy `index.html` and `privacy.html` into the repo root.
3. Open **Settings -> Pages**.
4. Set source to **Deploy from a branch**.
5. Select `main` and folder `/ (root)`.
6. Save and wait for Pages to publish.

Published URLs:

- Support: `https://flutter-lab.github.io/vocapal_legal/`
- Privacy: `https://flutter-lab.github.io/vocapal_legal/privacy.html`

## Release checklist (every app update)

Before submitting a new app version:

1. Re-check `privacy.html` for new permissions, new data flows, or new third-party services.
2. If policy text changes, update the **Effective date**.
3. Push legal page updates and verify both URLs load correctly.
4. Update App Store listing metadata to use the live support/privacy URLs.

## App Store metadata update

After publishing legal pages, update the URLs in your app project metadata file:

- `VocaPal/app_store_metadata_vocapal.md`

## Notes

- Keep this repo public so App Review can access the pages.
- Keep policy language consistent with actual in-app behavior to avoid review issues.
