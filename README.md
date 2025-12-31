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
# DevMon Project TODO

## Core Features

### Authentication & Profiles
- [ ] GitHub OAuth integration setup
- [ ] User profile pages with bio, skills, and verified cards
- [ ] Follow/follower system
- [ ] User settings and profile editing

### Feed & Social
- [ ] Professional feed displaying projects, challenges, and achievements
- [ ] Persistent post system (not ephemeral)
- [ ] Post creation and editing
- [ ] Like/comment system on posts

### GitHub Integration
- [ ] GitHub repository submission system
- [ ] DevMon config file (devmon.yaml) validation
- [ ] Repository verification and metadata extraction
- [ ] Commit history and activity verification

### Challenges System
- [ ] Algorithm challenge creation and management
- [ ] System design challenges
- [ ] CSS/UI pixel-perfect visual challenges
- [ ] Difficulty tier system
- [ ] Time-boxed challenge mechanics
- [ ] Challenge submission handling

### AI Evaluation System
- [ ] LLM integration for code evaluation
- [ ] Scoring on correctness, code quality, architecture, readability, security, originality
- [ ] Transparent and explainable scoring feedback
- [ ] Custom review criteria per competition host

### DevMon Card System
- [ ] Card rarity levels (Common, Uncommon, Rare, Epic, Legendary)
- [ ] Card generation based on verified skills
- [ ] Card collection and inventory
- [ ] Limited supply mechanics for each rarity
- [ ] Card trading/marketplace (future)

### Competition System
- [ ] ComCert points system
- [ ] Developer battle system (1v1 and group)
- [ ] Point staking mechanics
- [ ] Battle result tracking

### Leaderboards & Rankings
- [ ] Global leaderboard
- [ ] Category-wise leaderboards (Web, Embedded, Security, UI/CSS)
- [ ] Seasonal leaderboards with resets
- [ ] Top player homepage features

### Notifications
- [ ] Real-time in-app notifications
- [ ] Email notifications for battles
- [ ] Battle challenge notifications
- [ ] Battle start notifications
- [ ] Battle result notifications

### UI/UX
- [ ] Instagram-inspired design system
- [ ] Professional minimal aesthetic
- [ ] Grid-style layout with varied flexbox components
- [ ] Elegant rounded corners
- [ ] Dark/light theme support
- [ ] Responsive design

## Database Schema
- [ ] Users table with GitHub integration
- [ ] Profiles table
- [ ] Follow relationships
- [ ] Posts table
- [ ] Challenges table
- [ ] Submissions table
- [ ] DevMon cards table
- [ ] User card inventory
- [ ] ComCert points tracking
- [ ] Battles table
- [ ] Leaderboards table
- [ ] Notifications table

## API & Backend
- [ ] tRPC procedures for all features
- [ ] GitHub API integration
- [ ] LLM integration for scoring
- [ ] Email service integration
- [ ] Real-time notification system

## Testing
- [ ] Unit tests for core logic
- [ ] Integration tests for API endpoints
- [ ] E2E tests for user flows

## Deployment
- [ ] Environment configuration
- [ ] Database migrations
- [ ] Production deployment


### 🧪 Future Improvements
- Multi-language support  
- Adaptive AI task generation  
- Battle mode & raids  
- Seasonal limited edition DevMon cards  
- Mentorship & community trust system  





