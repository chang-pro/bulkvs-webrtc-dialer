# BulkVS WebRTC Dialer & SMS Dashboard

![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-Voice_SDK-333333?style=flat-square)
![Twilio](https://img.shields.io/badge/Twilio-Voice-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Repo](https://img.shields.io/badge/Source-Private-orange?style=flat-square)

**I built a second dialer platform using BulkVS telephony — a full WebRTC softphone with DTMF support, visual dialpad, and mass SMS.** This was my proving ground before building the larger Twilio platform and Ringora.

---

## Why I Built Two Dialers

I built this one first to learn the hard parts of browser-based telephony — WebRTC audio streams, DTMF tone handling, call state management. Once I had this working, I had the foundation to build the more complex Twilio platform and eventually Ringora's full power dialer.

## What I Built

### Full WebRTC Softphone
- **In-browser calling** via Twilio Voice SDK — no phone, no plugins, just a browser and a mic
- **Visual dialpad** (0–9, *, #) that feels like a real phone
- **Real-time call status** tracking: Connecting → Ringing → In Call → Ended
- **Mute/unmute** toggle during active calls
- **DTMF keypad** — send touch-tones during calls for IVR navigation, conference PINs, and voicemail systems. This was the hardest part — you need to send tones both to the remote party AND play them locally for user feedback.

### SMS Dashboard
- **Single SMS** with character count (160 chars = 1 segment)
- **Mass SMS** from CSV uploads with real-time progress bar
- Preview data before sending, detailed results after
- Delivery status tracking per message

## Tech Stack

`Next.js` · `TypeScript` · `Twilio Voice SDK` · `WebRTC` · `BulkVS` · `React`

---

> *Closed source. This was my learning project for telephony — the concepts here evolved into the Twilio Platform and Ringora.*
