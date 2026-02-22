# Privacy Policy — Lappaa

**Last updated: February 2026**

---

## The Short Version

Lappaa does not collect, upload, or share your data. Your voice recordings, transcriptions, and exported videos never leave your device. There is no Lappaa account, no backend server, and no cloud processing of any kind.

---

## On-Device Processing — What This Actually Means

Every step of Lappaa's workflow — recording, transcription, audio mastering, AI background generation, and video rendering — runs entirely on your iPhone or iPad using Apple's native frameworks.

This is an architectural decision, not a policy promise. There is no server to receive your audio because there is no server.

Lappaa is fully functional in Airplane Mode.

---

## Permissions

### Microphone
Used to record audio when you start a recording session. Audio is stored locally on your device and is never transmitted. You control when recording starts and stops.

### Speech Recognition
Used to generate captions and transcripts on-device via Apple's framework.

Note: Apple's frameworks may have their own data handling at the OS level. See [Apple's Privacy Policy](https://www.apple.com/legal/privacy/) for details.

### Photo Library — Add Only
Used to save your exported videos to the Photos app. "Add Only" access means Lappaa cannot read or browse your existing photos.

### Photo Library — Read *(Pro import feature)*
Required when you choose to import a video from your Photo Library to extract its audio. Only accessed when you explicitly trigger this action.

### Notifications
Optional. Used for Live Activities — real-time recording status on your Lock Screen and Dynamic Island. No content is delivered from a remote server.

---

## AI Features (AI Backgrounds)

AI Backgrounds uses Apple's local language model running entirely on your device. Your transcript is processed locally to generate a background image. No text, audio, or images are sent to any external AI service or API.

Requires iPhone 15 Pro or newer.

---

## Purchases & Subscriptions

Lappaa Pro subscriptions and the Lifetime purchase are handled entirely by Apple via the App Store. Lappaa does not process payments and does not have access to your payment information. See [Apple's Media Services Terms](https://www.apple.com/legal/internet-services/itunes/).

---

## Data Stored on Your Device

Lappaa stores locally:
- Audio recordings and imported audio files
- Draft projects (trim points, text, layout, visualizer settings)
- Exported video files (before sharing)
- App settings and preferences

This data is protected by your device's encryption when the device is locked. Lappaa does not use iCloud sync.

---

## Draft Cleanup

To manage local storage, Lappaa applies automatic cleanup rules you can configure in Settings:

- **Active drafts** — deleted after 7 days (default, configurable)
- **Exported drafts** — deleted after 30 days (default, configurable)
- **Archived drafts** — never deleted automatically

You can manually delete any draft or recording at any time.

---

## GDPR

Lappaa is developed in Europe and built with GDPR compliance as a structural default. Because no personal data is processed externally, there is no data controller relationship in the conventional sense. Your rights — access, portability, deletion — are exercised entirely on your own device. Deleting the app removes all data.

---

## Children

Lappaa is not directed at children under 13. Since no personal data is collected from any user, this is inherently satisfied.

---

## Changes

If this policy changes in a meaningful way, the date above will be updated. Given the local-only architecture, significant changes to data handling are unlikely.

---

## Contact

Questions? Visit the [Support page](SUPPORT.md) or open an issue in this repository.

---

*Lappaa is made in Europe by an independent developer committed to building tools that respect your data as much as your creativity.*
