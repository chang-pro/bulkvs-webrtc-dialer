# BulkVS WebRTC Dialer & SMS Dashboard

![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-Voice_SDK-333333?style=flat-square)
![Twilio](https://img.shields.io/badge/Twilio-Voice-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Repo](https://img.shields.io/badge/Source-Private-orange?style=flat-square)

**A full-featured WebRTC softphone and SMS dashboard built with BulkVS telephony and Twilio Voice SDK.** Features in-browser calling, a visual dialpad, DTMF support, and mass SMS broadcasting.

---

## Features

### WebRTC Softphone
- Full in-browser calling — no phone hardware needed
- Visual dialpad (0–9, *, #) with real-time call status
- Mute/unmute during active calls
- DTMF keypad for sending tones (IVR navigation, conference PINs)
- Clean call controls with status indicators (Connecting → Ringing → In Call)

### SMS Dashboard
- **Single SMS** — Send individual messages with character count (160 max)
- **Mass SMS** — CSV upload for bulk broadcasting with progress bar
- Preview data before sending
- Delivery results summary with success/failure breakdown

## Architecture

```
┌────────────────────────────────────────┐
│          Next.js Frontend               │
│   Softphone │ Dialpad │ SMS Dashboard   │
│        Twilio Voice SDK (WebRTC)        │
└──────────────────┬─────────────────────┘
                   │
          ┌────────┼────────┐
          ▼        ▼        ▼
    ┌──────────┐ ┌──────┐ ┌──────────┐
    │ Voice    │ │ SMS  │ │ BulkVS   │
    │ Token    │ │ API  │ │ Telephony│
    │ Endpoint │ │      │ │          │
    └──────────┘ └──────┘ └──────────┘
```

## Tech Stack

- **Framework:** Next.js, React, TypeScript
- **Voice:** Twilio Voice SDK (WebRTC), BulkVS telephony
- **SMS:** Twilio Programmable Messaging
- **UI:** Real-time status updates, progress tracking

## Skills Demonstrated

- WebRTC implementation for browser-based telephony
- Twilio Voice SDK client-side integration
- DTMF tone handling during active calls
- CSV parsing and bulk operation management
- Real-time progress tracking UI

---

> *This is a showcase page for a private repository. Source code available upon request for verified opportunities.*
