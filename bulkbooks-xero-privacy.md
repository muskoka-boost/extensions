# Privacy Policy — BulkBooks for Xero

_Last updated: 10 October 2026_

BulkBooks for Xero ("BulkBooks", "we") is a Chrome extension that helps bookkeepers download invoice and bill PDFs and file attachments from their Xero organisations. BulkBooks is an independent product and is **not affiliated with, endorsed by or sponsored by Xero Limited**.

**Publisher:** Muskoka Digital Boost, Ontario, Canada. Contact: hubscraper@gmail.com.

## Summary

- BulkBooks has **no servers** and never receives your Xero data. Documents go directly from Xero's API (`api.xero.com`) to your computer.
- BulkBooks only has **read-only** access to Xero. It can't create, change, void or delete anything in Xero.
- We don't sell, share or analyse your data, and we don't use it for advertising or to train AI/ML models.
- Subscription billing is handled by ExtensionPay and Stripe.

## What data the extension handles, and where it goes

| Data | Purpose | Where it is stored / sent |
|---|---|---|
| Xero OAuth access and refresh tokens | Call the Xero API on your behalf | Kept only in Chrome's in-memory session storage on your device. Cleared when Chrome closes or you click Disconnect. Sent only to Xero (`identity.xero.com`, `api.xero.com`). |
| List of your connected Xero organisations (names and IDs) | Let you choose which organisation to export | Shown in the extension. The last-selected organisation ID is saved locally in `chrome.storage.local`. |
| Invoices, bills, credit notes, bank-transaction metadata, PDFs and attachments | Build the ZIP file and CSV index you asked for | Processed in your browser's memory and saved as a ZIP to your Downloads folder. **Never sent to us or any third party.** |
| Export options (dates, checkboxes) and optional Xero Client ID override | Remember your preferences | `chrome.storage.local` on your device. |
| ExtensionPay licence key and subscription status | Check whether you have a paid subscription | Stored by the ExtPay library in Chrome storage. Sent to ExtensionPay (`extensionpay.com`). |
| Payment details (card, email) | Take payment | Entered on ExtensionPay/Stripe pages. We never see your card number. See ExtensionPay's privacy policy (linked from https://extensionpay.com) and Stripe's privacy policy (https://stripe.com/privacy). |

We don't collect analytics, telemetry, crash reports, browsing history or the contents of any website.

## Third parties

- **Xero Limited.** You sign in on Xero's own login page, and BulkBooks never sees your Xero password. Xero processes your data under its own terms and privacy notice: https://www.xero.com/legal/
- **ExtensionPay / Stripe.** Subscription management and payments only.

## Permissions

- `identity`: opens Xero's sign-in window (OAuth 2.0).
- `storage`: saves your preferences, session tokens and licence status locally.
- Host access to `api.xero.com` and `identity.xero.com`: needed to fetch your documents and sign-in tokens. No access to any other website.

## Retention and deletion

- Tokens are deleted when Chrome closes, or immediately when you click **Disconnect & revoke**, which also revokes BulkBooks' access at Xero.
- **Settings → Clear all local BulkBooks data** removes preferences and tokens. Uninstalling the extension removes all extension storage.
- ZIP files you download are yours, on your computer. Keep them secure, because they contain financial documents.
- You can also remove BulkBooks' access at any time from Xero (Settings → Connected apps).
- To delete your ExtensionPay customer record, contact us at hubscraper@gmail.com.

## Chrome Web Store Limited Use

BulkBooks' use of information received from Google APIs and from your browser follows the Chrome Web Store User Data Policy, including the Limited Use requirements. We use data only to provide the single purpose of the extension, don't transfer it to third parties except as described above, don't use it for advertising, and don't allow humans to read it.

## Children

BulkBooks is a professional tool and isn't directed at children under 16.

## Changes

We'll update this page and the "Last updated" date if our practices change. Material changes will be announced in the extension's release notes.

## Contact

hubscraper@gmail.com
