# DevMon

> **Prove your skill. Earn your DevMon. Build in public.**

DevMon is an **open-source, gamified developer platform** where **real-world coding tasks, open-source contributions, and project submissions** are evaluated through **AI-assisted review and community verification**.  
Developers earn **unique, non-forgeable DevMon cards** based on verified skill, with **rarity levels inspired by collectible games**.  

Unlike traditional platforms that rely on quizzes, stars, or resumes, DevMon focuses on **real contributions** and **verifiable skill**.

---

## 🚨 Project Status

**Early MVP (Active Development)**  
Expect changes and iterative improvements. Contributions, testing, and feedback are welcome.

---

## 🎯 Mission

### The Problem
- GitHub stars and resumes **often do not reflect actual skill**.  
- Most coding platforms test puzzles rather than real-world development.  
- Open-source contributions are undervalued or difficult to track.  

### The Solution
A transparent system where developers:
- Complete **real tasks**
- Submit **working repositories**
- Receive **AI-reviewed scores**
- Earn **cryptographically verifiable DevMon cards**

Skill becomes **provable, not claimed**.

---

## 🧩 Core Concepts

### 👤 Developer Identity
- GitHub OAuth login  
- Single account per developer  
- Reputation and cards are **permanent** and **verifiable**

### 🧪 Tasks
Practical tasks include:
- Fixing issues in open-source projects  
- Building small tools or libraries  
- Writing documentation or tests  
- Designing system components  

Each task includes:
- Difficulty (1–5)  
- Maximum score  
- Clear evaluation criteria  

---

### 🤖 AI Evaluation
Submissions are analyzed using:
- LLM-based evaluation (GPT-4 / GPT-4o-mini)  
- Static code analysis (ESLint, Pylint, Clippy)  
- Commit history review  
- Plagiarism detection  

**Scoring Example:**

| Component           | Weight |
|--------------------|-------|
| Functionality       | 30%   |
| Code Quality        | 25%   |
| Originality         | 15%   |
| Security            | 15%   |
| Documentation       | 10%   |
| Commit History      | 5%    |

**Output:**
- Total Score (0–100)  
- Feedback for improvement  
- Suggested DevMon card rarity (Common → Legendary)  
- Optional human moderation flag  

---

### 🃏 DevMon Skill Cards
- Every validated submission mints a **DevMon card**.  
- **MVP Rules:**
  - One card per user per task  
  - Hash ensures authenticity  
  - Displays name, score, and rarity  
  - Leaderboard uses card points  

- **Future Enhancements:**
  - Evolving cards with more tasks  
  - Seasonal limited edition cards  
  - Optional NFT integration for rare cards  

#### 🏆 Leaderboard
- Tracks top contributors by card points  
- Public visibility  
- Early MVP: top 10 contributors  
- Future: seasonal, battle-based, and “top ranger” recognition  

---

### 🌐 Community Features

**MVP Level:**
- View other users’ public cards  
- Optional peer review for Task #0  

**Post-MVP:**
- Mentorship and reviewing  
- Team challenges / raids  
- Social graph (followers, collaborators)  
- Trust scores influence card multipliers  

---

### 🛠 MVP Technical Architecture

**Backend:**
- Node.js + TypeScript  
- PostgreSQL  
- Redis (caching & leaderboard)  
- REST APIs (GraphQL optional)

**Services:**
- GitHub OAuth integration  
- AI review service  
- Card minting & hash signing  
- Submission tracking  

**Frontend:**
- React / Next.js  
- Tailwind CSS  

**Pages:**
- Login/Register  
- Task submission  
- AI feedback  
- Card display  
- Leaderboard  

**AI Layer (MVP):**
- Static analysis + linters  
- Score normalization  
- Optional moderation flag
  **Flow:**
  
**Security & Anti-Cheat:**
- One account per GitHub  
- Duplicate submission detection  
- Commit history validation  
- AI plagiarism detection  
- Server-side hash signing for cards  

---

### 🧩 Gamification & Progression

| Task points → DevMon card rarity → Leaderboard ranking |

- Rare cards are limited per season  
- Future: battle system, card evolution, seasonal events  
- Points & ranks are **earned, not bought**  

---

### 📁 Repository Structure

devmon/
├── README.md
├── VISION.md
├── ROADMAP.md
├── LICENSE
├── .gitignore
├── .env.example
├── docs/
│   ├── user.md
│   ├── task.md
│   ├── card.md
│   └── scoring.md
├── backend/
│   ├── src/
│   │   ├── index.ts
│   │   ├── routes/
│   │   ├── services/
│   │   └── models/
│   └── package.json
├── frontend/
│   ├── pages/
│   └── package.json
└── scripts/
    ├── seedTasks.ts
    └── verifyCard.ts


---

### 🧪 Future Improvements
- Multi-language support  
- Adaptive AI task generation  
- Battle mode & raids  
- Seasonal limited edition DevMon cards  
- Mentorship & community trust system  





