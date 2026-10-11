# Privacy Policy: ActivityVault for HubSpot

_Last updated: October 10, 2026_

ActivityVault for HubSpot ("ActivityVault", "the extension", "we") is a Chrome extension that exports activity records (notes, calls, emails, meetings and tasks) from your own HubSpot account to files on your computer. This policy explains what data the extension handles and where that data goes.

ActivityVault is an independent product and is not affiliated with, endorsed by, or sponsored by HubSpot, Inc.

## Summary

- Your HubSpot data is processed **only inside your browser**. We do not operate any server that receives your HubSpot data.
- Your HubSpot key is stored **only in your browser** and is sent **only to HubSpot** (`api.hubapi.com`).
- The only other service the extension contacts is **ExtensionPay** (`extensionpay.com`), which checks whether you have a paid subscription.
- We do not sell, rent, or share your data. We do not use analytics, advertising, or tracking.

## Data the extension handles

### 1. Your HubSpot Service Key (or legacy private-app access token)
- **What:** the key you create in your HubSpot account and paste into the Settings page.
- **Where it is stored:** `chrome.storage.local` in your Chrome profile on your device. It is not synced by the extension.
- **Where it is sent:** only to `https://api.hubapi.com`, in the `Authorization` header of HubSpot API requests.
- **How to delete it:** click **Remove key** in Settings, uninstall the extension, or delete or rotate the key in HubSpot (Development → Keys → Service keys).

### 2. HubSpot CRM data you choose to export
- **What:** the records you choose (contact, company or deal names and IDs, list membership IDs) and their associated activities (note text, call details, email subject/body/sender/recipients, meeting and task details, owner names).
- **How it is used:** it is downloaded from HubSpot's API into the extension's page in your browser, converted to CSV/Markdown/JSON, packed into a ZIP file, and saved through your browser's normal download mechanism.
- **Retention:** the extension does not keep a copy. The data exists in memory only while the export runs. The ZIP file you download is yours, and you control it.
- **Never sent to us** or to any third party other than HubSpot itself (where the data already lives).

### 3. Preferences
Your selected activity types and formats are stored in `chrome.storage.local` so they are remembered next time.

### 4. Subscription status (ExtensionPay)
To offer the paid plan, the extension includes the open-source ExtPay.js library from ExtensionPay (https://extensionpay.com). ExtPay:
- creates a random license key for your installation and stores it in `chrome.storage.sync`;
- contacts `extensionpay.com` to check whether that key has an active subscription;
- opens ExtensionPay/Stripe pages when you click **Upgrade** or **Log in**, where you may enter your email and payment details **on their sites, not in the extension**.

The extension also caches your paid/unpaid status (true/false and a timestamp) in `chrome.storage.local` so it keeps working briefly if ExtensionPay is unreachable.

ExtensionPay's and Stripe's handling of your email and payment information is governed by their own privacy policies:
- ExtensionPay: see the privacy policy linked from https://extensionpay.com
- Stripe: https://stripe.com/privacy

We (the developer) can see the email address and subscription status of paying users in the ExtensionPay dashboard. We use it only to provide the subscription and support, and never for marketing without your consent.

## Data we do NOT collect
We do not collect browsing history, website content, location, analytics, telemetry, crash reports, or advertising identifiers. The extension has no content scripts and does not read the web pages you visit.

## Permissions
- `storage`: to store your key, preferences and cached subscription status locally.
- Host access to `https://api.hubapi.com/*`: to call HubSpot's official API with your key.

## Limited Use
The use of information received from HubSpot's APIs follows the Chrome Web Store User Data Policy, including its Limited Use requirements. Data is used only to provide the export feature that you request.

## Security
Requests to HubSpot and ExtensionPay use HTTPS. We recommend creating a dedicated **read-only** Service Key for ActivityVault and rotating it periodically. Anyone with access to your Chrome profile could read the stored key, so protect your device and Chrome profile.

## Children
ActivityVault is a business tool and is not directed at children under 13.

## Changes
If this policy changes, we will update the "Last updated" date and, for material changes, note them in the extension's Chrome Web Store listing.

## Contact
Questions or deletion requests: **hubscraper@gmail.com**
