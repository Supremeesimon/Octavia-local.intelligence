
# 🌒 Octavia LocalIntel

**“Built for Developers” — Prospect smarter, not harder.**

Octavia LocalIntel is a dark-themed, AI-powered web application that helps developers discover local businesses that need digital help—like those with no websites or poor online ratings. Identify leads, visualize data, and export outreach-ready business lists with ease.

---
<img width="1672" alt="Screenshot 2025-04-08 at 8 23 08 PM" src="https://github.com/user-attachments/assets/0ae368ab-7ebc-4d15-924c-85af3963257d" />
<img width="1680" alt="Screenshot 2025-04-08 at 8 23 22 PM" src="https://github.com/user-attachments/assets/ee30254d-e307-41cf-998e-ce4c03013b61" />
<img width="1680" alt="Screenshot 2025-04-08 at 8 23 32 PM" src="https://github.com/user-attachments/assets/88513c81-2b2d-40b8-b765-f99723478e09" />
<img width="1680" alt="Screenshot 2025-04-08 at 8 23 43 PM" src="https://github.com/user-attachments/assets/7e49cd88-9b0e-4120-a6e4-2ba866cb9dd3" />
<img width="1680" alt="Screenshot 2025-04-08 at 8 23 50 PM" src="https://github.com/user-attachments/assets/b1cbda30-6f4f-4685-8775-565042e29911" />









🧠 Python-Powered Backend
Octavia's backend is heavily powered by Python, designed for clean API routing, AI integration, secure auth, and smart data processing.

📂 Backend File Structure (Key Files)
File	Purpose
backend/main.py	Initializes the FastAPI app, sets up routers, and configures Firebase Auth

backend/app/auth/__init__.py	Initializes auth module and exposes AuthorizedUser, User classes

backend/app/auth/user.py	Defines User models used across requests and JWT parsing

backend/databutton_app/mw/auth_mw.py	Middleware to validate Firebase JWT tokens and extract user info

backend/databutton_app/mw/__init__.py	Initializes the middleware module

backend/app/apis/business_analysis/__init__.py	Logic for analyzing business opportunity data from Serper (scores leads)

backend/app/apis/gemini/__init__.py	Handles Gemini API communication and user prompts

backend/app/apis/serper/__init__.py	Handles Serper API search queries and formats response data


✅ Modular routes

✅ Secure auth middleware

✅ AI and data integrations

✅ Production-ready with FastAPI



## 🚀 Features

- 🔍 Find businesses by location, category, and rating
- 🌐 Prioritize those without websites or with low Google ratings
- 💬 Chat-powered interface using Gemini for smart filtering and queries
- 📊 Real-time visualizations (charts, maps, tables)
- 🎨 Dark-mode, noir-style interface built with Tailwind CSS
- 📦 Export filtered business data as CSV/Excel
- 🤖 AI-assisted analysis with smooth split-screen UX

---

## 🧱 Tech Stack

### Frontend
- `React` + `TypeScript`
- `Tailwind CSS` (dark mode default)
- `Framer Motion` for animations
- `Gemini API` for chat interface

### Backend
- `Python` with `FastAPI`
- `Pandas`, `NumPy` for data processing
- `Matplotlib`, `Seaborn`, `Plotly` (dark theme)
- `Serper API` for business data (Google Maps wrapper)

---




cd frontend
npm install
npm run dev

cd backend
pip install -r requirements.txt
uvicorn main:app --reload

###Environment Variables
Create a .env file in the root of each project directory (frontend and backend).

Frontend:

ini
Copy
Edit
VITE_GEMINI_API_KEY=your_gemini_api_key
Backend:

ini
Copy
Edit
SERPER_API_KEY=your_serper_api_key


🎯 Usage
Login or register

Enter a target location (e.g., "Calgary") and optional category

Ask Gemini things like:

"Show me dentists in Calgary with no websites"

"Filter by businesses with ratings below 3.0"

Watch the canvas slide in and data visualizations appear

Export filtered results for cold outreach or lead generation

📦 Export Formats
.csv and .xlsx exports available

Includes: business name, address, contact info, website (if any), rating, hours

✨ Coming Soon
🔐 Auth + account-based usage tracking

📊 Custom lead scoring model

📞 One-click outreach (email/call tools)

📍 Multi-location comparison heatmaps

🧠 Predictive analytics using Gemini AI

🧠 Contributing
Pull requests and issues are welcome!

Fork the repo

Create your feature branch: git checkout -b feature/awesome-feature

Commit your changes: git commit -am 'Add cool feature'

Push to the branch: git push origin feature/awesome-feature

Create a PR ✅

📄 License
MIT — free to use, adapt, and build upon.

🙌 Credits
Built by Simon

Powered by Gemini, Serper, React, and Python

Inspired by real developer pain points and local lead gen strategies



