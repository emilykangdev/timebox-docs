---
title: Privacy Policy
metaTitle: Privacy Policy — TimeBox
description: How TimeBox handles your calendar data and personal information.
lastUpdated: April 28, 2026
callout: TimeBox is local-first. Your calendar data and edit history are stored on your device, not on our servers. We only collect what we need to let you sign in and use the product.
---

This Privacy Policy explains what information TimeBox ("we", "us") collects when you use the TimeBox app and website ("the Service"), how we use it, and the choices you have. By using TimeBox, you agree to the practices described here.

## 1. Information we collect

### Calendar data

When you connect your Google Calendar, TimeBox reads your calendar events so the app can show them, track changes, and let you undo edits. This data is stored **locally on your device**. We do not upload, copy, or retain your calendar events on our servers.

### Google account information

To authenticate with Google Calendar, we use Google's OAuth flow. Google shares a limited access token with TimeBox. We do not receive or store your Google password. You can revoke access at any time from your [Google account permissions page](https://myaccount.google.com/permissions).

### Email address (optional)

If you join our waitlist or contact us, we collect the email address you provide. We use it only to respond to you or to notify you when TimeBox is ready.

### AI prompts and responses

When you use AI features (e.g., natural-language event creation, reasoning about your time), TimeBox sends the relevant prompt to **OpenRouter**, which routes it to the underlying language model provider. By default, we also save the prompt and response to our Supabase database so we can debug, improve quality, and learn how the AI is being used. You can **turn off this analytics** from the app's settings — when off, prompts and responses are not stored on our servers, only used in-memory to return the answer to you.

### Basic usage information

Like most websites, this site may record standard request information (IP address, browser, referring page) in short-lived server logs for security and debugging. We do not use third-party advertising trackers.

## 2. How we use Google user data

TimeBox's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

- We only access the calendar scopes needed to read and write your events.
- Your calendar data is processed on your device for the features you use (viewing events, versioning, diffs, restore).
- We do not sell your data, transfer it to third parties, or use it for advertising.
- We do not use your calendar data to train machine learning models.

## 3. Where your data lives

Because TimeBox is local-first:

- Your calendar snapshots and edit history are stored in a folder on your computer.
- You can inspect, back up, or delete that folder at any time.
- Uninstalling the app does not automatically delete the local history folder — you can remove it manually.

If we later introduce optional cloud sync, it will be clearly labeled as opt-in and documented separately.

## 4. Cookies and analytics

The marketing website may use a minimal, privacy-respecting analytics tool to understand aggregate traffic (e.g., page views). We do not use advertising cookies or cross-site trackers. We will update this section if our tooling changes.

## 5. Sharing with third parties

We do not sell your personal information. We share data only with the service providers below, and only to the extent needed for them to provide their service:

- **Lemon Squeezy** — payments, subscription management, and license key issuance (Merchant of Record).
- **Supabase** — hosted database where we store your email, license key, and (unless you turn off AI analytics) your AI prompts and responses.
- **OpenRouter** — AI inference router. Your AI prompts pass through OpenRouter to the model provider that answers them. We do not send your calendar contents beyond what's needed to fulfill the request you made.
- **Resend** — transactional email delivery (your license key, account emails).

## 6. Security

We take reasonable steps to protect information we hold, including using HTTPS for our website and Google's official OAuth flow for authentication. No method of storage or transmission is 100% secure; if you have security concerns, please contact us.

## 7. Your choices

- **Disconnect Google Calendar:** Revoke access from [your Google permissions page](https://myaccount.google.com/permissions).
- **Delete local history:** Remove the TimeBox data folder from your device.
- **Turn off AI analytics:** In the app's settings, disable AI analytics so your prompts and responses are not saved to our database. The AI still works — we just don't keep a copy.
- **Unsubscribe:** Use the link in any email, or reply asking to be removed.
- **Access or delete your info:** Email us (below) to request a copy of, or deletion of, any data we hold.

## 8. Children

TimeBox is not directed to children under 13 and we do not knowingly collect personal information from them.

## 9. Changes to this policy

We may update this Privacy Policy as the product evolves. When we do, we'll update the "Last updated" date above. Material changes will be announced on the website.

## 10. Contact

Questions, requests, or concerns? Email [time-box@emilykang.dev](mailto:time-box@emilykang.dev).
