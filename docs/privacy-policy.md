# Privacy Policy

**Effective Date:** October 3, 2026

## 1. Responsible Contact (Controller)
**Dj Chami & Chantre Productions UG**
Germanusstrasse 30
52080 Aachen, Germany
Email: music.logger.app@gmail.com

## 2. Audio Data Handling (Microphone Access)
To provide the core "Background Recognition" feature, the apps (**Music Logger** & **Music Hunter**) require the `android.permission.RECORD_AUDIO` permission.

### Collection & Usage
*   **Collection:** We collect audio data solely for the purpose of identifying music playing in your environment.
*   **Processing:** Audio is processed in real-time. The audio stream is processed directly on your device to generate a unique digital fingerprint.
*   **No Permanent Storage:** We do **not** permanently store raw audio files on your device or our servers. The raw audio buffer is discarded immediately after the fingerprint is generated.
*   **No Audio Transmission:** No raw audio files are ever transmitted to our servers or any third parties.

## 3. Third-Party Data Sharing

To provide our services, we partner with selected third-party providers.

### 3.1 Apple Music / ShazamKit
To identify songs, we use external services provided by **Apple (Shazam)**.
*   **Data Shared:** Only an anonymous digital fingerprint is shared. This fingerprint cannot be reversed into intelligible audio.
*   **Purpose:** To retrieve song metadata (Title, Artist).
*   **Policy:** Usage is also subject to [Apple's Privacy Policy](https://www.apple.com/legal/privacy/en-ww/).

### 3.2 Spotify
We integrate with Spotify to provide direct playback features.
*   **Data Shared:** When you connect your Spotify account, we transmit search queries (Song Title, Artist) to Spotify to locate tracks.
*   **Permissions:** We request access to your basic profile (`user-read-private`) to authenticate requests. We do **not** access your private playlists or listening history.
*   **Security:** Authentication tokens are stored securely on your device. We do not process or store your Spotify credentials.
*   **Policy:** By connecting your account, you agree to [Spotify's Privacy Policy](https://www.spotify.com/legal/privacy-policy/).

### 3.3 YouTube Music (Google)
Music Hunter can export a recognised session as a playlist in your own YouTube Music library. This only happens when you start the export yourself.
*   **Scope Requested:** `https://www.googleapis.com/auth/youtube` ("Manage your YouTube account"). The YouTube Data API requires this scope to create a playlist and add items to it; the read-only scope cannot write.
*   **Data Shared:** Only the titles and artists of the tracks in the session you export. They are sent to the YouTube Data API to find the matching videos and to add them to a newly created playlist in your account.
*   **What We Do Not Do:** We do **not** read any other data from your Google account, we do **not** store content of your channel, and we do **not** share anything with third parties.
*   **Security:** The access token is stored on your device only. Our servers never receive it.
*   **Withdrawal:** Revoke access at any time in the app under Settings -> Connected Services, or at [myaccount.google.com/permissions](https://myaccount.google.com/permissions).
*   **Limited Use:** Music Hunter's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.
*   **Policy:** By connecting your account, you agree to [Google's Privacy Policy](https://policies.google.com/privacy).

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
