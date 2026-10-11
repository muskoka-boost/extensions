# TicketVault for Zendesk: Privacy Policy

_Last updated: October 10, 2026_

TicketVault for Zendesk ("TicketVault", "the extension", "we") is a Chrome extension that exports Zendesk Support tickets to files on your computer. This policy explains what data the extension handles and where that data goes.

**Summary: your ticket data never leaves your browser except as files that you download. We don't run servers that receive your Zendesk data, and we don't use analytics or tracking.**

## 1. Data the extension processes

When you start an export, TicketVault requests the following from **your own Zendesk account** (`https://<your-subdomain>.zendesk.com/api/v2/...`), using the Zendesk session you're already signed in with:

- ticket fields (ID, subject, status, priority, type, tags, dates, requester, assignee, group, organization, custom field values);
- ticket comments (public replies and, if you choose, internal notes), including author, timestamp, body, and attachment metadata (file name, type, size, link);
- basic profile data (name, email, role) for the users involved in those tickets, and for you, so it can confirm you're signed in as an agent.

Zendesk enforces your role's permissions, so TicketVault can only read what you can already see in Zendesk. All requests are read-only (HTTP GET).

This data is processed **in memory in your browser tab** and written into a ZIP file that you save to your device. Data from your most recent export stays in the tab's memory so that "Print all to PDF" works. It's discarded when you close or reload the tab. TicketVault doesn't write ticket data to extension storage, and it doesn't send ticket data anywhere else.

Attachment files aren't downloaded. Exports contain links to the attachments in Zendesk, and those links still require access to your Zendesk account.

## 2. Data stored by the extension

- **Settings** (selected formats, internal-notes default, request-rate limit, body format, launcher visibility), stored in `chrome.storage.sync`. If Chrome Sync is on, Google syncs these settings between your browsers.
- **Licence key**: a random identifier created by ExtPay.js and stored in `chrome.storage`. It's used to check your subscription status.

## 3. Payments and licence checks (ExtensionPay)

Subscriptions are handled by **ExtensionPay** (https://extensionpay.com), which uses **Stripe** to process payments. When you open the upgrade page, enter your payment details, or when the extension checks whether you have a paid subscription, your browser communicates directly with ExtensionPay. ExtensionPay receives your licence key and, if you subscribe, the email address and payment details you enter on their or Stripe's pages. We receive your subscription status and email from ExtensionPay so that we can provide support. We never see your full card details.

See ExtensionPay's privacy policy at https://extensionpay.com/privacy and Stripe's at https://stripe.com/privacy.

**No ticket data is ever sent to ExtensionPay, Stripe, or us.**

## 4. What we do not do

- We don't sell, rent, or share your data.
- We don't use your data for advertising, profiling, or creditworthiness decisions.
- We don't run analytics, telemetry, or crash reporting.
- We don't load remote code.
- We don't read your Zendesk password, cookies, or API tokens.

## 5. Your responsibilities

Exported files may contain personal data about your customers and colleagues. Once downloaded, they're under your control. Store, share, and delete them in line with your organization's policies and any applicable data-protection law (e.g. GDPR/CCPA). Make sure your organization permits exporting ticket data before you use the extension.

## 6. Data retention and deletion

We hold no ticket data, so there's nothing for us to delete. To remove local extension data, uninstall the extension, which clears its storage. To delete subscription records held by ExtensionPay, contact us at the address below and we'll pass on the request, or contact ExtensionPay directly.

## 7. Children

TicketVault is a business tool and isn't directed at children under 16.

## 8. Changes

If we change this policy, we'll update the date above and, for material changes, note them in the extension's Chrome Web Store listing.

## 9. Contact

Questions or requests: **hubscraper@gmail.com**

TicketVault is an independent product and is not affiliated with, endorsed by, or sponsored by Zendesk, Inc.
