# Lappaa — Voice to Video

**Last Updated:** 2026-05-05
**Platform:** iOS 26.0+ / iPadOS 26.0+

---

## Product Overview

Lappaa is a high-fidelity recorder that wraps your voice or video in a visual — captions, a visualiser, a background — and outputs a platform-ready video. One take. No timeline. No multi-clip editing. No cloud upload. Done in under a minute.

The workflow is simple: record or import, set your look in the editor, trim the ends, export. Or save a template once and skip the editing entirely — every future recording applies your template automatically, so the only step left is trimming.

The result works natively on Instagram Stories, Reels, TikTok, YouTube, LinkedIn, WhatsApp, iMessage, Signal, Telegram — anywhere that accepts a video file. Recipients can read the auto-captions even with sound off. Everything — recording, transcription, AI generation, mastering — happens on-device. No account. No internet required.

**Tagline:** "Give Your Voice a Visual"

**Philosophy:** Raw audio is invisible. Your voice deserves to be seen.

---

## Who It's For

Lappaa doesn't care what your job title is. It's for anyone who would rather say something than type it, and who wants the result to look like they meant it that way.

- **Say it once. Look like you meant it:** Record a 60-second update, a client note, a team announcement, or a pitch. The visual — captions, a clean background, your font — makes it feel considered even when it took ninety seconds to make. Save a template and the next one takes even less.
- **Creators wanting clips without production overhead:** Audiograms for Stories, teaser clips for Reels or TikTok, word-by-word captions synced to your audio. No desktop software. No session-by-session setup once you've saved a template.
- **Musicians and producers:** 32-bit float capture for demos and ideas. Import a finished master track, add a visualiser, normalise loudness, and export a 16:9 video for YouTube — from your phone, in one pass.
- **The new voice message:** Send an "unboxed" voice note on WhatsApp, Signal, iMessage, or Telegram. It plays like a video, reads like a caption, and lands like a personal message.

### Common Scenarios

| Scenario | What Lappaa Does |
|----------|-----------------|
| Async update for a client or team | Record once, auto-caption, export branded 1:1 — no typing required |
| TikTok hot take or rant | Word-by-word captions, 9:16 format, posted in under a minute |
| Audiogram for a podcast episode | Import audio, pick a visualiser, export Stories-ready clip |
| Share a beat or song idea | Record or import, add visualiser, post to feed |
| Publish a full track to YouTube | Import master, add 16:9 visualiser, normalise to -14 LUFS, export |
| DJ mix clip without filming | Import media, set background, normalise, share |
| Voice journal over a mood photo | Record over an imported photo or AI background |

---

## Saved Templates

Set your visual look once — background, font, visualiser, caption style, aspect ratio — and save it as a template. Every future recording applies it automatically. After recording, the only decision is where to trim.

Templates are optional. You can always record, adjust in the editor, and send with no template saved. But once you find a look, templates make the editor optional too.

---

## What It's Not

Lappaa is not a multi-clip editor. There is no timeline of cuts, no colour grading, no multi-track audio. It is built for single takes — you say it once and the result looks intentional.

If you need to assemble clips from multiple sources, CapCut, Instagram Edits, or a proper NLE are the right tools. If you need screen recording and camera overlays for walkthroughs, Loom is built for that. Lappaa is what you reach for when you don't need any of that — when the content is your voice and the job is making it watchable.

---

## Pricing

**Free:** Core recording, all 9 live visualisers, all editor visualisers, canvas editor, on-device transcription, AI Backgrounds (on supported devices), all aspect ratios, export with watermark.

**Lappaa Pro:**
- Import media (Files, Photos, Clipboard)
- Watermark-free exports
- Audio Mastering (configurable -23 to -14 LUFS)
- Word-by-Word captions

*Available as Weekly, Monthly, Yearly (auto-renewable), or Lifetime (non-consumable) via Apple In-App Purchase.*

---

## Technical Reference & Feature Catalog

### 1. High-Fidelity Recording

Lappaa is built around a professional-grade audio engine first. The visual layer comes after — not the other way around.

**Input Modes:**

- **Standard** — Full-fidelity microphone (and camera) capture at 32-bit float internal processing. No processing applied to the input signal.
- **Voice Isolation** — Enables Apple's system-level real-time noise filtering and echo cancellation before audio enters the recording pipeline. Designed for noisy or untreated environments. Note: Voice Isolation applies to microphone input only — it is not applied to imported media files.

**Live Visualiser Styles (9):**

| Style | Character |
|-------|-----------|
| Waveform | Classic amplitude trace |
| Radial Bar | Circular bar chart around centre |
| Radial Spikes | Spiky radial energy bursts |
| Neon | Glowing neon line oscillator |
| CRT Line (Phosphor) | Phosphor green scan-line aesthetic |
| Spectrum | Frequency bar chart |
| Retro Stack (Winamp) | Layered bar columns, retro VU style |
| Vector Round | Smooth continuous closed curve |
| Vector Square | Angular closed vector path |

*Gesture: Long press the visualiser to open the style picker.*

**Timer Styles (8):** Flip Clock · Nixie Tube · Digital LED · Standard · Minimal · Neon · Analog · Retro Terminal

*Gesture: Long press the timer to open the style picker. Double tap to toggle visibility.*

**System Integration:**

- **Siri & App Shortcuts:** Hands-free control via AppIntents. Examples:
  - *"Siri, start recording in Lappaa"*
  - *"Siri, record with Lappaa"*
  - *"Siri, start Lappaa"*
  - *"Siri, record Lappaa"*
  - *"Siri, start a session in Lappaa"*
  - *"Siri, Lappaa"*
- **Control Center widget:** Configurable via iOS Settings → Control Center (iOS 26+).
- **Home Screen widgets:** Available in multiple sizes.
- **Live Activities:** Real-time recording duration and waveform pulse on Lock Screen and Dynamic Island.
- **Background recording:** Audio capture continues when the app is backgrounded or the screen is locked.

---

### 2. Import Media *(Lappaa Pro)*

Three import sources, accessed via long press on the Import button in the Recorder view. All imported audio is automatically converted and mastered.

- **Files** — Opens the iOS Files app. Audio is transcoded to 44.1kHz AAC in a background process after import.
- **Photos** — Selects a video from the Photo Library. Requires Photo Library read access.
- **Clipboard** — Imports a copied media file or URL from the system clipboard.

---

### 3. The Visual Editor

A canvas-based video builder. All elements (Header, Subheader, Caption, Visualiser, Imported Media) are moveable and resizable. Layout, element positions, and sizes are saved independently per aspect ratio (9:16, 1:1, 16:9) — switching formats restores the previous configuration for that format.

**Visualiser Library (30+ styles):**

- *Standard & Abstract:* Bars, Wave, Pulse Circle, Spectrum, Line, Dots, Orbit, Ripple, Helix, Mountain Layers, Neon.
- *Retro & Geometric:* Radial Bars, Radial Spikes, CRT Trace, Retro Stack, Vector Round, Vector Square.
- *Iconic Runners:* Iconic Tortoise, Iconic Fish.
- *Sprite Characters:* Cat, Frog, Boy, Cane Man, Orange Cat, Chill, Dino, Dog, Fox, Girl, Red Hat, Stickman, Dancing Mouse.

**Canvas & Aspect Ratios:**

| Format | Use |
|--------|-----|
| 9:16 Vertical | Instagram Stories, TikTok, Reels |
| 1:1 Square | Instagram/Facebook feed, chat previews |
| 16:9 Landscape | YouTube, LinkedIn, presentations |

**Canvas Elements:** Header · Subheader · Caption · Visualiser · Imported Media

All elements support drag (move), pinch (resize), and twist (rotate). Pinch a visualiser outward to snap it to full canvas width. Double tap any element to reset to default position and size. When an element is at full width, drag is locked to the Y-axis only.

**Background Options:**

- **Solid colour** — Any hex value.
- **User photo/video** — Import from Photos or paste from Clipboard (long press background icon). Includes a Gaussian blur slider.
- **AI Backgrounds** *(iPhone 15 Pro+)* — The transcript or title text is passed to a local LLM and generates an image via ImagePlayground. Runs entirely on-device. No text or images are transmitted externally.

**Typography:** System · Rounded · Serif · Mono — with customisable weights and alignment (left / centre / right).

*Gesture: Long press any title or subtitle element to open a quick-edit text alert.*

**Timeline Controls:**

- **Zoom:** Pinch gesture, 0.5× to 50× magnification.
- **Fit to screen:** Button to reset zoom and show the full clip.
- **Scrub / seek:** Drag the playhead to any position.
- **Loop toggle:** Loops the current selection during playback.
- **Auto-Trim:** On load, analyses the global waveform and automatically sets trim handles to skip silence at the start and end (threshold: <5% amplitude).
- **Double tap duration:** Snaps selection to maximum allowed duration from current start handle.
- **Double tap start/end handle:** Jumps playhead to that clip boundary.
- **Long press timestamp:** Snaps the nearest handle to the current playhead position.
- **Single tap ruler:** Quick seek to that timestamp.

---

### 4. Transcription

On-device speech recognition using Apple's native framework. Transcription starts automatically when a recording is opened in the editor.

- **Caption modes:** Word-by-word or sentence captions.
- **Split:** Long caption sentences can be split at any word boundary.
- **Orphan Fixer:** Leading punctuation (periods, commas) is automatically moved from the start of a segment to the end of the previous segment.
- **Editing:** Edit any segment's text directly, adjust timing, search & replace (single or all occurrences), undo/redo.
- **Import:** `.srt` or `.vtt` files replace the current transcript entirely.
- **Export:** `.srt` subtitle file, raw audio file, or plain text transcript.

---

### 5. Social Audio Normalisation *(Lappaa Pro)*

Measures integrated loudness (LUFS) and True Peak, then normalises to a user-selected target before export. Designed for social media feeds — not a lossless studio mastering suite.

**LUFS target range:** -23 to -14, user-adjustable.

| Platform | Target | Notes |
|----------|--------|-------|
| Instagram Reels | -14 to -16 LUFS | Prevents algorithmic volume ducking |
| TikTok | -13 to -14 LUFS | Competitive loudness for mobile speakers |
| YouTube Shorts | -13 to -14 LUFS | Normalised to this target on upload |
| Podcast / voice | -23 LUFS | EBU R128 broadcast standard |

---

## Draft Lifecycle

Lappaa manages local storage automatically. Any draft can be manually deleted at any time.

| Draft State | Auto-Delete | Notes |
|-------------|-------------|-------|
| Active | After 7 days (configurable) | Working sessions |
| Active (versioned) | When exceeding 5 versions | — |
| Exported | After 30 days (configurable) | Marked after any export |
| Exported (versioned) | When exceeding 10 versions | — |
| Archived | Never | Protected from all cleanup |

---

## Gestures Reference

| View | Gesture | Outcome |
|------|---------|---------|
| Recorder | Long press visualiser | Opens style picker |
| Recorder | Long press Import button | Opens import source dialog (Files / Photos / Clipboard) |
| Recorder | Long press timer | Opens timer style picker |
| Recorder | Double tap timer | Toggles timer visibility (Hidden ↔ last active style) |
| Editor canvas | Pinch element | Resizes the element |
| Editor canvas | Pinch visualiser outward | Snaps visualiser to 100% canvas width |
| Editor canvas | Double tap element | Resets to default position and size |
| Editor canvas | Vertical drag (full-width element) | Locked to Y-axis |
| Editor canvas | Long press background icon | Pastes image from system clipboard |
| Editor canvas | Long press title / subtitle | Opens quick-edit text alert |
| Editor canvas | Twist element | Rotates the element |
| Timeline | Single tap ruler | Quick seek to timestamp |
| Timeline | Double tap duration | Snaps selection to max duration from current start |
| Timeline | Double tap start/end handle | Jumps playhead to clip boundary |
| Timeline | Long press timestamp | Snaps nearest handle to playhead position |
| Template row | Double tap | Toggles as default template for its aspect ratio |

---

## Privacy & System Requirements

**Privacy:** All processing is local. No audio, transcripts, or images leave the device. See `PRIVACY.md` for the full policy.

**System Requirements:**

- iOS 26.0+ / iPadOS 26.0+
- Microphone / camera permission — required for recording
- Speech Recognition permission — required for transcription
- Photo Library ("Add Only") — required to save exported videos
- Photo Library (Read) — required for media import *(Pro)*
- Notifications — optional, used for Live Activities

Apple Intelligence features (AI Backgrounds): iPhone 15 Pro / iPhone 15 Pro Max or newer, iOS 26+.

---

## Developer

**Petri Kajander (Sunbird OÜ)** — independent European developer, bootstrapped.

Same developer as:
- [Nuotit](https://nuotit.org) — Podcast player for iOS and iPadOS.
- [Nootti](https://nootti.com) — Cross-posting to Bluesky, Mastodon, Nostr.

**Links:**
- Website: [lappaa.com](https://lappaa.com)
- Support: `SUPPORT.md`
- Privacy: `PRIVACY.md`
