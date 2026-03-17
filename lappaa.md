# Lappaa — Voice to Video

**Last Updated:** 2026-03-17
**Platform:** iOS 26.0+ / iPadOS 26.0+

---

## Product Overview

Lappaa is an iOS and iPadOS app for turning voice recordings and audio into shareable social videos. It's built for musicians, artists, DJs, podcasters, business professionals, and anyone who wants their audio to be seen on messaging apps and social media — rather than waiting for someone to press play.

The core idea is simple: raw audio is invisible on visual platforms and often ignored in messaging apps. Lappaa "unboxes" it — instantly wrapping your voice or music in your custom animated visualizers, auto-generated captions, and custom backgrounds, then exporting a video ready for Instagram, TikTok, WhatsApp, or iMessage.

**Tagline:** "Give Your Voice a Visual"

**Philosophy:** Raw audio is invisible, your voice deserves to be seen.

### Core Capabilities

- **Record:** High-quality audio capture with live visualizers and optional Voice Isolation.
- **Import *(Pro)*:** Bring in audio from Files, Photos (video extraction), or Clipboard.
- **Edit:** Canvas-based video editor with 17 visualizer styles, custom text, and background options.
- **Transcribe:** On-device speech-to-text — automatic captions, no internet needed.
- **Master *(Pro)*:** Audio Mastering with configurable LUFS target (-23 to -14).
- **Export:** Share via iOS Share Sheet to Instagram, TikTok, Youtube, X, Threads, Telegram, iMessage, and more.

### Use Cases

| Scenario | Solution |
|----------|----------|
| Elevate an Instagram DM | Record and send an "unboxed" voice note: turn a raw audio bubble into a personalized, visual micro-video |
| TikTok hot take or rant | Record a thought, apply fast-paced word-by-word captions, post 9:16 instantly |
| Aesthetic Brain Dumps | Voice journal over a mood photo or AI background to make an aesthetic mini-vlog |
| Share a beat or song idea | Import a raw voice memo of a strumming idea, add visualizer, post to feed |
| Publish a full track to YouTube | Import audio, add stylish cover art and a 16:9 visualizer template, upload |
| Post a TikTok of a DJ mix without filming | Import audio, set background, normalize to -14 LUFS, share |
| Experts sharing quick insights | Record voice note, auto-caption, export a branded 1:1 video for your audience (e.g. LinkedIn)|

### Pricing

**Free:** Core recording, all 9 live visualizers, all 17 editor visualizers, canvas editor, on-device transcription, AI Backgrounds (on supported devices), all aspect ratios, export with watermark.

**Lappaa Pro:**
- Import audio (Files, Photos, Clipboard)
- Watermark-free exports
- Audio Mastering (configurable -23 to -14 LUFS)
- Word-by-Word captions

Available as Weekly, Monthly, Yearly (auto-renewable), or Lifetime (non-consumable) via Apple In-App Purchase.

---

## Recording

### Live Visualizer Styles (Recorder)

9 styles available in real time during recording:

| Style | Character |
|-------|-----------|
| Waveform | Classic amplitude trace |
| Radial Bar | Circular bar chart around center |
| Radial Spikes | Spiky radial energy bursts |
| Neon | Glowing neon line oscillator |
| CRT Line (Phosphor) | Phosphor green scan-line aesthetic |
| Spectrum | Frequency bar chart |
| Retro Stack (Winamp) | Layered bar columns, retro VU style |
| Vector Round | Smooth continuous closed curve |
| Vector Square | Angular closed vector path |

**Gesture:** Long press the visualizer to open the style picker.

### Timer Styles

8 aesthetic clock/timer displays:

Flip Clock · Nixie Tube · Digital LED · Standard · Minimal · Neon · Analog · Retro Terminal

**Gesture:** Long press the timer to open the style picker. Double tap to toggle visibility.

### Input Modes

**Standard** — Full-fidelity microphone capture at 44.1kHz / 32-bit float internal processing. No processing applied to the input signal.

**Voice Isolation** — Enables Apple's system-level real-time noise filtering and echo cancellation at the OS level before audio enters the recording pipeline. Designed for noisy or untreated environments. Note: Voice Isolation processes the microphone input only; it is not applied to imported audio files.

### System Integration

- **Siri & App Shortcuts:** Lappaa supports hands-free control via **AppIntents**. Start a recording instantly by saying:
    * *"Siri, start recording in **Lappaa**"*
    * *"Siri, record with **Lappaa**"*
    * *"Siri, start **Lappaa**"*
    * *"Siri, record **Lappaa**"*
    * *"Siri, start a session in **Lappaa**"*
    * *"Siri, **Lappaa**"*
- **Control Center widget:** Configurable via iOS Settings → Control Center (iOS 26+).
- **Home Screen widgets:** Available in multiple sizes.
- **Live Activities:** Real-time recording duration and waveform pulse on Lock Screen and Dynamic Island.
- **Background recording:** Audio capture continues when the app is backgrounded or the screen is locked.

---

## Import *(Lappaa Pro)*

Three import sources, accessed via long press on the Import button in the Recorder view:

**Files** — Opens the iOS Files app. Supports common audio formats. Audio is transcoded to 44.1kHz AAC in a background process after import.

**Photos** — Selects a video from the Photo Library and extracts its audio track. Requires Photo Library read access. The video track is discarded; only audio is imported.

**Clipboard** — Imports a copied audio file or URL from the system clipboard.

All imported audio is automatically converted to 44.1kHz AAC via a background actor. The import process does not block the main thread.

---

## Magic Editor

The editor is a canvas-based video builder. All elements are moveable and resizable.

### Visualizer Styles (Editor)

17 animated styles reacting to the audio waveform:

Bars · Wave · Spectrum · Line · Dots · Ripple · Mountain Layers · Retro Stack · Neon · Pulse Circle · Orbit · Helix · Radial Bars · Radial Spikes · CRT Trace · Vector Round · Vector Square

### Canvas & Aspect Ratios

| Format | Dimensions | Use |
|--------|-----------|-----|
| 9:16 Vertical | Story format | Instagram Stories, TikTok, Reels |
| 1:1 Square | Feed format | Instagram/Facebook feed posts |
| 16:9 Landscape | Wide format | YouTube Shorts, presentations |

**Per-format state:** Layout, element positions, and sizes are saved independently per aspect ratio. Switching between formats restores the previous configuration for that format.

### Canvas Elements

- **Header** — Primary title text
- **Subheader** — Secondary text
- **Caption** — Transcription / caption block
- **Visualizer** — Animated audio-reactive graphic

All elements support drag (move), pinch (resize), and snap-to-full-width (pinch visualizer outward). Double tap any element to reset to default position/size.

**Vertical drag lock:** When an element is at full width, drag is locked to the Y-axis only.

### Background Options

- **Solid color** — Any hex value
- **User photo** — Import from Photos library or paste from Clipboard (long press background icon). Includes a Gaussian blur slider.
- **AI Backgrounds** — Generated on-device via ImagePlayground *(iPhone 15 Pro+)*

### Typography

Font families: System · Rounded · Serif · Mono
Controls: Weight, alignment (left / center / right)

**Gesture:** Long press any title or subtitle element to open a quick-edit text alert.

### Timeline

- **Zoom:** Pinch gesture, 0.5× to 50× magnification
- **Fit to screen:** Button to reset zoom to show the full clip
- **Scrub / seek:** Drag playhead to any position
- **Loop toggle:** Loops the current selection during playback
- **Double tap duration:** Snaps selection to maximum allowed duration from current start handle
- **Double tap start/end handle:** Jumps playhead to that clip boundary
- **Long press timestamp:** Snaps the nearest handle (start or end) to the current playhead position
- **Single tap ruler:** Quick seek to that timestamp

**Auto-Trim:** On load, analyzes the global waveform and automatically sets trim handles to skip silence at the start and end (threshold: <5% amplitude).

---

## Transcription

On-device speech recognition using Apple's native framework.

### Automatic Captioning

Transcription starts automatically when a recording is opened in the editor. Segments are aligned to the audio timeline and displayed as caption overlays.

**Orphan Fixer:** Leading punctuation (periods, commas) is automatically moved from the start of a segment to the end of the previous segment.

### Editing

- Edit any segment's text directly
- Adjust segment start/end timing
- Search & Replace: single occurrence or all occurrences
- Undo / redo support

### Import / Export

**Import:** `.srt` or `.vtt` files replace the current transcript.

**Export options:**
- `.srt` subtitle file
- Raw audio file
- Plain text transcript

---

## AI Backgrounds *(iPhone 15 Pro+)*

**How it works:**
The current transcript or title text is passed to a local LLM.
The entire pipeline runs on-device. No text or images are transmitted externally.

---

## Social Audio Normalization *(Lappaa Pro)*

**What it does:** Measures the integrated loudness (LUFS) and True Peak of the audio, then normalizes and limits it to a user-selected target before export.

**LUFS target range:** -23 LUFS (broadcast standard) to -14 LUFS (streaming-optimized), user-adjustable.

**Platform guidance:**

| Platform | Target | Notes |
|----------|--------|-------|
| Instagram Reels | -14 to -16 LUFS | Prevents algorithmic volume ducking |
| TikTok | -13 to -14 LUFS | Competitive loudness for mobile speakers |
| YouTube Shorts | -13 to -14 LUFS | Normalized to this target on upload |
| Podcast / voice | -23 LUFS | EBU R128 broadcast standard |

**Scope:** Audio normalization in Lappaa is designed to ensure exported videos play correctly on algorithmic social media feeds. It is not intended to be a professional, lossless studio mastering suite for audio distribution.

---

## Draft Lifecycle

Lappaa manages local storage automatically.

| Draft State | Auto-Delete | Notes |
|-------------|-------------|-------|
| Active | After 7 days (configurable) | Working sessions |
| Active (versioned) | When exceeding 5 versions per recording | — |
| Exported | After 30 days (configurable) | Marked after any export |
| Exported (versioned) | When exceeding 10 versions per recording | — |
| Archived | Never | Protected from all cleanup |

**Manual delete:** Any draft can be deleted at any time by the user.

---

## Gestures Reference

| View | Gesture | Outcome |
|------|---------|---------|
| Recorder | Long press visualizer | Opens style picker |
| Recorder | Long press Import button | Opens import source dialog (Files / Photos / Clipboard) |
| Recorder | Long press timer | Opens timer style picker |
| Recorder | Double tap timer | Toggles timer visibility (Hidden ↔ last active style) |
| Editor canvas | Pinch element | Resizes the element |
| Editor canvas | Pinch visualizer outward | Snaps visualizer to 100% canvas width |
| Editor canvas | Double tap element | Resets to default position and size |
| Editor canvas | Vertical drag (full-width element) | Locked to Y-axis |
| Editor canvas | Long press background icon | Pastes image from system clipboard |
| Editor canvas | Long press title / subtitle | Opens quick-edit text alert |
| Timeline | Single tap ruler | Quick seek to timestamp |
| Timeline | Double tap duration | Snaps selection to max duration from current start |
| Timeline | Double tap start/end handle | Jumps playhead to clip boundary |
| Timeline | Long press timestamp | Snaps nearest handle to playhead position |
| Template row | Double tap | Toggles as default template for its aspect ratio |

---

## Privacy

All processing is local. No audio, transcripts, or images leave the device.

See [PRIVACY.md](PRIVACY.md) for the full policy.

---

## System Requirements

- iOS 26.0+ / iPadOS 26.0+
- Microphone permission — required for recording
- Speech Recognition permission — required for transcription
- Photo Library ("Add Only") — required to save exported videos
- Photo Library (Read) — required for video (audio) import *(Pro)*
- Notifications — optional, used for Live Activities

Apple Intelligence features: iPhone 15 Pro / iPhone 15 Pro Max or newer, iOS 26+.

---

## Developer

Petri Kajander (Sunbird OÜ) — independent European developer, bootstrapped.

Same developer as [Nuotit](https://nuotit.org) — Podcast player for iOS and iPadOS.

- Website: [lappaa.com](https://lappaa.com)
- Support: [SUPPORT.md](SUPPORT.md)
