# Uxelo

**Get an expert-level UI/UX audit of any screenshot in seconds.**

Uxelo is an AI-powered UI/UX analysis platform. Upload a screenshot of any screen and Uxelo runs a targeted, automated inspection across accessibility, layout, and visual hierarchy guidelines — no manual checklists, no guesswork.

<p align="center">
  <img src="./screenshots/01-landing.png" alt="Uxelo Landing Page" width="800"/>
</p>

<p align="center">
  <a href="https://uxelo-web-project-1nos.vercel.app/"><b>🚀 Live Demo</b></a> ·
  <a href="#getting-started"><b>Setup Guide</b></a> ·
  <a href="#features"><b>Features</b></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Live-Vercel-black?logo=vercel" alt="Vercel"/>
  <img src="https://img.shields.io/badge/Stack-MERN-green" alt="MERN Stack"/>
  <img src="https://img.shields.io/badge/AI-Gemini%20Vision-blue?logo=googlegemini" alt="Gemini Vision"/>
  <img src="https://img.shields.io/badge/Status-Active-success" alt="Status"/>
</p>

---

## 📖 Overview

Manually auditing a product's UI/UX for accessibility and design consistency is slow and inconsistent. Uxelo automates this process: it takes static screenshots or mockups and runs them through a visual analyzer powered by **Gemini Vision**, producing a diagnostic report with concrete, prioritized, page-level recommendations — in seconds instead of hours.

## ✨ Features

- **Instant Visual Audits** — Submit a screenshot and get an inspection covering accessibility, layout, and hierarchy in seconds.
- **UI & UX Scoring** — Every screen is scored out of 100 on both UI and UX, with an aggregated project-level average.
- **Multi-Page Projects** — Group related screens (Homepage, Dashboard, Checkout, Settings, etc.) into a single project and track them together.
- **Prioritized Recommendations** — Findings are automatically split into **Quick Wins** (easy, high-impact fixes) and **High Priority** issues (critical fixes needed).
- **PDF Report Export** — Export a full diagnostic report for an entire project, or export a report for a single screenshot — both as downloadable PDFs.
- **Workspace Dashboard** — A clean console showing all your projects, their analysis status, and overall scores at a glance.
- **Authentication** — Secure sign-in with email/password (JWT) or Google OAuth.
- **Dark Mode** — Full dark mode support across the app.
- **Free Plan Limits** — 5 projects and 5 screenshots per project on a rolling 24-hour window.

## 🖼️ Screenshots

| Workspace Dashboard | Diagnostic Report |
|---|---|
| ![Dashboard](./screenshots/02-dashboard.png) | ![Diagnostic Report](./screenshots/03-diagnostic-report.png) |

| Quick Wins & High Priority | Per-Page Breakdown |
|---|---|
| ![Quick Wins](./screenshots/04-quick-wins-priority.png) | ![Project Pages](./screenshots/05-project-pages.png) |

## 🧠 How It Works

1. **Create a project** and give it a name.
2. **Upload screenshots** of the screens you want audited (up to 5 per project on the free plan).
3. Uxelo's analyzer inspects each screenshot against accessibility, layout, and hierarchy guidelines using Gemini Vision.
4. View **UI and UX scores** per page and across the whole project.
5. Review issues sorted into **Quick Wins** and **High Priority**, each tagged to the page it belongs to.
6. **Export a PDF report** — for the full project or for a single screenshot — to share with your team.

## 🛠️ Tech Stack

**Frontend**
- React + Vite
- Tailwind CSS
- Framer Motion

**Backend**
- Node.js + Express
- MongoDB

**AI / Analysis**
- Gemini Vision API (`gemini-2.0-flash`)

**Infrastructure**
- Cloudinary — image storage
- JWT + Google OAuth — authentication
- Vercel — deployment

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB instance (local or Atlas)
- Gemini API key
- Cloudinary account
- Google OAuth credentials

### Installation

```bash
# Clone the repository
git clone https://github.com/Misbah-Islam/Uxelo.git
cd Uxelo
```

**Backend setup**
```bash
cd server
npm install
```

Create a `.env` file inside `server/`:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
GOOGLE_CLIENT_ID=your_google_oauth_client_id
GOOGLE_CLIENT_SECRET=your_google_oauth_client_secret
```

```bash
npm run dev
```

**Frontend setup**
```bash
cd ../client
npm install
```

Create a `.env` file inside `client/`:
```env
VITE_API_BASE_URL=http://localhost:5000
VITE_GOOGLE_CLIENT_ID=your_google_oauth_client_id
```

```bash
npm run dev
```

The app will be available at `http://localhost:5173`.

## 🌐 Live Demo

Try it here: **[uxelo-web-project-1nos.vercel.app](https://uxelo-web-project-1nos.vercel.app/)**

## 📁 Project Structure

```
Uxelo/
├── client/          # React + Vite frontend
└── server/          # Node/Express backend
```

## 📌 Roadmap

- [ ] Paid tiers with higher project/screenshot limits
- [ ] Team workspaces
- [ ] Historical trend tracking per project
- [ ] Figma plugin integration

## 👤 Author

**Misbah Islam**
[GitHub](https://github.com/Misbah-Islam) · [Live Project](https://uxelo-web-project-1nos.vercel.app/)

---

<p align="center">Built with ❤️ using the MERN stack and Gemini Vision</p>
