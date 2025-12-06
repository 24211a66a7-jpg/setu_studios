# 🌈 Setu Studios - Build Ideas, Fast & Beautiful

<p align="center">
  <a href="https://setustudios.vercel.app/" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/🔗_Live_Demo-setustudios.vercel.app-brightgreen?style=for-the-badge" alt="Live Demo" />
  </a>
  <br/>
  <img src="https://img.shields.io/badge/React-18-blue?logo=react&style=for-the-badge" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Supabase-Postgres-3ECF8E?logo=supabase&style=for-the-badge" />
  <img src="https://img.shields.io/badge/AI-Gemini%2FOpenAI-purple?logo=google&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Hosting-Vercel-black?logo=vercel&style=for-the-badge" />
</p>

---

## 🎨 What is Setu Studios?

**Setu Studios** is your creative launchpad for turning ideas into reality. Whether you're a founder, maker, or team, Setu Studios helps you brainstorm, analyze, and package new products and services - all in a beautiful, fast, and secure app.

| Benefit                | Description                                                      |
|------------------------|------------------------------------------------------------------|
| 🚀 Instant Ideation    | Capture and refine ideas in seconds                               |
| 🤖 AI Analysis         | Get smart feedback and suggestions                               |
| 📦 Service Packaging   | Bundle offerings, manage carts, and process orders               |
| 🔒 Secure & Private    | Data protected with Supabase RLS                                 |
| ✉️ Notifications       | Stay updated with EmailJS                                        |

---

## 🌟 Why Setu Studios is Useful

| Reason         | How it Helps You                           |
|----------------|--------------------------------------------|
| Speed          | Go from idea to prototype in minutes        |
| Clarity        | AI highlights strengths, gaps, next steps   |
| Collaboration  | Share, edit, and package ideas with team    |
| Automation     | Order flows, notifications, analysis built-in|
| Security       | Sensitive keys and data are protected       |

---

## 🖼️ Flowchart: How It Works

```mermaid
flowchart TD
  A["💡 Idea Entry"]
  B["🤖 AI Analyzer"]
  C["📦 Package Builder"]
  D["🛒 Cart & Orders"]
  E["🔔 Email Notifications"]
  F["🔒 Supabase Auth & DB"]
  G["🛠️ Admin Dashboard"]

  A --> B
  B --> C
  C --> D
  D --> E
  A --> F
  B --> F
  C --> F
  D --> F
  F -.-> G
```

---

## 🏗️ Architecture Diagram

```mermaid
graph LR
  FE["Frontend (React)"] -- "API / DB" --> SB["Supabase"]
  FE -- "LLM Proxy" --> PX["Serverless Proxy"]
  PX -- "Gemini / OpenAI" --> LLM["LLM Provider"]
  FE -- "Email" --> EM["EmailJS"]
  SB -- "Realtime / Storage" --> DB[(Postgres DB)]
```

---

## 🔄 Workflow Table

| Step                | Action                                  | Result                        |
|---------------------|-----------------------------------------|-------------------------------|
| 1. Idea Entry       | User submits idea                       | Saved to Supabase DB          |
| 2. AI Analysis      | Idea sent to Gemini/OpenAI via Proxy    | Feedback returned to user     |
| 3. Package Builder  | User bundles services/products          | Cart updated                  |
| 4. Order/Checkout   | User places order                       | Order saved, email sent       |
| 5. Admin Dashboard  | Admin reviews orders/ideas              | Management & analytics        |

---

## 🛠️ Tech Stack

| Layer         | Technology                        |
|---------------|-----------------------------------|
| Frontend      | React 18, TypeScript, Vite        |
| Styling       | Tailwind CSS, Framer Motion       |
| Backend/BaaS  | Supabase (Postgres, Auth)         |
| Email         | EmailJS                           |
| AI/LLM        | Gemini / OpenAI (serverless proxy)|
| Hosting       | Vercel                            |

---

## 🌈 Features

| Feature                | Description                                      |
|------------------------|--------------------------------------------------|
| ✨ Idea Management      | Create, edit, and categorize ideas               |
| 🤖 AI Analyzer         | Get instant feedback and suggestions             |
| 📦 Packages & Cart     | Bundle services, manage cart, process orders     |
| 🛒 Order Notifications | Email updates for orders and activity            |
| 🔒 Authentication      | Secure login and data with Supabase              |

---

## 🆚 Feature Comparison Table

| Feature           | Setu Studios | Typical Idea App |
|-------------------|:------------:|:----------------:|
| AI Analysis       | ✅           | ❌               |
| Service Packaging | ✅           | ❌               |
| Cart/Orders       | ✅           | ❌               |
| Email Notifications| ✅          | ❌               |
| Supabase Security | ✅           | ❌               |
| Realtime DB       | ✅           | ❌               |

---

## 🚀 Deployment
1. Push repo to GitHub
2. Connect to Vercel
3. Add environment variables (see `.env.example`)
4. Build: `npm run build`

---

## ⚡ Installation & Setup
```powershell
git clone https://github.com/guidebazaar/setustudios.git
cd setustudios
npm install
copy .env.example .env
# Edit .env with your credentials
npm run dev
```

---

## 🔗 API Usage
- **Supabase:** Auth & DB (`src/config/supabase.ts`)
- **EmailJS:** Notifications (`src/services/email.ts`)
- **Gemini/OpenAI:** Idea analysis (`src/services/gemini.ts`)
- All API calls are centralized in `src/services/`

---

## 🧩 Troubleshooting
- Supabase errors: check `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`
- Email issues: verify EmailJS keys
- LLM errors: use a proxy and check quota

---

## 🤝 Contributing
1. Fork
2. Create a branch
3. Make changes + tests
4. Open a PR

---

## 📄 License
MIT — see `LICENSE` file.

---

<div align="center">
  <img src="https://img.shields.io/badge/Made_with-%F0%9F%92%A1-FFD700?style=for-the-badge" />
  <br>
  <b>Setu Studios — Empowering Ideas</b>
</div>
