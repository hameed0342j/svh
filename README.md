# 🚛 SVH — Smart Logistics Hackathon Toolkit

> **AI-powered hackathon ideation framework for generating novel, scalable logistics solutions.**  
> Built with skills from [superpowers-skills](https://github.com/obra/superpowers-skills) and [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills).

---

## 📂 Repository Structure

```
svh/
├── README.md                          ← You are here
├── skills.md                          ← Comprehensive 13-skill reference guide
├── logistics-hackathon-ideas.md       ← 10 scored logistics ideas with architectures
├── corrected-evaluation.md            ← Honest evaluation with anti-inflation corrections
│
├── hackathon-skills/                  ← 🧠 Claude.ai-uploadable skills (ZIP & upload)
│   ├── hackathon-logistics-ideator/   ← Main ideation engine (collision-zone + inversion + scale)
│   ├── collision-zone-thinking/       ← Force unrelated domains together for breakthroughs
│   ├── inversion-exercise/            ← Flip assumptions to find hidden opportunities
│   ├── scale-game/                    ← Stress-test at 1000x to validate architecture
│   ├── simplification-cascades/       ← One insight that eliminates 10 components
│   ├── hackathon-idea-evaluator/      ← Score ideas honestly with anti-inflation rules
│   └── hackathon-pitch-builder/       ← Structure 3-min pitch with demo script
│
├── awesome-claude-skills/             ← Source: ComposioHQ skills (56+ skills)
└── superpowers-skills/                ← Source: obra/superpowers-skills (31 skills)
```

---

## 🏆 Top 3 Logistics Ideas (Corrected Scores)

| Rank | Idea | Score | One-liner |
|------|------|-------|-----------|
| 🥇 | **AddressIQ** | **53/60** | AI confidence scoring for delivery addresses — India's #1 last-mile pain point |
| 🥈 | **DeliveryCast** | **50/60** | "Weather forecast" for delivery success — heatmap predicts failures before dispatch |
| 🥉 | **ReturnFlow** | **49/60** | Intercept returns mid-transit, re-route to nearest buyer — ₹30-80 Cr/day savings |

> **Power Move:** AddressIQ + PackBuddy = **SmartRoute** (~56/60) — verified addresses feed package clustering for maximum impact.

---

## 🧠 Skills Overview

### What Are These Skills?

Skills are structured problem-solving techniques formatted as `SKILL.md` files with YAML frontmatter. They can be:
- **Uploaded to [Claude.ai](https://claude.ai)** → Settings → Skills → Add Skill (as ZIP)
- **Used with Claude Code** (Antigravity) → Place in `.claude/skills/` directory
- **Referenced manually** → Read and apply the techniques during brainstorming

### 7 Uploadable Skills

| Skill | What It Does | When to Use |
|-------|-------------|-------------|
| **hackathon-logistics-ideator** | Full ideation pipeline with all techniques combined | Start here — generates and scores ideas |
| **collision-zone-thinking** | Forces Logistics × [Biology/Games/Weather/Dating] collisions | When you need a breakthrough, not increment |
| **inversion-exercise** | Flips "faster is better" → "strategic slowness saves money" | When every solution feels obvious |
| **scale-game** | Tests at 1x vs 1,000,000x to find architectural limits | When judges ask "will this scale?" |
| **simplification-cascades** | Finds one abstraction that replaces 4 systems | When complexity is spiraling |
| **hackathon-idea-evaluator** | Scores on 6 dimensions with anti-inflation rules | Before committing to build |
| **hackathon-pitch-builder** | Structures 3-min pitch: Hook → Problem → Demo → Scale → Ask | When preparing the final presentation |

### How to Upload to Claude.ai

1. Navigate to `hackathon-skills/` folder
2. **Right-click** any skill folder (e.g., `hackathon-logistics-ideator`) → **Compress to ZIP**
3. Go to [claude.ai](https://claude.ai) → **Settings** → **Skills** → **Add Skill**
4. Upload the ZIP file
5. The skill auto-triggers when your prompt matches its description

---

## 📊 Scoring Methodology

Ideas are scored on 6 dimensions (1-10 each, total /60):

| Dimension | What's Measured | Anti-Inflation Rule |
|-----------|----------------|-------------------|
| **Novelty** | Is the TECHNOLOGY new (not just the framing)? | Caps at 7 if core algorithm exists elsewhere |
| **Feasibility** | Can you build an MVP in hackathon time? | -2 if needs data/hardware you don't have |
| **Scalability** | Does architecture hold at 1000x? | Must specify what breaks at scale |
| **Impact** | Market size × adoption probability | Must model cultural/behavioral barriers |
| **Demo-ability** | Can you show it working LIVE? | -1 for mock-data-dependent demos |
| **Domain Fit** | Is this a CORE logistics problem? | Must align with real industry pain points |

**Target:** ≥ 48/60 on corrected scoring before building.

---

## 🇮🇳 India Logistics Context

Key data points powering the idea generation:

| Metric | Value | Source |
|--------|-------|--------|
| Logistics cost (% of GDP) | 13-14% (vs 8% globally) | IBEF, National Logistics Policy |
| Last-mile delivery cost | 53% of total shipping cost | Shiprocket, McKinsey |
| Daily e-commerce deliveries | 10M+ | Industry estimates |
| RTO rate (Tier 2/3) | 15-25% | iCarry, Delhivery reports |
| Failed delivery cost | ₹100-300 per attempt | Industry average |
| Gig delivery workforce | 80%+ of last-mile | Shadowfax, Porter data |
| Warehouse utilization | 60-70% | Grant Thornton |
| D2C brands in India | 50,000+ | Inc42, YourStory |
| Cold chain food wastage | ~30% | NITI Aayog |

---

## 🛠️ Tech Stack Recommendations (For Building)

| Layer | Recommended | Why |
|-------|------------|-----|
| **Frontend** | Next.js + Tailwind CSS | Fast, SSR, great for dashboards |
| **Backend** | FastAPI (Python) | ML-friendly, async, fast prototype |
| **Database** | PostgreSQL + PostGIS | Geospatial queries for logistics |
| **ML/AI** | scikit-learn, XGBoost | Classification/scoring models |
| **Maps** | Leaflet.js + OpenStreetMap | Free, customizable heatmaps |
| **Real-time** | WebSockets / SSE | Live dashboard updates |
| **Deployment** | Vercel (FE) + Railway (BE) | Free tier, instant deploy |

---

## 📋 Hackathon Execution Checklist

```
□ Domain selected: Logistics ✅
□ Problem validated using domain template
□ Idea scored ≥ 48/60 on CORRECTED rubric
□ Collision-zone thinking applied — novel angle found
□ Inversion exercise applied — assumptions challenged
□ Scale-game applied — architecture validates at 1000x
□ Simplification cascades — complexity reduced to core
□ Implementation plan created — tasks split among team
□ Presentation structured — Hook → Problem → Demo → Scale → Ask
□ Demo script rehearsed (3-minute pitch)
□ GitHub repo clean with README ✅
□ Google Drive submission materials ready
□ Backup demo video recorded
```

---

## 📜 License

This project uses skills derived from:
- [superpowers-skills](https://github.com/obra/superpowers-skills) by Jesse Vincent
- [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) by ComposioHQ

Used for educational/hackathon purposes.

---

<p align="center"><b>Built for winning hackathons. 🏆</b></p>
