# academics-projects

# MSc Data Science: Academic Projects

**Abhiram Jammula**, MSc Data Science, Aston University (London)
[LinkedIn](https://www.linkedin.com/in/abhiram-jammula-38937224b/)

This repo collects the projects I worked on during my Master's. They cover machine learning, explainable and responsible AI, data design for fraud detection, and business strategy. Some are individual and some are team projects, and for each one I've said which part was mine.

| Project | Module | Type | Main skills |
| --- | --- | --- | --- |
| [RedPill Verify](#1-redpill-verify-verified-milestone-payments-for-a-uk-fintech) | Interdisciplinary Collaborative Project | Client project, team lead | Synthetic data design, fraud and risk analysis, pilot design |
| [Adobe Client Pitch](#2-adobe-client-pitch-genai-in-higher-education) | Interdisciplinary Collaborative Project | Client project, team lead | Framework design, GenAI research, pitching |
| [ShopSense AI](#3-shopsense-ai-explainable-recommendation-and-responsible-ai) | AI: Vision and Reality | Individual | Explainable AI, recommender systems, AI governance |
| [Weather Activity Recommender](#4-local-weather-analyser-with-smart-activity-recommender) | Fundamentals of Digital Technologies | Group of five | Python, scikit-learn, decision logic |
| [WRSX Simulation](#5-wrsx-group-strategic-plan-and-board-simulation) | Strategic Management | Group of six | Financial and strategic analysis |

---

## 1. RedPill Verify: Verified-Milestone Payments for a UK Fintech

*Interdisciplinary Collaborative Project · Sep to Nov 2026 · Team lead, team of six*

**The client:** RedPill Verify Ltd, a UK fintech building a conditional payment tool for business-to-business transactions.

**The problem:** small construction subcontractors often wait weeks to be paid, can't see whether the money exists, and face slow, subjective sign-off.

**What we recommended:** a pilot where each milestone is funded into a bank's restricted account. The system checks objective evidence (time, location, duplicates, quantities), people judge quality, and money is released only when work is accepted or a dispute is settled.

**What I did:**
- Led the team and presented a 15 to 20 minute recommendation and pilot plan to the client's founder.
- Compared five payment approaches: manual, digital workflow, escrow, project bank account and conditional payment.
- Built a fraud and control register of 38 risks across 9 groups, including prompt injection into AI-read contracts, narrowed to 11 controls for the pilot.
- Designed a simulated evidence pack for the client to test its own verification engine:
  - 21 images with real EXIF metadata, a 32-item materials schedule, JSON claims and CSV event logs
  - a SHA-256 integrity manifest
  - 19 planted fraud cases and 6 honest control cases, to measure detection and false-flag rates
- Designed an 18-week pilot with review gates and a stop rule on any wrongful payment.

**Output:** recorded pitch, a 15-page Harvard-referenced report with six appendices, and the simulated evidence pack.

> The evidence pack uses fictional firms and data. Its answer key isn't included here.

---

## 2. Adobe Client Pitch: GenAI in Higher Education

*Interdisciplinary Collaborative Project · 2026 · Team leader, team of six (Team Synapse)*

**The brief** (from Adobe's Head of Global Education): how can generative AI transform creativity and productivity in education, and how should universities adopt it?

**What we produced:**
- **GenAI Readiness Index:** a 1 to 5 scoring framework across three categories (total out of 15), so a university can see how ready it is to adopt generative AI.
- **"Create with Confidence" campaign:** a student awareness campaign and poster made in Adobe Express, with the tagline *"AI drafts. You decide."*
- **Recommendations** for institutions, students and Adobe, with a phased plan: assess, align, launch, monitor.

**My role:** I led the team, set the project direction, brought everyone's sections together into one pitch, and directed the final pitch video.

---

## 3. ShopSense AI: Explainable Recommendation and Responsible AI

*AI: Vision and Reality · Sep 2026 · Individual report and presentation*

A consultancy report for a fictional AI e-commerce platform that wants to keep more customers and get fewer returns.

**Main recommendations:**
- **Generative AI as decision support, not autonomy.** Shoppers want AI help with research, not with the final purchase.
- **A "Why This Pick" explanation layer** on a hybrid LLM and graph-based recommender.
- **Faithful explanations, not just convincing ones.** An LLM can write a reason that sounds right but isn't why the model chose the item. Explanations should come from the recommender's real ranking signals and be tested against how the model actually behaves.
- **Popularity-bias monitoring**, so long-tail products and smaller sellers aren't pushed out.
- **Ongoing governance** using the NIST Generative AI Profile, EU AI Act risk tiers (Articles 5 and 50) and co-design with customers, sellers and compliance staff.

---

## 4. Local Weather Analyser with Smart Activity Recommender

*Fundamentals of Digital Technologies · Jun 2026 · Group of five*

**My part:** the Smart Activity Recommender. It takes the rain probability from a teammate's logistic regression model and turns it into plain advice for four everyday activities.

Each activity has its own thresholds, because each one is affected by the weather differently:

| Activity | Rain threshold | Also checks |
| --- | --- | --- |
| Drying laundry | 40% (strictest) | Rain only |
| Football | 65% (most tolerant) | Temperature |
| Morning walk | 70% | Cold below 2°C, wind above 20 mph |
| Cycling | Activity-specific | Wind |

**Example:** with a 59.7% chance of rain and 30 mph wind, the recommender advises against walking, cycling and drying laundry, but says football is fine. A single "will it rain?" answer couldn't make those distinctions.

**Data:** 2,192 daily records of London weather, 2020 to 2025. This is a **synthetic dataset generated with AI** for teaching purposes, not real Met Office data.

**Limitations:** the thresholds are based on judgement, not learned from data. With user feedback they could be calibrated against real outcomes.

**Tech:** Python, pandas, scikit-learn

---

## 5. WRSX Group: Strategic Plan and Board Simulation

*Strategic Management · Oct to Nov 2026 · Group of six*

WRSX is a fictional listed advertising group in *The Strategy Experience* simulation. Its share price had fallen 39% to 228p.

**Part 1, the plan:** we wrote a three-year turnaround plan using PESTEL, Five Forces, VRIO, ERRC and SAFe. The target was a share price of about 590p, reached by raising earnings per share and rebuilding investor trust through better governance.

**Part 2, the simulation:** across six board meetings the share price rose from **228p to 528p (+132%)** and revenue from **£200m to £333.8m**. We missed the price target by 62p. I split that gap into +84p from earnings that beat the plan and −147p from a lower P/E ratio. Growth through acquisitions raised profit, but weak risk and governance scores held back how investors valued it.

**My role:** I proposed the agenda items and options at each board meeting before the team voted, and wrote an individual review of our decision-making.

*Case data: The Strategy Experience, Learning Dynamics Ltd.*

---

## Tools and skills across these projects

Python · pandas · scikit-learn · synthetic test data design · JSON / CSV · EXIF metadata · SHA-256 · explainable AI · recommender systems · EU AI Act · NIST AI RMF · fraud and risk analysis · financial and strategic analysis · team leadership · client pitching

## Teammates

- **Weather Recommender:** Peddoju Ester Rani, Himadri Jawle, Mahesh Sudharshan Chennur, Shreya Daram
- **WRSX (Group H):** Esther Rani Peddoju, Mahesh Sudharshan Chennur, Shreya Daram, Himadri Jawle, Harathi Byagari
