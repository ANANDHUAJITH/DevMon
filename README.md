# DevMon


> **Prove your skill. Earn your DevMon. Build in public.**

DevMon is an **open-source, gamified developer platform** where real-world coding tasks, open-source contributions, and project submissions are evaluated through **AI-assisted review and community verification**.  
Developers earn **unique, non-fakeable DevMon cards** based on their verified skill, with rarity levels inspired by collectible games.  

Unlike traditional platforms that rely on quizzes, stars, or resumes, DevMon focuses on **real contributions** and **verifiable skill**.

---

## 🚨 Project Status

🚧 **Early MVP (Active Development)**  
Expect changes and iterative improvements. Contributions, testing, and feedback are welcome.

---

## 🎯 Why DevMon Exists

### The Problem
- GitHub stars and resumes often **do not reflect skill**.  
- Coding platforms test puzzles, not real-world development.  
- Open-source contributions are undervalued or hard to track.  

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
Tasks involve practical work such as:
- Fixing issues in open-source projects  
- Building small tools or libraries  
- Writing documentation or tests  
- Designing system components  

Each task has:
- Difficulty level (1–5)  
- Maximum score  
- Clear evaluation criteria  

---

### 🤖 AI Evaluation
Submissions are analyzed using:
- LLM-based evaluation (OpenAI GPT-4 / GPT-4o-mini)  
- Static code analysis (ESLint, Pylint, Clippy)  
- Commit history review  
- Plagiarism detection  

**Scoring Breakdown Example:**

| Component          | Weight |
|-------------------|-------|
| Functionality     | 30%   |
| Code Quality      | 25%   |
| Originality       | 15%   |
| Security          | 15%   |
| Documentation     | 10%   |
| Git Commit History | 5%    |

**Output:**  
- Total Score (0–100)  
- Feedback for improvement  
- Suggested DevMon card rarity (Common → Legendary)  
- Optional human moderation flag  

---

### 🃏 DevMon Skill Cards
-Every validated task submission mints a **DevMon card**.

### MVP Rules:

-One card per user per task

-Hash ensures no forgery

-Displays name, score, and rarity

-Leaderboard uses card points

### Future Enhancements:

-Evolving cards with more tasks

-Seasonal limited edition cards

-Optional NFT integration for rare cards

#### 🏆 Leaderboard

-Tracks top contributors by card points

-Public visibility

-Early MVP shows top 10

-Future: seasonal, battle-based, and top ranger recognition

### 🌐 Community Features

**** MVP Level:

-View other users’ public cards

-Optional peer review for Task #0

**** Post-MVP:

-Mentorship and reviewing

-Team challenges / raids

-Social graph (followers, collaborators)

-Trust scores influence card multipliers

### 🛠 MVP Technical Architecture
*** Backend

-Node.js + TypeScript

-PostgreSQL database

-Redis for caching & leaderboard

-REST APIs (future GraphQL optional)

**** Services:

-GitHub OAuth integration

-AI review service

-Card minting & hash signing

-Submission tracking

***** Frontend

-React / Next.js

-Tailwind CSS for UI

**** Pages:

-Login/Register

-Task submission

-AI feedback

-Card display

-Leaderboard

*** AI Layer

-still thinking

-Static analysis + linters

-Score normalization

-Optional moderation flag

*** MVP Flow:

| User → GitHub Login → Task Submission → AI & Static Analysis → Score & Feedback → Card Minting → Leaderboard Update |

-Security & Anti-Cheat

-One account per GitHub

-Duplicate submission detection

-Commit history validation

-AI plagiarism detection

-Server-side hash signing for cards



### 🧩 Gamification & Progression

| Task points → DevMon card rarity → Leaderboard ranking |

-Rare cards limited per season

-Future: battle system, card evolution, seasonal events

-Points & ranks are earned, not bought

📁 Repository Structure
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


### 🧪 Future Improvements

-Multi-language support

-Adaptive AI question/task generation

-Battle mode & raids

-Seasonal limited edition DevMon cards

-Mentorship & community trust
