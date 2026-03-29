# 🚀 ET Pulse — AI-Native News Intelligence System

ET Pulse is an AI-native news platform that transforms traditional article-based consumption into **interactive, personalized intelligence briefings**.

Instead of reading multiple articles, users:

* Understand news in seconds
* Explore deeper insights
* Ask follow-up questions

---

## 🎯 Problem

Business news is still consumed like it's 2005:

* Static articles
* One-size-fits-all feeds
* High time investment (15–20 mins/day)

---

## 💡 Solution

ET Pulse replaces reading with understanding through:

* ⚡ **Understand in 30s** → Quick AI summary of an article
* 🧠 **AI Briefing** → Multi-article synthesis with structured insights
* 💬 **Ask AI** → Context-aware chat with follow-up exploration
* 🌐 **Vernacular Engine** → Contextual language adaptation

---

## 🧩 Core Features

### 1. Personalized Feed

* Based on interests, user type, and language
* AI-first discovery (not article-first)

### 2. Two-Layer AI System

* Quick → Speed (Understand in 30s)
* Deep → Decision-making (AI Briefing)

### 3. Interactive Chat

* Context-aware conversations
* Linked to briefings

### 4. Vernacular Intelligence

* Native language generation (not translation)

---

## 🏗️ Tech Stack

### Frontend

* React (Vite)
* Tailwind CSS

### Backend

* Node.js / Express

### AI Layer

* OpenRouter API
* Gemini 2.0 Flash

### Data Sources

* ET RSS Feeds (Primary)
* GNews API (Fallback)

### Storage (MVP)

* localStorage (user profile & state)

---

## 🧠 Architecture Overview

* Multi-agent system:

  * Data Agent
  * Personalization Agent
  * Briefing Agent
  * Chat Agent
  * Vernacular Agent

* Central orchestrator handles all API calls

* Structured JSON outputs with retry logic

---

## 🔄 User Flow

Home Feed
→ Open Article (original content)
→ Click "Understand in 30s"
→ Expand to AI Briefing
→ Click follow-up question
→ Chat (context-aware)
→ Saved in Profile

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/et-pulse.git
cd et-pulse
```

---

### 2. Install dependencies

#### Frontend

```bash
cd client
npm install
```

#### Backend

```bash
cd server
npm install
```

---

### 3. Setup environment variables

Create `.env` in server:

```env
OPENROUTER_API_KEY=your_api_key_here
```

---

### 4. Run the app

#### Start backend

```bash
cd server
npm run dev
```

#### Start frontend

```bash
cd client
npm run dev
```

---

### 5. Open in browser

```
http://localhost:5173
```

---

## 🔌 API Endpoints

| Endpoint                | Description               |
| ----------------------- | ------------------------- |
| GET /news               | Fetch latest articles     |
| POST /generate-summary  | Quick summary             |
| POST /generate-briefing | Multi-article AI briefing |
| POST /chat              | Context-aware chat        |
| POST /translate         | Vernacular processing     |

---

## ⚡ Key Design Decisions

* AI is **on-demand**, not forced
* Original articles are always visible (trust-first UX)
* Two-layer AI system for clarity + depth
* No database for MVP → fast + hackathon-friendly

---

## 📊 Impact

* ⏱️ 75% reduction in news consumption time
* 📈 Higher engagement & retention
* 🌍 Vernacular access for wider audience

---

## 🏆 Built for

ET Hackathon — Problem Statement 8
**AI-Native News Experience**

---

## 👨‍💻 Team

* Shahil Choudhary(Nichirin Blade)

---

## 🚀 Future Improvements

* Database integration (MongoDB / Firebase)
* Real-time personalization engine
* Multi-model AI routing
* Push notifications for AI briefings


### 🚀 Quick Start Guide (One-Click)

The easiest way to get started is using the provided batch scripts:

1.  **Setup**: Run `setup.bat`. This will install all dependencies for both the frontend and backend and set up your `.env` files.
2.  **Launch**: Run `start-app.bat`. This will automatically launch both the **Backend (Port 3001)** and the **Frontend (Port 5173)** in two separate windows.

---

### 🛠️ Manual Execution (Alternative)

If you prefer using the terminal manually, follow these steps:

#### 1. Installation
Run `npm run install-all` from the root directory to install both frontend and backend dependencies.

#### 2. Running
You must run **both** services simultaneously:
- **Backend**: `npm run server` (starts the Express API on port 3001).
- **Frontend**: `npm run dev` (starts the Vite React app on port 5173).

---

## 🛠️ Project Structure
- `/src`: Frontend React application (Vite).
- `/server`: Node.js Express backend.
- `/server/services`: AI logic (Gemini/OpenRouter) and News services.
- `/public`: Static assets and icons.

## 🤖 AI Features
- **Understand in 30s**: Instant AI briefings for your top sectors.
- **Analyze with AI**: Deep-dive breakthroughs for specific news articles.
- **Pulse AI Chat**: Context-aware assistant for follow-up questions.
- **Vernacular Support**: Full UI and AI translation for Hindi, Tamil, Telugu, Bengali, and Marathi.

## ❓ Troubleshooting
- **401 Unauthorized**: Ensure your `OPENROUTER_API_KEY` is correct in both the root `.env` and `/server/.env`.
- **Port 3001 Busy**: If the backend fails to start, ensure no other process is using port 3001.
- **Stuck Loading**: Check the browser console and `server` terminal for AI generation timeouts.

---

## 📦 How to Zip and Share
When sharing this project via ZIP, please **exclude** the following folders to keep the file size manageable:
- `node_modules` (in both the root and the `server` folder)
- `dist` (frontend build output if present)
- `.git` (if initialized)

The recipient should run `setup.bat` immediately after unzipping to restore these dependencies.

