# Privacy Policy — TranscriptVault for Intercom

_Last updated: October 10, 2026_

TranscriptVault for Intercom ("the extension", "we") is a Chrome extension that exports your Intercom conversation transcripts to files on your computer. It is an independent product and is **not affiliated with, endorsed by, or sponsored by Intercom**.

## Summary
- We do not operate servers that receive your data. We do not collect, store, sell or share your Intercom data.
- Your Intercom access token and your conversations stay in your browser and on your computer.
- The only third party involved besides Intercom is ExtensionPay (with Stripe), which handles the paid subscription.

## What the extension handles and where it goes

### 1. Your Intercom access token
- You paste it into the extension's Settings page.
- If you tick "Remember token on this device", it is stored in `chrome.storage.local` on your computer; otherwise in `chrome.storage.session` and erased when the browser closes.
- It is sent **only** to Intercom's API (`api.intercom.io`, or `api.eu.intercom.io` / `api.au.intercom.io` if you choose that region) in the `Authorization` header, over HTTPS.
- You can delete it at any time with "Forget token", by removing the extension, or by revoking/deleting the app in your Intercom Developer Hub.

### 2. Your Intercom conversation data
- Conversation content (messages, internal notes, names and email addresses of customers and teammates, tags, assignees, timestamps, attachment links) is downloaded from Intercom's API directly into the extension page in your browser.
- It is processed in memory and saved as a ZIP file through your browser's normal download mechanism.
- It is **never** transmitted to us or to any third party. The extension does not include analytics, telemetry, crash reporting or advertising code.

### 3. Settings
- Region, API version, throttle and ZIP part-size preferences are stored in `chrome.storage.local`.

### 4. Subscription (ExtensionPay / Stripe)
- Paid plans are processed by [ExtensionPay](https://extensionpay.com) and [Stripe](https://stripe.com). When you upgrade, a payment page hosted by ExtensionPay/Stripe opens; your payment details go to them, never to the extension.
- The bundled ExtensionPay library contacts `extensionpay.com` to create an anonymous installation key and to check whether your subscription is active. ExtensionPay may store the email address you provide at checkout and your subscription status. See ExtensionPay's and Stripe's privacy policies.
- No Intercom data is ever sent to ExtensionPay or Stripe.

## Permissions
- `storage` — keep settings, the token (if you choose) and licence status locally.
- `https://api.intercom.io/*` (and, only if you select them, the EU/AU API hosts) — read your conversations through Intercom's official API.

## Your responsibilities
Exported files may contain personal data about your customers and teammates. Once saved to your computer, you are the controller of those files; store, share and delete them in line with your organisation's policies and applicable law (e.g., GDPR, CCPA).

## Children
The extension is a business tool and is not directed at children under 13 (or 16 where applicable).

## Changes
If this policy changes, we will update the "Last updated" date above and, for material changes, note it in the extension's release notes.

## Contact
Questions or requests: **hubscraper@gmail.com**
