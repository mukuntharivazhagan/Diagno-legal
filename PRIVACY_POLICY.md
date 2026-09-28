# Privacy Policy for DIAGNO: Clinical Diagnostic Mastery

**Effective Date:** September 27, 2026  
**Last Updated:** September 27, 2026  
**Application Name:** DIAGNO (com.diagno.health / Diagno Medical Learning App)  
**Developer Contact:** support@diagno.health / dev@diagno.health  

---

## 1. Introduction & Academic Mission

DIAGNO ("we," "our," or "us") provides a gamified, peer-reviewed clinical education and diagnostic simulation application designed for medical students, resident physicians, and healthcare practitioners. 

We take your digital privacy seriously. This Privacy Policy informs you about how we collect, process, store, and protect your information when you use our mobile application and web services.

> **CRITICAL MEDICAL DISCLAIMER & SYNTHETIC DATA STATEMENT**:  
> **DIAGNO contains strictly simulated, synthetic, or de-identified educational clinical vignettes.** No Protected Health Information (PHI) under the Health Insurance Portability and Accountability Act (HIPAA) or General Data Protection Regulation (GDPR) is hosted, processed, or permitted on this platform. Users must **never** input real patient identifiable information into any field in DIAGNO.

---

## 2. Information We Collect

We only collect data necessary to provide seamless game synchronization, educational progress tracking, difficulty auto-calibration, and UI performance optimization.

### A. Information You Provide Directly
* **Account Credentials & Authentication**: When you sign in using Google Sign-In or Email/Password via Firebase Authentication, we receive your email address, public display name, and avatar image URL.
* **Support & Feedback Submissions**: When you voluntarily submit diagnostic errors, question feedback, or support tickets via the in-app feedback modal, we collect your submitted category, comments, and application version.

### B. Educational Progress & User Game State
To allow cross-device progression, the following data points are securely synced to our Cloud Firestore database (`/users/{uid}`):
* **Academic Level & Experience**: User level, experience points (XP), clinical rating (CR / ELO matchmaking rating).
* **Diagnostic History**: Daily puzzle completions, grand rounds weekly quest stages, correct/incorrect diagnosis commits, differential choices, and clinical image challenges solved.
* **In-Game Virtual Economy**: Vitality Stones, Rubies, and Gems earned through diagnostic accuracy and daily streaks.
* **Companion Mascot & Progression**: Unlocked pets, pet stage (Egg, Juvenile, Young, Adult, Mastery), and enhancements.
* **Clinical Bookmarks & Achievements**: Saved high-yield clinical pearls, bookmarked diagnostic cases, and unlocked achievement medals.
* **Match & Duel History**: Outcomes of 1v1 Classic Mode Arena and Battleship Game Mode duels (scores, response speeds, wagers).

### C. Automated Telemetry & Analytics (Envelope Architecture)
Every interaction event logged through our custom analytics framework records a standardized envelope containing:
* `user_id`: Anonymized user identifier (or authenticated Firebase UID).
* `session_id`: Unique identifier generated per app session.
* `session_number`: Cumulative count of app launches.
* `timestamp`: ISO 8601 millisecond timestamp.
* `screen` & `feature`: Navigation screen (e.g., `daily`, `reels`, `arena`, `pets`) and feature module.
* `platform` & `app_version`: Client runtime environment (`android`, `ios`, `pwa`, `web`) and application build version.
* `user_level`, `user_rating`, `user_streak`: Contextual skill parameters to evaluate content difficulty.

### D. Educational Difficulty & UX Friction Detection
To discover where medical trainees experience cognitive overload or confusing UI elements:
* **Adaptive Difficulty Calibration**: We aggregate response time, clue reveal frequency, and case abandonment rates to balance question difficulty.
* **UX Friction Metrics**: We collect non-intrusive UI interaction anomalies (such as repeated clicks on unresponsive elements, rapid tap bursts, and screen bounce backtracks) with anonymous screen coordinates to generate interface heatmaps and fix software bugs.

### E. Information We NEVER Collect
* ❌ We **do not** collect GPS location or precise geolocation.
* ❌ We **do not** access your device contacts, address book, or calendar.
* ❌ We **do not** access your microphone, camera, or local media files.
* ❌ We **do not** collect credit card numbers or financial account details (all in-game currency is earned virtually).
* ❌ We **do not** track your activity across third-party websites or sell advertising identifiers.

---

## 3. How We Use Your Information

We process collected data exclusively for the following purposes:
1. **Core App Functionality**: Authenticating your identity, syncing your level, streak, and companion pets across all your devices.
2. **Clinical Content Balancing**: Analyzing which clinical vignettes have disproportionately high failure rates to refine explanations and hint quality.
3. **Multiplayer Matchmaking**: Pairing you with peers of comparable clinical rating (CR) during synchronized medical speed duels.
4. **Bug Diagnosis & Crash Prevention**: Identifying interface dead clicks, dropped network calls, and latency bottlenecks.
5. **Academic Reporting**: Calculating global anonymized leaderboards and peer percentiles.

---

## 4. Third-Party Infrastructure & Data Processors

DIAGNO relies on enterprise-grade cloud providers that adhere to rigorous security standards:
* **Google Firebase (Cloud Firestore & Firebase Authentication)**: Cloud database and authentication services provided by Google LLC. Data is encrypted at rest using AES-256 and in transit using TLS 1.3.
* **Google Cloud Platform**: Server hosting and API proxy infrastructure.

We **never** sell, rent, or trade your personal data to third parties, data brokers, advertising networks, or pharmaceutical sponsors.

---

## 5. Data Retention & Account Deletion

* **Retention Period**: Your profile, game state, and diagnostic records are retained as long as your account remains active. Aggregated telemetry summaries are archived for longitudinal difficulty modeling.
* **User Rights & Account Deletion**: Under GDPR, CCPA, and Google Play Data Safety policies, you have the right to inspect, export, or permanently delete your data. To request complete account deletion, email `privacy@diagno.health` or use the in-app Account Settings deletion request. Upon verification, all documents under `/users/{uid}` and corresponding authentication profiles will be deleted within 30 days.

---

## 6. Protection of Minors (COPPA)

DIAGNO is an academic tool intended for adult medical students and healthcare professionals aged 17 and older. We do not knowingly collect personal information from children under the age of 13.

---

## 7. Security Measures

We maintain industry-standard administrative, technical, and physical safeguards:
* Client-side Firestore Security Rules strictly restrict reading and writing `/users/{uid}` solely to the authenticated owner.
* Analytics event telemetry ingestion is write-only for clients to prevent peer data inspection.
* Zero storage of plaintext passwords (managed via OAuth 2.0 and Google Identity).

---

## 8. Updates to This Policy

We may update this policy periodically to reflect new educational features or regulatory requirements. Any modifications will be posted within the app under `Profile > About > Privacy Policy` and indicated by the "Last Updated" date above.

---

## 9. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or our data handling practices, please contact our Data Protection Officer:

* **Email**: `privacy@diagno.health`
* **Developer**: DIAGNO Medical Systems
* **Support Portal**: In-app `Profile > Help & Support`
