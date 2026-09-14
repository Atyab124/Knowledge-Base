---
name: "YouTube Realtime Captions (Translated)"
status: "shipped"
github: "https://github.com/Atyab124/Youtube-Transcription-Extension"
---

# YouTube Realtime Captions (Translated)

- What it is: Chrome extension + local Node backend that overlays realtime translated captions on any YouTube video, reels-style
- Role: solo build
- Stack: Chrome MV3 extension (offscreen audio capture, service worker, content-script overlay), Node.js/TypeScript WebSocket backend, OpenAI Realtime API for transcription, GPT-4o-mini for translation (English/Hindi)
- Notable: captures tab audio via `tabCapture`, resamples to 24kHz mono PCM16 via an audio worklet, streams over WebSocket to a local backend — no cloud hosting required; includes its own smoke test script
- Real numbers: —
