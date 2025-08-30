<div align="center">

# 🐾 Meyme – Your AI Cat Companion  

<img src="assets/banner.png" alt="Meyme Banner" width="700">  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)  
![FastAPI](https://img.shields.io/badge/FastAPI-Framework-success?logo=fastapi)  
![MurfAI](https://img.shields.io/badge/30%20Days%20Voice%20Agents%20Challenge-Day%2029-orange)  
![License](https://img.shields.io/badge/License-MIT-lightgrey)  

**An intelligent, voice-driven AI cat agent that listens, understands, and responds with feline charm.**  
_Built as part of the **30 Days of AI Voice Agents Challenge by Murf AI (completed up to Day 29/30)**._  

---

<img src="https://media.giphy.com/media/3oriO0OEd9QIDdllqo/giphy.gif" width="300" alt="Meyme Cat Agent">

</div>

---

## 🐱 About Meyme

**Meyme (Meowy – the AI Cat Agent)** is a playful, conversational AI that listens to voice commands, responds in real-time, and adds personality to conversations.  

---

## ✨ Key Features

- 🎙️ **Real-time voice streaming**  
- 📝 **Live transcription (STT)**  
- 🔄 **Turn detection** for natural conversations  
- 🧠 **AI-powered replies** using LLMs (Gemini/OpenAI/etc.)  
- 😺 **Cat-like persona** with meows & playful style  
- 🌦️ **Weather updates** (OpenWeather API)  
- 🔍 **Web search/trip ideas** (Tavily API)  
- 💬 **Session memory** (per conversation)  
- 🎨 **Frontend UI** (responsive & modern)  
- 🚀 **One-app deployment** (backend + frontend)  

---

## 🛠️ Tech Stack

- **Backend**: Python 3, FastAPI  
- **Frontend**: HTML5, JavaScript, Tailwind CSS  
- **Templates**: Jinja2  
- **Speech-to-Text**: AssemblyAI (or alternative)  
- **Text-to-Speech**: Murf AI  
- **AI Model**: Gemini / OpenAI / Anthropic  
- **Web Search**: Tavily API  
- **Weather Data**: OpenWeather API  
- **Architecture**: WebSockets (streaming), REST (tools)  
- **Env Management**: `.env` for API keys  

---

## ⚡ Getting Started

### Prerequisites
- Python 3.8+  
- API keys for:
  - STT (AssemblyAI or similar)  
  - TTS (Murf AI)  
  - LLM (Gemini / OpenAI)  
  - Weather (OpenWeather)  
  - Web Search (Tavily)


## 📂 Project Structure

meyme-ai-cat-agent/
├── backend/
│   ├── controllers/
│   │   ├── websocket_controller.py       # Voice streaming
│   │   └── agent_controller.py           # Main agent logic
│   ├── services/
│   │   ├── stt_service.py                # Speech-to-Text
│   │   ├── tts_service.py                # Text-to-Speech
│   │   └── llm_service.py                # AI Model
│   ├── tools/
│   │   ├── weather_tool.py               # Weather info
│   │   └── web_search_tool.py            # Web search
│   ├── templates/
│   │   └── index.html                    # Frontend UI
│   ├── static/
│   │   ├── css/
│   │   └── js/
│   ├── main.py                           # FastAPI app
│   └── requirements.txt
└── README.md

## 🎮 Usage

Speak into the mic → Meyme listens, transcribes & replies.

Responses include voice + on-screen text.

Ask about weather, trips, or random info.

Switch Meyme’s persona (playful, wise, pirate cat 🏴‍☠️).

## 🚀 Deployment

1. Add your API keys to .env.
2. Deploy using uvicorn / Gunicorn with ASGI workers.
3. Use Docker for easy deployment.
4. Configure HTTPS with Nginx / Render / Heroku.

## 🗺️ Roadmap

🐾 More cat voices & personalities

📝 Persistent user profiles & chat history

🎲 Fun tools (jokes, trivia, translator, math solver)

🔒 Privacy-first (on-device models)

📱 Mobile-friendly voice-only version

🌍 Easy deployment via Streamlit/Flask

## 🤝 Contributing

1. Fork the repo.
2. Create a branch: git checkout -b feature/amazing-update
3. Commit & push changes.
4. Open a Pull Request.

Let’s make Meyme the best AI cat companion 🐈✨

 ## 📜 License

MIT License – free to use, adapt, and share.

## 🐾 Summary

Meyme is your friendly AI-powered cat companion—built with love during the Murf AI 30-Day Voice Agent Challenge (up to Day 29).
She listens, thinks, and meows back with charm, smarts, and personality.

😺 Not just an AI… a cat that talks back! 

### Installation

```bash
# Clone repo
git clone https://github.com/code-with-parth/meyme-ai-cat-agent.git

# Enter backend
cd backend

# Setup virtual environment
python3 -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Run server
uvicorn main:app --host 0.0.0.0 --port 8000 --reload
