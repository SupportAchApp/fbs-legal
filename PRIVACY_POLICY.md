# Privacy Policy

**App:** Simworld Air
**Version:** 1.1
**Effective date:** 2026-09-19
**Last updated:** 2026-09-19

---

## 1. Who this policy covers

This policy explains how personal data is handled when you use the Simworld Air
mobile application (the **App**), its account-deletion page, and its support
channel. Simworld Air is a flight-booking simulator: it does not sell real
flights and never processes a real in-app payment.

The controller is **Ayoub El Hazzaz**, the sole developer and legal
seller/provider for Simworld Air. The controller can be contacted at
**cs.ach.app@outlook.com**.

This policy is intended to address Morocco Law 09-08 and CNDP requirements, the
EU GDPR and UK GDPR where applicable, and comparable privacy rights in other
places where the App is available. Local mandatory rights continue to apply
even if they are not listed individually below.

## 2. Data we process

### 2.1 Core account and simulation data

| Data | Why it is processed |
|---|---|
| Name, email and Firebase account identifier supplied through Google, Apple or email/password; an anonymous account identifier for the debug/guest option where offered | Create, authenticate and secure an account |
| Optional saved traveler profile: name, date of birth, gender, nationality, email and phone | Pre-fill later simulated passenger forms |
| Optional saved payment reference: cardholder name, expiry, last four digits and cosmetic card brand | Pre-fill the simulated payment form |
| Simulated booking data: itinerary, fare, extras, seat, price and passenger name | Run booking, check-in, in-flight, landing, achievements and history recovery |
| Miles balance, claim/ad-reward state, achievement and bounded game/recent-activity state | Operate the virtual economy and prevent duplicate rewards |
| Legal-document version and acceptance time | Keep a record of the terms shown and require review after material changes |

The full card number and CVV never leave the device and are never stored. A
server booking contains only the passenger name, not the saved traveler's date
of birth, gender, nationality, email or phone. Because the App is a simulator,
you should use fictional details and must not enter passport, national-ID or
real payment-card data.

### 2.2 Optional analytics and diagnostics

Firebase Analytics and Firebase Crashlytics are included but **collection is
off by default at the native platform layer**. The App asks separately whether
you want to share:

- anonymous usage analytics, such as a coarse feature name, cabin/fare
  category, result count or success/failure category; and
- redacted crash and diagnostic reports, such as stack traces, app version,
  platform and a stable technical error category.

Each choice is optional, independent and can be changed at any time under
**Profile → Privacy & diagnostics**. Refusing does not restrict the App. We do
not set an Analytics or Crashlytics user ID and our telemetry layer rejects
email addresses, account IDs, passenger/form contents, exact routes, booking
references, authentication tokens and free-form feedback.

Google may create an app-instance/device identifier for these services after
the relevant choice is enabled. Analytics data is intended to be retained for
2 months and Crashlytics reports for 90 days; the matching Firebase-console
settings must remain configured accordingly.

### 2.3 Rewarded advertising — Android only

The current release does not enable rewarded advertising. A future Android
edition may offer an optional Google AdMob rewarded
video in exchange for virtual Miles. The iOS edition is normally paid but may
be temporarily free during a promotional campaign, and neither loads nor
embeds the mobile-ads SDK.

Before Android requests an ad, Google's consent flow is shown where required.
Ads are requested in non-personalized mode, but Google may still process an IP
address, device/app identifiers, consent state, ad interaction and fraud/
delivery information for ad serving, frequency capping, reporting, security
and reward verification. Refusing optional advertising consent prevents an ad
request; it does not prevent ordinary use of the App.

Reward credit is verified server-to-server. The App sends AdMob a short-lived,
single-use opaque reward token—not your Firebase UID. We retain the minimum
token/transaction marker needed to prevent duplicate credit until its expiry.

### 2.4 Backend, security and support data

Vercel functions receive the authenticated API request plus coarse app
version/build/platform headers. Runtime logs use generated request IDs and
stable status/error codes; they must not contain request bodies, tokens, UID,
email, booking reference, itinerary, passenger data or IP address. On the
current hosting plan runtime logs are available for a short operational window
(currently about one hour).

The unauthenticated deletion form uses a keyed one-way hash of the network
address for short-term abuse prevention; the raw address is not stored. If you
voluntarily send private feedback, we process the message and reply address
only to handle that request. Do not include sensitive or booking information.

We do not collect precise location, contacts, photos or microphone data. We do
not sell personal data and do not use data for cross-app tracking.

## 3. Legal bases and purposes

| Purpose | Legal basis where the GDPR/UK GDPR applies |
|---|---|
| Authentication, simulated bookings, balance, achievements, saved profile and account deletion | Performance of the service contract or steps requested by you |
| Security, fraud/duplicate-reward prevention, rate limiting and service reliability | Legitimate interests in protecting users, the service and its free quotas |
| Optional Analytics | Consent |
| Optional Crashlytics diagnostics | Consent |
| Optional Android advertising/identifier access where consent is required | Consent |
| Responding to rights requests and lawful authority requests | Legal obligation |

You may withdraw consent from the in-app privacy settings or Android ad privacy
options. Withdrawal does not affect earlier lawful processing.

## 4. Processors and recipients

- **Google Firebase / Google LLC:** Authentication, Firestore, optional
  Analytics and optional Crashlytics.
- **Google AdMob / Google LLC:** Android rewarded ads and server-side reward
  verification only after the applicable consent/ad-eligibility checks.
- **Apple Inc.:** Sign in with Apple and iOS distribution/payment.
- **Google Play:** Android distribution and any store-level payment.
- **Vercel Inc.:** backend functions, operational metrics and short-lived
  runtime logs.
- **Email delivery provider:** only when a user voluntarily submits feedback
  or contacts support.

Processors receive only what is needed for their role. We may also disclose
information when required by law, court order or a competent authority. We do
not share data for sale or cross-context behavioural advertising.

## 5. Retention

| Data | Retention |
|---|---|
| Account, balance, achievements and saved profile/reference | Until account deletion |
| Completed server booking history | Rolling 15-booking buffer; pending/live bookings are kept until completion processing |
| Recent Miles activity | Most recent 10 entries |
| Analytics / crash reports | Intended 2 months / 90 days respectively |
| Ad reward tokens and duplicate-prevention markers | Until their configured expiry/TTL |
| Runtime request logs | Hosting-plan operational window, currently about one hour |
| Web deletion request | Until processed, or deleted after 90 days if unresolved |
| Voluntary support/feedback | Only as long as needed to resolve and document the request, then deleted under the support-retention process |

Provider backups may retain encrypted copies for a limited ordinary backup
cycle after deletion.

## 6. International transfers

The App is available globally and its providers may process data outside your
country, including in the United States. Where required we use the relevant
provider data-processing terms and safeguards, such as adequacy decisions, the
EU Standard Contractual Clauses, the UK International Data Transfer Addendum,
or comparable contractual safeguards.

Transfers from Morocco are subject to Law 09-08 and any required CNDP
declaration/authorization; those regulatory steps must be completed before a
transfer that requires them is activated. Users in Brazil and other
jurisdictions retain the international-transfer protections required by their
local law.

## 7. Your choices and rights

Depending on your location, you may have rights to access, correct, delete,
restrict or object to processing, withdraw consent, obtain portability, and
appeal or complain to a regulator. Moroccan users may contact the CNDP; EEA
and UK users may contact their local supervisory authority; residents of
California, Brazil and other regions retain the rights granted by local law.
We do not sell or share personal information for behavioural advertising.

Contact **cs.ach.app@outlook.com** with the subject “Data Subject Request”. We
may need to verify that the request concerns your account. We aim to respond
within 30 days or the period required locally.

## 8. Account and data deletion

- **In the App:** Profile → Account → **Delete my account**. Authenticated
  deletion removes the Firebase account and associated server data.
- **Without the App:** submit the account email at
  [flight-booking-cyan-nu.vercel.app/delete-account](https://flight-booking-cyan-nu.vercel.app/delete-account).
  Because this path is not authenticated, ownership is reviewed and the
  request is completed within 30 days.

Device-only theme, language, diagnostics choices and mini-game preferences may
remain on the device after server account deletion and can be removed by
uninstalling/clearing the App.

## 9. Security

Traffic is encrypted in transit. Firestore rules deny client writes to
server-authoritative data and owner-scope permitted reads. Backend mutations
verify Firebase tokens, validate and bound inputs, rate-limit costly actions,
and use atomic/idempotent operations. Secrets and service-account credentials
are never shipped in the App. No system can be guaranteed completely secure;
report concerns to **cs.ach.app@outlook.com**.

## 10. Children

The App is not directed to children under 13 and we do not knowingly collect
their personal data. A user under the age of majority must have a parent or
guardian's permission where required. Contact us to report a child's account
for deletion.

## 11. Changes

Material changes update the version/date and are shown through the in-app legal
gate. Optional consent is never inferred from accepting the Terms or this
policy.

## 12. Contact

**Controller:** Ayoub El Hazzaz 
**Email:** cs.ach.app@outlook.com

---

*Last updated 2026-09-19 (v1.1). See also the [Terms and Conditions](./TERMS_AND_CONDITIONS.md).*
