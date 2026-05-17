# Debate Chess Clock

An AI-powered debate timing and analytics platform. Like a chess clock, but for structured discussions.

---

## What is Debate Chess Clock?

Debate Chess Clock manages speaking time, tracks debate flow, and generates real-time conversational insights during structured debates and discussions. It combines the simplicity of a chess clock with live transcription, AI analysis, and post-debate review tools.

---

## Features

- Real-time speaker timers with automatic synchronization as speakers switch
- Voice differentiation that identifies active participants without manual input
- AI transcription and summarization that generates searchable debate records and extracts key points
- Action item extraction that automatically surfaces decisions and follow-ups
- Interruption tracking that monitors and flags interruptions during sessions
- Sentiment analysis that tracks conversational tone throughout the debate
- Post-debate analytics with full session review and speaker breakdowns

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | SvelteKit, TypeScript |
| Real-time | WebSockets |
| Audio/ML | TensorFlow.js, Web Audio API |
| Backend | Node.js, Python, REST APIs |
| Database | PostgreSQL |
| Infrastructure | AWS, Cloudflare, Railway |

---

## Getting Started

```bash
git clone https://github.com/Arminderf-Singh/Debate-Chess-Clock.git
cd Debate-Chess-Clock
npm install
npm run dev
```

The AI transcription pipeline requires a Python backend. See `/backend/README.md` for setup instructions.

---

## Architecture Overview

```
Client (SvelteKit)
  └── WebSocket connection -> Node.js server
        ├── Speaker detection (TensorFlow.js + Web Audio API)
        ├── Timer sync engine
        └── Python AI pipeline
              ├── Transcription
              ├── Summarization
              └── Sentiment analysis -> PostgreSQL
```

---

## Use Cases

- Competitive debate tournaments
- Team meetings and stand-ups
- Panel discussions and interviews
- Educational debate practice

---

## License

MIT
