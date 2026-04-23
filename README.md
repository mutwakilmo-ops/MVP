
# Coding Agent Session Export: Building YC Founder Engagement Dashboard + SDG Impact Lab

**Date:** April 2026
**Project:** YC Bookface-style Internal Tools Dashboard + 17 SDGs Platform
**Tech Stack:** React, TypeScript, Tailwind CSS, Recharts, Ruby on Rails, PostgreSQL, Bolt.new, DeepSeek
**Live URLs:** 
- https://yc-founder-engagemen-tch8.bolt.host/
- https://sdg-impact-lab-platf-cgoj.bolt.host/
**GitHub:** https://github.com/mutwakilmo-ops

---

## Summary

This session shows how I built a production-ready YC-style engagement analytics dashboard from scratch in one coding session. The dashboard tracks founder retention by gender, education level, and region — with auto-generated insights and JSON export. The same patterns map directly to SDG 4 (Quality Education) and SDG 5 (Gender Equality). I then extended the same thinking to build an umbrella platform for all 17 UN SDGs, showcasing a $12 trillion market opportunity.

**What this demonstrates:** Full-stack product engineering, rapid shipping, product thinking, AI tool fluency, and mission-driven architecture.

---

## Initial Prompt to Agent (Bolt.new + DeepSeek)

---

## Agent Response & Key Exchanges

### Exchange 1: Data Architecture

**Agent:** What data structure do you need for users?

**Me:** Users need: name, gender, education_level, region, created_at, last_active_at, total_session_seconds. Also FeatureLog: user_id, feature_name, event_type, created_at. Seed 200 users showing engagement gaps — rural women should have lower retention to prove the pattern.

**Agent:** Understood. Generating Rails migration and seed file with 200 users, realistic distribution showing gender/education/region gaps. Rural women show 34% lower engagement to demonstrate the pattern.

**My thinking:** I intentionally designed the data model to surface equity gaps. This proves the dashboard can identify underserved segments — critical for both YC founders (which founders need more help?) and SDG 4/5 (which students need more support?).

---

### Exchange 2: Insights Panel

**Me:** Add auto-generated insights that detect these gaps. Example: "Women in rural areas have 40% lower engagement — suggest mobile-friendly offline features"

**Agent:** Added conditional insight generation. Logic checks filtered data and generates text like: "Women in rural areas show 34% lower retention — offline-first features would boost equity (SDG 5)."

**My thinking:** The insights panel transforms raw data into actionable recommendations. This is exactly what YC Partners need — not just numbers, but "what should I do differently?"

---

### Exchange 3: Frontend Implementation

**Agent:** Building dashboard components with Recharts for the feature usage bar chart.

**Me:** Make sure it's mobile responsive and dark mode. YC internal tools should look clean.

**Agent:** Tailwind CSS configured with dark mode. Responsive grid layout. Cards for each metric.

**My thinking:** Internal tools need to be usable anywhere — on a desktop at HQ or on a phone between meetings. Dark mode reduces eye strain for engineers who live in terminals.

---

### Exchange 4: Deployment

**Me:** Deploy.

**Agent:** Deployed. Live at https://yc-founder-engagemen-tch8.bolt.host/

**Result:** Working MVP in one session (approximately 3 hours total).

---

## Full Build Log

| Time | Milestone | Key Decision |
|------|-----------|--------------|
| 0:00 | Project setup (Vite + React + TypeScript + Tailwind) | Chose Vite for speed |
| 0:15 | Rails API + PostgreSQL + seed data (200 users) | Real backend, not mock |
| 0:45 | Dashboard UI + metrics cards | Card-based layout for clarity |
| 1:15 | Filters (gender, education, region) | Designed for SDG 4/5 mapping |
| 1:45 | Feature usage chart (Recharts) | Horizontal bars for easy scanning |
| 2:15 | Insights panel + JSON export | Auto-detects equity gaps |
| 2:45 | Deployment + testing | One-click deploy |
| 3:00 | Live MVP complete | Ships fast |

---

## Part 2: Extending to SDG Impact Lab (17 Goals)

After the YC dashboard was live, I asked the agent to build an umbrella platform for all 17 SDGs.

**Prompt:**

**Agent:** Created 17 SDG cards with emojis, titles, and descriptions. Added market data: $12T opportunity, 380M jobs by 2030, $5-7T annual investment need.

**Me:** Link to the YC dashboard as proof of concept.

**Agent:** Added integration section showing the MVP that proves the pattern.

**Deployed:** https://sdg-impact-lab-platf-cgoj.bolt.host/

---

## Technical Decisions & Why

| Decision | Why |
|----------|-----|
| Rails + PostgreSQL | Matches YC's stack, real production backend |
| React + TypeScript | Type safety, maintainable at scale |
| Tailwind CSS | Rapid UI development, consistent design |
| Recharts | Simple, customizable, good for dashboards |
| localStorage → PostgreSQL | Agent recommended upgrade; I agreed for real use case |
| Dark mode first | YC engineers work late; reduces eye strain |
| Insights panel | Shows product thinking beyond raw data |
| Export JSON | Real internal tool feature (share with team) |

---

## Challenges & Debugging

**Challenge 1:** Seeded data wasn't showing clear engagement gaps.

**Debug:** I examined the seed file and realized distribution was too uniform. I asked the agent to bias the data: rural women = 34% lower retention. The agent regenerated the seed file.

**Challenge 2:** Filters weren't updating all metrics consistently.

**Debug:** The agent had built separate state for each component. I requested a single source of truth via a custom hook that fetches filtered data from the API. Agent refactored.

**Challenge 3:** Deployment initially failed due to missing environment variables.

**Debug:** Agent identified missing DATABASE_URL and configured Render.com settings.

---

## Results & Impact

| Metric | Result |
|--------|--------|
| Time to MVP | ~3 hours (one session) |
| Lines of code | ~2,500 (frontend + backend) |
| Live users | Publicly accessible dashboard |
| Features shipped | 6 major features (metrics, filters, chart, insights, export, responsive) |
| Demonstrates for YC | Full-stack, product thinking, ships fast, internal tools |

---

## What This Session Proves for YC Internal Tools Role

| YC Requirement | Evidence from Session |
|----------------|----------------------|
| Design and build features end-to-end | Built full dashboard + API + frontend from scratch |
| Work alongside Partners on productivity software | Dashboard mimics internal YC partner tools |
| Scope and prioritize roadmap | Chose metrics that matter for engagement AND SDGs |
| Analyze usage and engagement for continuous improvement | Insights panel auto-detects gaps |
| Ship fast | Two live MVPs in days |
| Full-stack web | React + TypeScript + Rails + PostgreSQL |
| Front-end focus | Tailwind, Recharts, responsive, dark mode |
| Use AI tools fluently | Prompted, iterated, deployed with Bolt.new + DeepSeek |

---

## My Background (As Shared With Agent)

- **Co-founder, HackYourFuture Belgium:** Coding school for refugees — zero to operational MVP in 2 months
- **Community Health Officer, MSF:** Frontline crisis response — rapid problem-solving under pressure
- **Android Expert:** 4 jury-validated apps (Kotlin, MVI, Jetpack Compose)
- **Now:** Full-stack web (Rails + React) at 2x speed

---

## Vision Statement

> *"Build for YC first. Scale the patterns to the world. Then scale to all 17 SDGs. That's the 20x startup mindset."*

My ultimate vision is to leverage technical grit to build AI-driven solutions that tackle the 17 UN Sustainable Development Goals — creating global impact through code.

---

## Live Proof

| Asset | URL |
|-------|-----|
| YC Founder Dashboard | https://yc-founder-engagemen-tch8.bolt.host/ |
| SDG Impact Lab | https://sdg-impact-lab-platf-cgoj.bolt.host/ |
| GitHub Profile | https://github.com/mutwakilmo-ops |

---

**End of Session Export**
