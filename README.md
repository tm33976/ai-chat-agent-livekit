# AI Chat Agent – LiveKit + Next.js + Python

This project demonstrates a **real-time conversational AI chat agent** built using **LiveKit’s Agents SDK** and a **React (Next.js)** frontend.  
It enables two-way chat communication via **WebRTC data channels**, eliminating the need for traditional HTTP streaming.  



---

## 🚀 Project Overview

This project is divided into two major parts:

1. **Server (Python Agent)**  
   - Implements a Python-based AI Agent using LiveKit’s SDK.  
   - Handles real-time communication between frontend and backend.  
   - Can be extended to integrate with Django or LLMs for smarter AI responses.

2. **Client (Next.js Frontend)**  
   - Provides a clean and responsive chat interface.  
   - Connects to the agent in real-time via LiveKit Data Channels.  
   

---

## 🛠️ Tech Stack

- **Backend:** Python, LiveKit Agents SDK  
- **Frontend:** React (Next.js), TailwindCSS  
- **Communication:** LiveKit Data Channels (WebRTC)  
- **Environment:** Node.js, PNPM, Virtualenv  

---

## ⚙️ Setup Instructions

### 1️⃣ Run the Python Agent

```bash
cd server
cp .env.example .env
# Populate real values in .env (API keys, room info, etc.)
python -m venv .venv
source .venv/bin/activate   # (use .venv\Scripts\activate on Windows)
pip install -r requirements.txt
python agent.py start
```

---

### 2️⃣ Run the Next.js App

> 💡 Note: If you encounter PNPM version issues, run this command first:
> ```bash
> export COREPACK_ENABLE_STRICT=0
> ```

```bash
cd client
cp .env.example .env.local
# Populate real values in .env.local
pnpm install
pnpm dev
```

Then, open your browser and navigate to:  
👉 [http://localhost:3000](http://localhost:3000)

---

## 🧩 Future Enhancements

- Integrate **Django REST Framework** for user management and chat history.
- Add **voice input/output** using STT (Speech-to-Text) and TTS (Text-to-Speech).
- Deploy to **AWS or Vercel** for public access.
- Connect with **OpenAI API** for advanced conversational logic.

---

## 📄 Author

👨‍💻 **Tushar Mishra**  
Full Stack Developer | AI Enthusiast  
📧 tm3390782@gmail.com  
🌐 [Portfolio](https://tushar-mishra-cse-portfolio.vercel.app) | [GitHub](https://github.com/tm33976) | [LinkedIn](https://www.linkedin.com/in/tushar-mishra-5253ab311/)

---

