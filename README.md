# AI Voice Agent Interview Platform

An interactive web application that simulates job interviews using AI-powered voice conversations.  
Built with **Next.js**, this platform delivers a realistic interview experience through real-time voice interaction, AI-generated questions, and instant feedback.

---

## Author

**Aman Singh** – Full Stack Developer

---

## Features

- 🎙️ Voice-based interaction with an AI interviewer
- 🤖 Natural language processing for dynamic question & answer flow
- ⏯️ Pause/Resume interview functionality
- 📊 Track interview progress and stages
- 🔄 Real-time feedback on responses
- 🎯 Customized follow-up questions based on your answers
- 🛡️ Built-in rate limiting for API security
- ♿ Accessibility-first design following WCAG guidelines

---

## Accessibility Features

### Keyboard Navigation
- Full keyboard support for all interactive elements
- Visible focus indicators & logical tab order

### Screen Reader Support
- Semantic HTML with ARIA landmarks
- Descriptive ARIA labels
- Live regions for dynamic updates
- Status announcements for progress, recording states, AI responses, and errors

### Audio Interface
- Play/Pause controls for AI voice responses
- Visual indicators synced with audio
- Alternative text for all audio controls

### Visual Accessibility
- High contrast color scheme
- Clear layout and spacing
- Status indicators for recording, interview progress, and system status

---

## Tech Stack

- **Framework**: Next.js 14
- **Frontend**: React, TailwindCSS
- **AI Services**:
  - OpenAI GPT-4 for interview logic
  - Deepgram for Speech-to-Text and Text-to-Speech
- **State Management**: React Context API
- **API Protection**: In-memory rate limiting
- **Styling**: TailwindCSS with custom animations

---

## Getting Started

1. **Clone this repository**
   ```bash
   git clone https://github.com/amansingh2426/ai-voice-agent-interview.git
   cd ai-voice-agent-interview
Install dependencies

bash
Copy
Edit
npm install
# or
yarn install
Set up environment variables
Create .env.local in the root folder:

env
Copy
Edit
OPENAI_API_KEY=your_openai_api_key
DEEPGRAM_API_KEY=your_deepgram_api_key

RATE_LIMIT_POINTS=10
RATE_LIMIT_DURATION=1
RATE_LIMIT_BLOCK_DURATION=60
Run locally

bash
Copy
Edit
npm run dev
# or
yarn dev
Visit: http://localhost:3000

API Rate Limiting
10 requests per second per client

60-second block when exceeded

Applies to all API endpoints:

Speech-to-Text conversion

AI response generation

Text-to-Speech synthesis
