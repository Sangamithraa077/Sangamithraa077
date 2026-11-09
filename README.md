<div align="center">

<img src="assets/banner.png" width="100%" alt="banner" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=19&duration=2600&pause=900&color=2DD4BF&center=true&vCenter=true&width=680&lines=Catching+policy+contradictions+before+the+audit+does...;Teaching+an+AI+coach+to+check+its+own+numbers...;Reading+655%2C147+SSH+log+events+so+you+don't+have+to...;Reporting+the+score+that+embarrasses+my+model..." alt="typing banner" />

![Role](https://img.shields.io/badge/Role-All--Rounder-0F766E?style=for-the-badge&logo=cricket&logoColor=white)
![Batting](https://img.shields.io/badge/Batting-Full--Stack%20AI-134E5E?style=for-the-badge)
![Bowling](https://img.shields.io/badge/Bowling-Applied%20ML%20Security-0E7490?style=for-the-badge)

</div>

<br>

## 🏏 Playing XI Profile

I'm a Computer Science student from Coimbatore who builds AI systems for a specific kind
of problem: information that is too dense, too scattered, or too high-stakes for a person
to check by hand. A policy that contradicts itself two clauses later. A login pattern that
looks almost, but not quite, like every other one that day. An athlete's muscles quietly
tiring while the effort score still says everything is fine.

What I care about most is the part after the model runs. PolicySentinel keeps a knowledge
graph and an audit trail behind every conflict it flags. My SSH detector was tested on a
server it had never seen, and its README reports the drop from about 99% F1 to about 68%
instead of hiding it. Athlete Intelligence checks every number its AI coach quotes, and its
own write-up admits where the model does not beat a simple baseline. An AI system that
can't show its work is just a black box with better PR.

Off the field, my GitHub bio calls what I do *"Tüfteln"*, German for tinkering, which is
closer to the truth than any job title. My profile motto: **"Sunrise never waits for
latecomers."** I try to build the same way: early, deliberate, and without waiting for
permission to start.

<br>

## 🏆 Man of the Match Performances

<details open>
<summary><b>Athlete Intelligence</b> · <i>the newest innings: explainable fatigue tracking for athletes</i></summary>
<br>

**The over:** Fatigue is usually measured after the fact, by asking an athlete "how hard
did that feel, from 6 to 20?" By then it is too late to prevent anything.

**How it was played:** A real-time, explainable, personalised muscle-fatigue platform built
on wearable EMG, IMU and PPG signals. Four cooperating agents audit signal quality, adjust
to the athlete's own baseline, explain the drivers with SHAP, and apply warning and stop
thresholds. An AI coach (Claude, then a local Ollama model, then rule-based answers as a
fallback) turns that into plain advice, and every number it quotes is checked: a draft with
an invented figure is sent back once, then replaced with a verified answer. It also says "I
can't tell that from these readings" to questions it has no business answering.

**The honest scoreboard:** Evaluated leave-one-athlete-out on 34 athletes, the best model is
off by about 1.65 Borg points versus 3.17 for guessing the average, and the README itself
points out that most of that gain comes from elapsed time rather than the sensors. 419
passing tests.

**[scorecard →](https://github.com/Sangamithraa077/Agentic-Fatigue-Fingerprinting)**

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/-XGBoost-EC0000?style=flat-square)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![SHAP](https://img.shields.io/badge/-SHAP-0B7285?style=flat-square)
![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat-square)

</details>

<details open>
<summary><b>PolicySentinel</b> · <i>built for the Société Générale Hackathon, deployed and live</i></summary>
<br>

**The over:** Policies pile up as a company grows, and they start contradicting each other
quietly. One policy says delete logs after 90 days, another says keep them for 7 years. Or
a "MUST encrypt" slowly softens into a "SHOULD" over a few revisions. Nobody notices until an
audit does.

**How it was played:** Upload a PDF or DOCX, build the clause tree, and have Gemini 2.5 Flash
extract each obligation as subject, modality, action and object. A semantic engine and a
deterministic rule-based engine then compare obligations across policies, map them to GDPR,
ISO 27001, SEBI CSCRF and RBI Master Direction, and draft redlines that a human accepts or
rejects. Everything lands in a Neo4j knowledge graph with an audit trail. If Gemini hits its
quota, a circuit breaker fails over to a local rule-based engine so the app keeps working.
Built with a teammate.

**[watch the replay →](https://policysentinel-frontend.onrender.com)** · **[scorecard →](https://github.com/Sangamithraa077/PolicySentinel)**

![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React_18-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Neo4j](https://img.shields.io/badge/-Neo4j-018bff?style=flat-square&logo=neo4j&logoColor=white)
![Gemini](https://img.shields.io/badge/-Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

</details>

<details>
<summary><b>RegIntel AI</b> · <i>opening partnership, built for the SEBI Hackathon</i></summary>
<br>

**The over:** SEBI keeps issuing circulars. Somewhere, a compliance team has to map every one
of them against internal SOPs by hand.

**How it was played:** Batted this one as part of a team. An Agentic Compliance OS where 8
specialised agents, coordinated by one orchestrator, ingest SEBI circulars, extract
clause-level obligations, find gaps against company SOPs with vector-embedding similarity
search, draft precise redlines without touching unrelated clauses, validate evidence, and
score compliance health, with explainability and audit trails throughout.

**[scorecard →](https://github.com/ashokpsgitech/SEBI-hackathon--RegIntel-AI)**

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React_19-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/-Tailwind_v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![LLM Agents](https://img.shields.io/badge/-LLM_Agents-4285F4?style=flat-square)

</details>

<details>
<summary><b>SSH-Bruteforce-Detection</b> · <i>the wicket-taking spell</i></summary>
<br>

**The over:** SSH brute-force detectors that are trained and tested on the same dataset look
great on paper, then struggle on a network they have never seen. Random train/test splits
also leak information between neighbouring time windows.

**How it was played:** A leakage-free pipeline: chronological 70/10/20 splits over 10,353
fifteen-minute windows built from 655,147 OpenSSH log events, with an automated check that no
window appears in two splits. XGBoost reached 98.77% accuracy (99.32% F1) in-domain. Then,
with zero retraining, it faced a different server's logs (84,195 events from an AWS EC2
host): F1 fell to about 68%, which the README explains as domain shift instead of hiding it.
The tree models held up better than LSTM and GRU there, keeping ROC-AUC between 0.77 and 0.80.

**[scorecard →](https://github.com/Sangamithraa077/SSH-Bruteforce-Detection)**

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/-XGBoost-EC0000?style=flat-square)
![LightGBM](https://img.shields.io/badge/-LightGBM-2E7D32?style=flat-square)
![LSTM / GRU](https://img.shields.io/badge/-LSTM_%2F_GRU-6A1B9A?style=flat-square)

</details>

<br>

## 🎒 Kit Bag

<div align="center">

<img src="https://skillicons.dev/icons?i=py,java,ts,js,react,vite,tailwind,fastapi,postgres,docker,pytorch,git,github" alt="skills" />

<br><br>

![Gemini](https://img.shields.io/badge/Gemini_2.5-134E5E?style=flat-square&logo=google&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-0E7490?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-0F766E?style=flat-square)
![scikit--learn](https://img.shields.io/badge/scikit--learn-14B8A6?style=flat-square&logo=scikitlearn&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-134E5E?style=flat-square)
![Neo4j](https://img.shields.io/badge/Neo4j-0E7490?style=flat-square&logo=neo4j&logoColor=white)
![Render](https://img.shields.io/badge/Render-0F766E?style=flat-square&logo=render&logoColor=white)

</div>

<br>

## 📋 Team Role

| Position | What I bring |
|---|---|
| **All-rounder: Agentic AI** | Multi-agent pipelines that reason in stages, stop when the data is bad, and show their work |
| **New-ball bowler: Applied ML Security** | Detection systems tested on data they have never seen |
| **Wicketkeeper: RegTech & Knowledge Graphs** | Making regulation something software can actually check |
| **Third umpire: Explainability & Honest Evaluation** | SHAP explanations, number-checking guardrails, and results reported even when they sting |

<br>

## 🏋️ Nets Practice — Currently Working On

<table>
<tr>
<td width="50%" valign="top">

**🐳 Docker & Deployment**
`██████░░░░` 60%

</td>
<td width="50%" valign="top">

**🕸️ Neo4j Knowledge Graphs**
`██████░░░░` 60%

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🧬 Vector Embeddings & Semantic Search**
`█████░░░░░` 50%

</td>
<td width="50%" valign="top">

**🧠 LLM Orchestration & Prompt Engineering**
`███████░░░` 70%

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🔍 Explainable AI & Audit Trails**
`█████░░░░░` 55%

</td>
<td width="50%" valign="top">

**📡 Biosignal & Time-Series ML**
`█████░░░░░` 50%

</td>
</tr>
</table>

<br>

## 📮 Send a Message to the Dugout

Every project up there started as a small, stubborn question I couldn't let go of: *why
does this contradict that?*, *why did this model fail on new data?* If you're chasing a
question like that too, or you just want to compare notes on cricket, code, or both, don't
overthink it. Say hi. No pitch required, no "quick 15 minutes," just a real message from
a real person.

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Sangamithraa077-181717?style=for-the-badge&logo=github)](https://github.com/Sangamithraa077)
[![Email](https://img.shields.io/badge/Email-sangamithraasenthil%40gmail.com-0F766E?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sangamithraasenthil@gmail.com)

</div>

<br>

<div align="center">

<sub>Thanks for scrolling this far, that means more to me than a star. See you in the next commit. 💙💚</sub>

</div>
