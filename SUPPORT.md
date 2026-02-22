# Support — Lappaa

Questions about Lappaa? Start here. If something's missing, [open an issue](https://github.com/petrikaj/lappaa/issues).

---

## Basics

### What is Lappaa?
Lappaa is an iOS and iPadOS app that turns voice recordings and audio into shareable social videos. Record or import audio, add animated visualizers and auto-generated captions, pick a background, and export a video ready for Instagram, TikTok, WhatsApp, or any messaging app.

### Do I need an account?
No. Lappaa requires no account, no sign-in, and no email address. Download and start recording.

### Does it work offline?
Yes, completely. Recording, transcription, video rendering, and AI background generation all happen on your device. No internet connection is needed after the app is installed.

### Does my audio get uploaded anywhere?
No. Nothing leaves your device. See [PRIVACY.md](PRIVACY.md).

---

## Recording

### How do I start recording?
Tap the record button. You can also use "Hey Siri, Start Recording in Lappaa" via Siri Shortcuts, or add the Lappaa widget to your Control Center or Home Screen for instant one-tap capture.

### What is Voice Isolation?
Voice Isolation turns on Apple's system-level microphone processing, which filters background noise and echo in real time before anything is recorded. It's useful for noisy environments like cafés or outdoors. Toggle it in the recorder settings.

Note: Voice Isolation applies to the microphone only. It is not applied when you import existing audio files.

### Can I record with the screen off?
Yes. Recording continues in the background when you lock your screen or switch apps. Your Live Activity on the Lock Screen will show recording status.

### How do I change the visualizer style while recording?
Long press the visualizer on the recording screen.

### How do I change the timer style?
Long press the timer. To hide the timer entirely, double tap it.

---

## Magic Editor

### What can I edit?
The Magic Editor is a canvas where you control:
- Animated visualizer style (17 options)
- Title, subtitle, and caption text
- Background: solid color, your photo, or AI-generated
- Aspect ratio: 9:16 (Stories/TikTok), 1:1 (Square), 16:9 (Landscape)
- Fonts, weights, and text alignment
- Trim points via the zoomable timeline

### How do I move and resize elements?
Drag to move. Pinch to resize. Pinch the visualizer outward to snap it to full canvas width. Double tap any element to reset it to its default position and size.

### Will my layout reset when I switch aspect ratios?
No. Lappaa saves your layout independently for each aspect ratio. Switch to 1:1, adjust, switch back to 9:16 — each configuration is remembered.

### What is Auto-Trim?
When you open a recording, Lappaa automatically detects silence at the start and end and suggests trim points. This saves you from manually finding where the audio begins and ends.

---

## Captions & Transcription

### How does transcription work?
Lappaa uses Apple's on-device speech recognition. It starts automatically when you open a recording in the editor. Nothing is sent to the internet.

### Can I edit the captions?
Yes. Tap any segment to edit text, adjust timing, or delete it. Search & Replace works across the whole transcript. Undo/redo is supported.

### Can I import my own subtitles?
Yes. Import `.srt` or `.vtt` files to replace the auto-generated transcript.

### Can I export my transcript?
Yes — as `.srt` or plain text from the editor menu.

---

## AI Backgrounds

### What are AI Backgrounds?
Lappaa reads the mood and content of your transcript using a local AI model and generates a matching background image — entirely on your device. No prompt, no cloud, no account.

### Which devices support AI Backgrounds?
iPhone 15 Pro, iPhone 15 Pro Max, and any newer iPhone or iPad with equivalent or greater neural hardware. Requires iOS 26.0 or later.

### Why isn't AI Backgrounds available on my device?
AI Backgrounds uses Apple's framework, which requires specific neural hardware. This is an Apple hardware requirement, not a Lappaa limitation.

---

## Audio Mastering *(Lappaa Pro)*

### What is Audio Mastering?
It measures your audio's loudness and normalizes it to a target level after recording or audio import: your video sounds consistent and right on any platform.

### What LUFS target should I use?

LUFS (Loudness Units Full Scale) measures perceived audio loudness. Different platforms have different targets:

| Content | Recommended Target | Reason |
|---------|-------------------|--------|
| Music / DJ clips for Instagram or TikTok | -14 LUFS | Prevents your audio being ducked by the algorithm |
| Voice notes / talk content | -23 LUFS | EBU R128 broadcast standard |
| General social media | -16 to -18 LUFS | Safe middle ground |

If you're posting music and it sounds quieter than everything else in the feed, try -14 LUFS.

### Will it distort my audio?
No. Lappaa applies a safety limiter at -2 dBTP to prevent clipping before and after normalization.

---

## Lappaa Pro

### What does Pro include?
- **Import audio** — from the iOS Files app, from video files in your Photo Library, or from your Clipboard
- **No watermark** on exports
- **Audio Mastering** with adjustable LUFS target (-23 to -14)
- **Word-by-word caption generation** (on supported devices)

### How do I get Pro?
Open Lappaa → Settings → Lappaa Pro. Choose from weekly, monthly, yearly, or a one-time Lifetime purchase. All billing is through Apple.

### How do I restore my purchase on a new device?
Settings → Lappaa Pro → Restore Purchases. Your purchase is tied to your Apple ID.

### How do I cancel my subscription?
iPhone Settings → Apple ID → Subscriptions → Lappaa.

---

## Importing Audio *(Pro)*

### What can I import?
- **Files app** — common audio formats (MP3, AAC, WAV, FLAC, M4A, and more)
- **Photos** — any video in your library; Lappaa extracts the audio track
- **Clipboard** — copied audio files or URLs

### How do I import audio from a video I filmed?
Long press the Import button in the Recorder view → choose Photos → select your video. Lappaa will extract the audio automatically.

### Does Lappaa compress my imported audio?
All imported audio is converted to 44.1kHz AAC for internal processing. This happens in the background. For export, Audio Mastering *(Pro)* then normalizes the loudness to your chosen target.

---

## Exporting & Sharing

### Where can I share my videos?
Anywhere that accepts video. Lappaa uses the native iOS Share Sheet — you can send directly to Instagram, TikTok, WhatsApp, Signal, Telegram, iMessage, save to Files, or save to Photos.

### How do I auto-save every export to my Photo Library?
Settings → Auto-Save to Photos → On.

### Why is there a watermark on my export?
Watermark-free exports are a Lappaa Pro feature. Upgrade to remove it.

---

## Storage & Drafts

### How does Lappaa manage storage?
Drafts are stored locally. Automatic cleanup rules (all configurable in Settings):
- **Active drafts** — deleted after 7 days
- **Exported drafts** — deleted after 30 days
- **Archived drafts** — never automatically deleted

You can also delete any draft manually at any time.

### What does archiving a draft do?
Archiving protects a draft from all automatic cleanup, permanently. Use it for recordings you want to keep indefinitely.

---

## Siri, Widgets & Shortcuts

### How do I set up the Siri Shortcut?
Say "Hey Siri, Start Recording in Lappaa" to start hands-free recording.

### How do I add the Control Center widget?
Control Center → look for Lappaa in the available controls list.

### How do I add the Home Screen widget?
Long press your Home Screen → tap **+** → search "Lappaa" → add your preferred widget size.

---

## Troubleshooting

### Microphone isn't recording
iPhone Settings → Privacy & Security → Microphone → enable Lappaa.

### AI Backgrounds  isn't available
Confirm you have iPhone 15 Pro or newer and are running iOS 26.0 or later.

### Live Activity isn't showing during recording
iPhone Settings → Lappaa → Live Activities → enable.

---

## Contact & Feedback

Found a bug or have a feature idea? [Open an issue](https://github.com/petrikaj/lappaa/issues) or use the feedback option inside the app.

Lappaa is built by an independent European developer — feedback is read and genuinely appreciated.

---

*Privacy policy: [PRIVACY.md](PRIVACY.md)*
