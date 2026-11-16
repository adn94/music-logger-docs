# Privacy Policy

**Effective Date:** November 16, 2026

## 1. Responsible Contact (Controller)
**Ahmet Aydin, DigitalAydin**
Weidengasse 28
50668 Köln, Germany
Email: music.logger.app@gmail.com

## 2. Audio Data Handling (Microphone Access)
To provide the core "Background Recognition" feature, the apps (**Music Logger** & **Music Hunter**) require the `android.permission.RECORD_AUDIO` permission.

### Collection & Usage
*   **Collection:** We collect audio data solely for the purpose of identifying music playing in your environment.
*   **Processing:** Audio is processed in real-time. The audio stream is processed directly on your device to generate a unique digital fingerprint.
*   **No Permanent Storage:** We do **not** permanently store raw audio files on your device or our servers. The raw audio buffer is discarded immediately after the fingerprint is generated.
*   **Fingerprints Kept on Your Device (Music Hunter):** If a fingerprint finds no match when it is created, because you are offline or because the track is not (yet) known to the recognition service, Music Hunter keeps that fingerprint in its database on your device and checks it again later. A fingerprint is not a recording; no audio can be played back from it. It is deleted when the track has been identified, when you delete its session or your account in the app, when you tap "Clear fingerprints" (Settings -> Identify later), or at the next check after it has become older than the period you choose there (1, 3, 6 or 12 months; 6 by default). All fingerprints together take at most 25 MB; beyond that the oldest are removed first. Fingerprints are never uploaded to our servers.
*   **Repeated Tracks (iOS):** To recognise a track that plays again within a session, Music Hunter compares fingerprints of that session with each other on your device. Nothing leaves your device in this step.
*   **No Audio Transmission:** No raw audio files are ever transmitted to our servers or any third parties.

## 3. Third-Party Data Sharing

To provide our services, we partner with selected third-party providers.

### 3.1 Apple Music / ShazamKit
To identify songs, we use external services provided by **Apple (Shazam)**.
*   **Data Shared:** Only an anonymous digital fingerprint is shared. This fingerprint cannot be reversed into intelligible audio. A fingerprint that found no match when it was created may be sent to the recognition service again later, when the app checks it again.
*   **Purpose:** To retrieve song metadata (Title, Artist).
*   **Policy:** Usage is also subject to [Apple's Privacy Policy](https://www.apple.com/legal/privacy/en-ww/).

### 3.2 Spotify
Both apps can open a recognised track in Spotify.
*   **Opening a track:** The app opens Spotify (app or website) with a search for that track. Music Hunter searches by the track's ISRC (an international track code) if available, otherwise by title and artist. Nothing is sent to Spotify before you tap.
*   **Connect Spotify (Music Logger, and Music Hunter before 1.1.7):** Optional. When connected, the app sends title and artist to Spotify to find the exact track. It requests your basic profile (`user-read-private`) and stores an access token on your device. We do **not** access your private playlists or listening history.
*   **Removal:** Music Hunter 1.1.7 deletes this token from your device and no longer offers the connection. You can remove an app's access at any time in your Spotify account under [Manage apps](https://www.spotify.com/account/apps/).
*   **Policy:** What happens inside Spotify is subject to [Spotify's Privacy Policy](https://www.spotify.com/legal/privacy-policy/).

### 3.3 YouTube Music (Google)
Music Hunter can export a recognised session as a playlist in your own YouTube Music library. This only happens when you start the export yourself.
*   **Scope Requested:** `https://www.googleapis.com/auth/youtube` ("Manage your YouTube account"). The YouTube Data API requires this scope to create a playlist and add items to it; the read-only scope cannot write.
*   **Data Shared:** Only the titles and artists of the tracks in the session you export. They are sent to the YouTube Data API to find the matching videos and to add them to a newly created playlist in your account.
*   **What We Do Not Do:** We do **not** read any other data from your Google account, we do **not** store content of your channel, and we do **not** share anything with third parties.
*   **Security:** The access token is stored on your device only. Our servers never receive it.
*   **Withdrawal:** Revoke access at any time in the app under Settings -> Connected Services, or at [myaccount.google.com/permissions](https://myaccount.google.com/permissions).
*   **Limited Use:** Music Hunter's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.
*   **Policy:** By connecting your account, you agree to [Google's Privacy Policy](https://policies.google.com/privacy).

### 3.4 Apple Music (opening tracks, playlist export)
Both apps can open a recognised track in Apple Music. On iPhone, they can also save a session as a playlist in your Apple Music library.
*   **Opening a track:** When you tap it, the app looks the track up in Apple's public music catalogue, by its Apple Music ID or by title and artist. Nothing is sent before you tap.
*   **Playlist export (iPhone):** Optional, and only when you start it. iOS first asks you to allow access to Apple Music. The app then sends the playlist name, a short description ("Recorded with Music Hunter" or "Recorded with Music Logger") and the matching tracks to Apple, which creates the playlist in your library.
*   **What We Do Not Do:** We do **not** read your Apple Music library or listening history. The lookup and the export go directly from your device to Apple. Our servers are not involved.
*   **Withdrawal:** You can remove an app's access to Apple Music at any time in the iPhone Settings.
*   **Policy:** What happens inside Apple Music is subject to [Apple's Privacy Policy](https://www.apple.com/legal/privacy/en-ww/).

## 4. Data Retention & Deletion
*   **Recognition Logs:** Metadata (Title, Artist, Timestamp) is stored locally and, if Sync is enabled, in our secure Supabase cloud.
*   **Fingerprints (Music Hunter):** Fingerprints without a match are stored on your device (see Section 2) and are not synchronised to our cloud. Like the rest of the app's local data, they can be included in your device's own backups (for example iCloud or Google backup) if you have enabled them. Deleting a session or your account in the app removes the fingerprints belonging to it from this device; uninstalling the app removes all of them.
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
