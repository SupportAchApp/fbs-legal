# Privacy Policy

**App:** Simworld Air
**Version:** 2.0
**Effective date:** 2026-09-02
**Last updated:** 2026-09-02

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
| **Name and email address** (via Google Sign-In), or an anonymous device identifier if you use the temporary guest option (Terms §4) | Creating and authenticating your account |
| **Simulated booking data** (route, fare, seat, price, a passenger *name* you enter in the booking flow) | Running the simulated booking → check-in → in-flight → landing flow, and recovering your booking history if you reinstall the App |
| **Miles balance, achievement state, and a bounded recent-activity log** | Tracking your simulated balance and unlocked achievements |
| **Ad-view records** | Preventing duplicate rewarded-ad credit for the same ad view |
| **Legal-document acceptance** (which Terms/Privacy Policy version, and when) | Proving consent was obtained, and re-prompting you if either document materially changes |

Passenger details beyond name (date of birth, gender, nationality, email, phone) that you optionally enter are kept **only on your device** and are never sent to our backend.

### 2.2 Data We Do Not Collect

We do not collect your physical address or precise location. The App has no user-submitted content, photos, or social features.

---

## 3. How We Use Your Data

| Processing activity | Legal basis |
|--------------------|-------------|
| Authenticating your account and running the simulated booking flow | **Contract performance** |
| Tracking your simulated balance and achievements | **Contract performance** |
| Preventing abuse of the balance/achievement system (rate limiting, anti-forgery checks) | **Legitimate interest** |
| Complying with legal obligations (e.g., data subject requests) | **Legal obligation** |

We do **not** sell your personal data to third parties.

---

## 4. Data Sharing

### 4.1 Service Providers

- **Google Firebase** (Google LLC) — authentication (Google Sign-In, or an anonymous identifier for the temporary guest option) and database (Firestore). Data may be processed in the United States or other regions where Google operates.
- **Google AdMob** (Google LLC) — serves the optional rewarded-video ads; verifies ad completions server-to-server. Ads are currently non-personalized (Terms §6) — no advertising-identifier-based tracking is used.
- **Vercel** — hosts the backend functions that process balance/achievement updates, legal-document acceptance, and account deletion.

### 4.2 Legal Requirements

We may disclose your data if required to do so by law, court order, or a competent authority, including the CNDP (Morocco) or applicable EU supervisory authorities.

---

## 5. Data Retention

| Data | Retention period |
|------|----------------|
| Account, balance, achievements | Until account deletion (Section 7) |
| Booking history (server-side) | Kept as a rolling buffer of your 15 most recent completed (landed) bookings; older entries are automatically evicted |
| Recent balance-activity log | The 10 most recent entries; older entries are automatically evicted |
| Ad-view dedup records | Until account deletion |
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

Profile → Account → **Delete my account**, then confirm. Deletion is immediate — your account, Miles balance, achievements, and booking history are removed from our servers as soon as you confirm.

### 7.2 Without the App Installed

Visit [flight-booking-cyan-nu.vercel.app/delete-account](https://flight-booking-cyan-nu.vercel.app/delete-account) and submit the email address associated with your account. Because this page has no signed-in session, we can't verify ownership automatically — a person reviews and processes each request against the matching account, and deletion completes within **30 days**.

Device-local preferences not tied to your account (chosen theme, local mini-game scores) are not personal data linked to your deleted account and are unaffected by either path.

Some data may briefly persist in backups after deletion and is removed in the ordinary course of our backup-deletion cycle.

---

## 8. Data Security

- All data transmitted between the App and our backend is encrypted in transit (TLS).
- Firestore security rules restrict data access to the authenticated owner of that data only; every balance/achievement/deletion mutation is processed server-side inside an atomic transaction, never written directly by the client.
- API keys and service-account credentials are never embedded in the App — third-party API calls are proxied through our backend, which holds any secrets server-side.

No system is completely secure. If you believe your data has been compromised, contact us at **cs.ach.app@outlook.com**.

---

## 9. Advertising

The App may show optional rewarded-video ads via Google AdMob, currently using Google's test ad units and non-personalized targeting only (no advertising identifier is used, so no Apple ATT prompt or EU/UK consent-management flow is currently shown). Ads are not targeted at users under 13. See Google's own privacy policy for how AdMob processes data on its side.

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

*This Privacy Policy was last updated on 2026-09-02 (v2.0). See also our [Terms and Conditions](./TERMS_AND_CONDITIONS.md).*
