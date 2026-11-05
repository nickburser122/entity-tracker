# entity-tracker

Contracted-entity statement tracker (بيان جهات متعاقدة), Arabic and right-to-left. It imports xlsx, xls and csv files and JSON backups.

## Storage

- Data is stored in Firestore under an anonymous Firebase sign-in and cached in `localStorage`.
- Google Sheets sync is optional and starts a Google OAuth request when used.

## Limits

- Sheets sync needs a connection and a Google account with access to the sheet.

## Network and install

Calls Firebase for storage, and Google Sheets when sync is used; nothing else leaves the browser. Loads the Firebase SDK, Google Identity Services, SheetJS and Google Fonts from CDNs. Not installable; no service worker.
