# Privacy Policy

**App:** Simworld Air
**Version:** 1.0
**Effective date:** 2026-09-10
**Last updated:** 2026-09-10

---

## 1. Introduction

Simworld Air ("we", "our", "us") is committed to protecting your personal data. This Privacy Policy explains what data we collect, why we collect it, how we use and protect it, and what rights you have.

This policy applies to all users of the Simworld Air mobile application and complies with:

- **Morocco Law 09-08** on the Protection of Individuals with Regard to the Processing of Personal Data, and the regulations of the **Commission Nationale de contrôle de la Protection des Données à caractère Personnel (CNDP)**;
- The **EU General Data Protection Regulation (GDPR)** (Regulation 2016/679) for users located in the European Economic Area.

See also our [Terms and Conditions](./TERMS_AND_CONDITIONS.md), which this policy is incorporated into by reference.

---

## 2. Data We Collect

### 2.1 Account Data

| Data | Purpose |
|------|---------|
| **Name and email address**, from Google Sign-In, Sign in with Apple, or an email address you register directly. An anonymous device identifier instead, if you use the temporary guest option (Terms §4) | Creating and authenticating your account |
| **Password**, if you register with an email address. Handled entirely by Firebase Authentication — we never see or store it in any form | Authenticating your account |
| **Saved traveler information**, if you choose to save it: name, date of birth, gender, nationality, email, phone | Pre-filling the passenger form on future simulated bookings, and keeping it across reinstalls and devices |
| **Saved payment reference**, if you choose to save one: cardholder name, expiry date, last four digits, and a cosmetic card brand. **Never the full card number, never the security code (CVV)** | Pre-filling the simulated payment screen. Never used to charge anything — nothing in the App can be charged |
| **Simulated booking data** (route, fare, seat, price, and the passenger *name* attached to that booking) | Running the simulated booking → check-in → in-flight → landing flow, and recovering your booking history if you reinstall |
| **Miles balance, daily-claim streak and last-claim time, achievement state, and a bounded recent-activity log** | Tracking your simulated balance, your claim streak, and unlocked achievements |
| **Legal-document acceptance** (which Terms/Privacy Policy version, and when) | Proving consent was obtained, and re-prompting you if either document materially changes |

**On the traveler and payment fields specifically.** These are optional and are stored only if you explicitly save them from the Profile screen or from the "Save" action on the passenger or payment screen. Until you do, they stay on your device. Once saved, they are stored on our backend so they survive an uninstall or a switch of device, and they are deleted with your account. A booking record itself only ever carries the passenger *name* — date of birth, gender, nationality, email and phone are never attached to a booking record on our servers.

**Because this is a simulator, there is no reason to enter real identity or payment details anywhere in it.** We recommend you don't. Nothing in the App validates, verifies, or needs a real passport number, national ID, or card number, and none of those is ever requested.

### 2.2 Data We Do Not Collect

We do not collect your physical address or your precise location. The App has no user-submitted content, photos, or social features. We use **no analytics SDK, no crash-reporting SDK, and no advertising SDK** — there is no third-party telemetry in the App of any kind. We never receive or store a full payment card number, a card security code, a passport number, or a national identity number.

---

## 3. How We Use Your Data

| Processing activity | Legal basis |
|--------------------|-------------|
| Authenticating your account and running the simulated booking flow | **Contract performance** |
| Tracking your simulated balance and achievements | **Contract performance** |
| Storing traveler information and a payment reference you have explicitly chosen to save | **Contract performance** (you asked us to save it) |
| Running the daily claim, including the server-side calendar-day check | **Contract performance** |
| Preventing abuse of the balance/achievement system (rate limiting, anti-forgery checks) | **Legitimate interest** |
| Complying with legal obligations (e.g., data subject requests) | **Legal obligation** |

We do **not** sell your personal data to third parties.

---

## 4. Data Sharing

### 4.1 Service Providers

- **Google Firebase** (Google LLC) — authentication (Google Sign-In, email/password, or an anonymous identifier for the temporary guest option) and database (Firestore). Data may be processed in the United States or other regions where Google operates.
- **Apple Inc.** — Sign in with Apple, on iOS. If you use Apple's "Hide My Email" option, Apple relays messages to your real address without disclosing it to us.
- **Vercel** — hosts the backend functions that process balance, daily-claim, achievement, legal-acceptance and account-deletion operations.
- **Apple and Google as app stores** — process your purchase of the App. We receive only aggregate sales reporting that does not identify you.

We do not use any advertising network. We do not use any analytics or crash-reporting provider.

### 4.2 Legal Requirements

We may disclose your data if required to do so by law, court order, or a competent authority, including the CNDP (Morocco) or applicable EU supervisory authorities.

---

## 5. Data Retention

| Data | Retention period |
|------|----------------|
| Account, balance, daily-claim state, achievements | Until account deletion (Section 7) |
| Saved traveler information and saved payment reference | Until you clear or overwrite them, or until account deletion |
| Booking history (server-side) | A rolling buffer of your 15 most recent completed (landed) bookings; older entries are automatically evicted |
| Recent balance-activity log | The 10 most recent entries; older entries are automatically evicted |
| A web-based deletion request (Section 7.2) | Deleted once the request is processed, or after 90 days if unresolved |

---

## 6. Your Rights

### 6.1 All Users (Morocco Law 09-08)

- **Right of access, rectification, and deletion** of the personal data we hold about you.
- **Right to object** to processing based on legitimate interest.
- **Right to lodge a complaint** with the CNDP (www.cndp.ma).

### 6.2 EU/EEA Users (GDPR — Additional Rights)

- **Right to restriction** of processing in certain circumstances.
- **Right to data portability.**
- **Right to lodge a complaint** with your local EU supervisory authority.

To exercise any of these rights, contact us at **cs.ach.app@outlook.com**. We will respond within **30 days**.

---

## 7. Account and Data Deletion

You may delete your account and everything tied to it at any time, permanently:

### 7.1 In-App

Profile → Account → **Delete my account**, then confirm. Deletion is immediate — your account, Miles balance, achievements, and booking history are removed from our servers as soon as you confirm. Deletion also removes any saved traveler information and saved payment reference.

### 7.2 Without the App Installed

Visit [flight-booking-cyan-nu.vercel.app/delete-account](https://flight-booking-cyan-nu.vercel.app/delete-account) and submit the email address associated with your account. Because this page has no signed-in session, we can't verify ownership automatically — a person reviews and processes each request against the matching account, and deletion completes within **30 days**.

Device-local preferences not tied to your account (chosen theme, local mini-game scores) are not personal data linked to your deleted account and are unaffected by either path.

Some data may briefly persist in backups after deletion and is removed in the ordinary course of our backup-deletion cycle.

---

## 8. Data Security

- All data transmitted between the App and our backend is encrypted in transit (TLS).
- Firestore security rules restrict data access to the authenticated owner of that data only; every balance/achievement/deletion mutation is processed server-side inside an atomic transaction, never written directly by the client.
- API keys and service-account credentials are never embedded in the App — third-party API calls are proxied through our backend, which holds any secrets server-side.
- Passwords for email-registered accounts are handled entirely by Firebase Authentication and are never stored by us in any form. Full payment card numbers and security codes are never transmitted to or stored on our servers at all — our backend explicitly rejects any request containing a field resembling a security code.

No system is completely secure. If you believe your data has been compromised, contact us at **cs.ach.app@outlook.com**.

---

## 9. Advertising

**The App contains no advertising.** Versions before September 2026 offered optional rewarded-video advertisements served by Google AdMob; that feature and its SDK have been removed entirely. No advertising identifier is collected, no advertising network receives any data from the App, and no App Tracking Transparency prompt or consent management flow is required or shown. Any ad-view records previously held for duplicate-credit prevention were removed with the feature.

---

## 9bis. Payments

The App is sold as a paid app through the Apple App Store and Google Play. Your payment is processed entirely by the store, under the store's own privacy policy. We never receive your card details, billing address, or any other payment information, and we cannot identify you from the sales reporting we receive. The simulated payment screen inside the App is not connected to this in any way and never charges anything.

---

## 10. Children's Privacy

The App is not directed at children under 13. We do not knowingly collect personal data from children under 13. If you believe a child under 13 has used the App and provided us with personal data, contact us at **cs.ach.app@outlook.com** and we will delete it promptly.

---

## 11. International Data Transfers

Your data may be processed outside Morocco (e.g., in the United States via Google Firebase). When transferring data outside Morocco or the EEA, we rely on Standard Contractual Clauses (SCCs) and/or providers certified under recognized adequacy frameworks (e.g., EU-U.S. Data Privacy Framework).

---

## 12. Changes to This Policy

We may update this Privacy Policy at any time. When we do, we will update the "Last updated" date and version number at the top of this document and, for material changes, prompt you to review and accept the new version in-app.

---

## 13. Contact and Data Controller

**Data Controller:** Simworld Air

**Email:** cs.ach.app@outlook.com

For GDPR inquiries or formal data subject requests, please email us with the subject line **"Data Subject Request"**. We will respond within **30 days**.

---

*This Privacy Policy was last updated on 2026-09-10 (v1.0). See also our [Terms and Conditions](./TERMS_AND_CONDITIONS.md).*
