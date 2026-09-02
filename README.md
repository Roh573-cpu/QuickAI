# ⚡ Quick.ai — AI-Powered Content & Productivity SaaS

> From idea to article, image, or polished resume — in seconds. One platform, every AI tool you need.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://quick-ai-kappa-eight.vercel.app)
[![Made with MERN](https://img.shields.io/badge/stack-MERN-61DAFB?logo=react)](#tech-stack)
[![License](https://img.shields.io/badge/license-MIT-blue)](#license)
[![Status](https://img.shields.io/badge/status-active-success)](#)

🔗 **Live App:** [quick-ai-kappa-eight.vercel.app](https://quick-ai-kappa-eight.vercel.app)

---

## 📖 Overview

**Quick.ai** is a full-stack **MERN SaaS platform** that bundles multiple AI-powered productivity tools into a single, unified dashboard. Instead of juggling five different AI apps for writing, image editing, and resume review, users get one clean interface backed by a subscription/freemium model.

Built to demonstrate real-world SaaS architecture: authentication, API-metered AI usage, file/image handling, a database-backed dashboard, and a deployed production environment — not just a CRUD demo.

<img width="800" alt="Quick.ai Landing Page" src="https://github.com/user-attachments/assets/bcd09918-30eb-4041-b27d-bd9bbec77cf6" />


---

## ❓ Problem → Solution

Creators, students, and professionals waste time switching between separate tools to write content, design images, and polish resumes. **Quick.ai** consolidates these into one AI-driven workspace, so the workflow is: *log in → pick a tool → generate → done.*

---

## ✨ Features

- 📝 **AI Article Writer** — generate long-form articles from a topic/prompt
- 🏷️ **Blog Title Generator** — instant, SEO-friendly title suggestions
- 🎨 **AI Image Generation** — text-to-image creation
- 🧼 **Background Remover** — one-click image background removal
- 🩹 **Object Removal** — remove unwanted objects from photos
- 📄 **AI Resume Review** — upload a resume, get AI-driven feedback
- 👥 **Community Feed** — share and browse AI-generated creations
- 🔐 **Secure Authentication** — sign up/login (Clerk CLI for Authentication)
- 💳 **Freemium / Usage-based Plans** — free tier + paid upgrade path
- 📱 **Fully Responsive UI** — works across desktop and mobile


---

## 🛠️ Tech Stack

| Layer          | Technology                                   |
|----------------|-----------------------------------------------|
| Frontend       | React.js, Tailwind CSS                        |
| Backend        | Node.js, Express.js                           |
| Database       | MongoDB (Mongoose)     |
| Authentication | Clerk CLI Authentication                    |
| AI Provider    | Google Gemini API        |
| Image Handling | Cloudinary |
| Deployment     | Vercel (frontend + serverless backend)         |


---

## 🏗️ Architecture

```
Client (React) 
   │
   ▼
Express REST API 
   │
   ├──► MongoDB (users, history, credits)
   └──► External AI API (Gemini/OpenAI) + Image API
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js ≥ 18
- MongoDB Atlas URI
- API keys for your chosen AI/image/auth providers

### Installation

```bash
# Clone the repo
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install
```

### Environment Variables

Create a `.env` file in the `server` directory:

```env
DATABASE_URL=
CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
GEMINI_API_KEY=
CLIPDROP_API_KEY=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
```

### Run Locally

```bash
# In /server
npm run server

# In /client
npm run dev
```

---

## 📁 Folder Structure

```
quick-ai/
├── client/          # React frontend
│   ├── src/
│   └── ...
├── server/          # Express backend
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── ...
└── README.md
```

---

## 🗺️ Roadmap

- [ ] Add usage analytics dashboard
- [ ] Team/workspace collaboration
- [ ] More AI tools (video summarization, code generation)
- [ ] Dark mode

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](../../issues).

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

**Rohan Dey** — [rohandeysc@gmail.com] · [www.linkedin.com/in/rohan-dey-61a020360](#) · 

⭐ If you found this project interesting, consider giving it a star!
