# Privacy Policy

**Effective Date:** February 2, 2026

## 1. Responsible Contact (Controller)
**Dj Chami & Chantre Productions UG**
Germanusstrasse 30
52080 Aachen, Germany
Email: music.logger.app@gmail.com

## 2. Audio Data Handling (Microphone Access)
To provide the core "Background Recognition" feature, the app requires the `android.permission.RECORD_AUDIO` permission.

### Collection & Usage
*   **Collection:** We collect audio data solely for the purpose of identifying music playing in your environment.
*   **Processing:** Audio is processed in real-time. The audio stream is processed directly on your device to generate a unique digital fingerprint.
*   **No Permanent Storage:** We do **not** permanently store raw audio files on your device or our servers. The raw audio buffer is discarded immediately after the fingerprint is generated.
*   **No Audio Transmission:** No raw audio files are ever transmitted to our servers or any third parties.

## 3. Third-Party Data Sharing (Shazam)
To identify songs, we use external services provided by **Apple (Shazam)**.
*   **Data Shared:** Only an anonymous digital fingerprint is shared. This fingerprint cannot be reversed into intelligible audio.
*   **Purpose:** To retrieve song metadata (Title, Artist).
*   **Policy:** Usage is also subject to [Apple's Privacy Policy](https://www.apple.com/legal/privacy/en-ww/).

## 4. Data Retention & Deletion
*   **Recognition Logs:** Metadata (Title, Artist, Timestamp) is stored locally and, if Sync is enabled, in our secure Supabase cloud.
*   **Account Deletion:** You can delete your account and all associated cloud data at any time:
    *   **In-App:** Settings -> Account -> Delete Account.
    *   **Email:** Contact music.logger.app@gmail.com with the subject "Data Deletion Request".

## 5. Security
*   **Encryption in Transit:** All network communication is transmitted over secure **HTTPS / SSL** connections.
*   **Encryption at Rest:** Sensitive account data is encrypted in our cloud database.

## 6. Your Rights (GDPR)
Under the GDPR, you have the following rights:
*   **Access & Correction:** Request details or corrections of your data.
*   **Deletion:** Request the erasure of your data.
*   **Withdrawal of Consent:** Revoke microphone permissions at any time in device settings.
*   **Complaint:** Lodge a complaint with a supervisory authority (e.g., LDI NRW).
