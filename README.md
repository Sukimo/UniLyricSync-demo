# UniLyricSync Demo
Demo project for [UniLyricSync](https://github.com/Sukimo/UniLyricSync) — karaoke-style word highlight tool for Unity 6

---

## Requirements

- Unity 6.0+
- TextMeshPro (bundled with Unity 6 via com.unity.ugui)
- UniLyricSync package

---

## How to Run

1. Clone this repo
2. Open project in Unity 6
3. Open `Assets/Demo/Scenes/UniLyricDemo.unity`
4. Press Play

---

## Demo Samples

### Sample 1 — Words light up
**Effect:** Color Only

Short 3-word phrase showing clean word-by-word highlight in sync with audio. The simplest use case — each word lights up exactly on beat.

---

### Sample 2 — Feel the beat now
**Effect:** Wave + Color

5 words with sine-wave bounce effect per character. Shows the juicy side of UniLyricSync for energetic or music-driven content.

---

### Sample 3 — Every word comes alive when the music plays
**Effect:** Scale + Color

Full sentence demonstrating natural reading pace sync. Each word scales up slightly on activation then returns to normal.

---

### Sample 4 — Sync your story one word at a time
**Effect:** Color Only + Per-word Override Color

Each word uses a different highlight color via the override color feature on individual markers. Shows how to create visual variety without changing the effect type.

---

### Sample 5 — UniLyricSync lets you place triggers on a timeline and highlight each word as the audio plays in your Unity game
**Effect:** Color Only

Long sentence stress test. Shows word wrap handling, timing accuracy across a longer clip, and that the tool stays stable with higher word counts.

---

## UI Controls

The demo includes a floating panel in the top-left corner built with UI Toolkit

| Control | Description |
|---------|-------------|
| Play / Pause / Stop | Playback controls |
| Loop | Toggle loop on the current clip |
| Effect | Switch between Color Only, Scale + Color, Wave + Color |
| Transition | Control how fast the colour lerp animates |
| Scale Amount / Speed | Tune the scale pop effect |
| Wave Amp / Speed / Spread | Tune the wave bounce effect |
| Catalog | Click any row to load that lyric data |

All slider changes apply in real time without modifying the original asset files

---

## Project Structure

```
Assets/
├── Demo/
│   ├── Scenes/
│   │   └── UniLyricDemo.unity
│   ├── Audio/
│   │   ├── 01. Words light up.mp3
│   │   ├── 02. Feel the beat.mp3
│   │   ├── 03. Every word.mp3
│   │   ├── 04. Sync your story.mp3
│   │   └── 05. Long sentence.mp3
│   ├── LyricData/
│   │   ├── Sample01.asset
│   │   ├── Sample02.asset
│   │   ├── Sample03.asset
│   │   ├── Sample04.asset
│   │   └── Sample05.asset
│   └── UI/
│       ├── UniLyricDemo.uxml
│       ├── UniLyricDemo.uss
├──     ├── UniLyricPanel.asset
│       └── UniLyricUIController.cs
└── UniLyricSync/
    ├── Editor/
    └── Runtime/
```

---

## Credits

Voice: [ElevenLabs](https://elevenlabs.io) AI Text-to-Speech

---

## Related

- [UniLyricSync](https://github.com/yourname/UniLyricSync) — the tool package
- MIT License
