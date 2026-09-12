<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a8a,100:38bdf8&height=240&section=header&text=Vihang%20Patil&fontSize=62&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Full-Stack%20Developer%20%7C%20AI%2FML%20Engineer%20%7C%20B.Tech%20CSE&descAlignY=56&descSize=19" width="100%"/>

<a href="https://github.com/Vihangpatil37">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=21&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&multiline=true&width=760&height=90&lines=Building+a+real-time+hospital+OPD+queue+%26+registration+system;Socket.IO+%2B+Flutter+%2B+Next.js+%2B+Express;Final-Year+B.Tech+CSE+%40+Parul+University+(PIET);Also+shipping+SCPR+%E2%80%94+an+AI+career+guidance+platform" alt="Typing SVG" />
</a>

<br/>

[![Email](https://img.shields.io/badge/Email-vihangpatil37%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vihangpatil37@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Vihangpatil37-181717?style=for-the-badge&logo=github)](https://github.com/Vihangpatil37)
[![Portfolio](https://img.shields.io/badge/Portfolio-protfoliov.vercel.app-38BDF8?style=for-the-badge&logo=vercel&logoColor=white)](https://protfoliov.vercel.app)
![Profile Views](https://komarev.com/ghpvc/?username=Vihangpatil37&label=Profile%20Views&color=0e75b6&style=for-the-badge)

</div>

<br/>

## ⚡ About Me

```yaml
name:         Vihang Patil
role:         Full-Stack Developer & AI/ML Engineer
education:    B.Tech CSE, Parul University (PIET) — Class of 2027
focus:        Real-time systems · Multi-LLM orchestration · Explainable ML · Recommendation systems
flagship:     NextGen Hospital OPD Queue & Registration System — a real-time patient/queue platform for Shri Satya Sai Gramya Arogya Mandir
philosophy:   Engineer AI systems, don't just call APIs — auditability and explainability are non-negotiable
currently:    Deepening real-time system design, agentic AI architecture, and scalable backend engineering
```

- 🏥 Building the **NextGen Hospital OPD Queue & Registration System** — a real-time patient registration and queue management platform for **Shri Satya Sai Gramya Arogya Mandir**
- ⚡ Patients register via a native Flutter app, receive a live queue token, and hospital staff manage the queue from a real-time web dashboard — all synchronized via Socket.IO, no polling
- 🚀 Also the sole architect and developer of **[SCPR](#-other-projects)**, an AI-powered career guidance platform for Indian secondary-school students
- 🧠 I care about *engineering* systems properly — real-time sync, role-based auth, explainability, and multi-provider fallback are core to how I build
- 🛠️ Full-stack across Next.js/React, Node.js/Express/NestJS, Flutter, MongoDB, and Python ML tooling
- 🌐 Portfolio: **[protfoliov.vercel.app](https://protfoliov.vercel.app)** — "Liquid Glass Cosmos" UI, built with Next.js 15 + TypeScript + Framer Motion
- 📫 Reach me at **vihangpatil37@gmail.com**

<br/>

## 🏥 Flagship Project — NextGen Hospital OPD Queue & Registration System

<div align="center">

### [Real-time patient registration & OPD queue management](https://github.com/Vihangpatil37/NGO)

*Built for Shri Satya Sai Gramya Arogya Mandir — patients register on mobile, staff run the queue from a live dashboard*

</div>

<table align="center">
<tr>
<td align="center" width="33%">

**Stage 1**
### 📱 Patient Registration
Flutter app (Android/iOS) — new or returning patients register in Gujarati, Hindi, or English and receive an auto-incrementing queue token

</td>
<td align="center" width="33%">

**Stage 2**
### ⚡ Real-Time Queue Sync
Socket.IO broadcasts every registration, call, skip, and completion live — patient and staff screens update instantly, with no polling

</td>
<td align="center" width="33%">

**Stage 3**
### 📋 Staff Operations Dashboard
Next.js admin portal — staff Call Next / Skip / Complete patients, manage doctors, search records, and view live stats

</td>
</tr>
</table>

**How it works:** a patient opens the Flutter app, picks a language, and registers as new or returning — Socket.IO instantly pushes that registration and token to the admin dashboard. Staff work the live queue, calling, skipping, or completing patients, and the patient's app is notified the moment their token is called. Doctors log in through the same patient app with phone + PIN to set their daily availability, which shows up on the admin dashboard in real time.

| | |
|---|---|
| ⚡ **Real-time sync** | Socket.IO across patient app and admin dashboard — no polling, no refreshing |
| 📱 **Patient app** | Flutter (Android/iOS), Gujarati/Hindi/English localization, live token tracking |
| 📋 **Admin dashboard** | Next.js 15 + React 19 — queue control, patient search, doctor management, stats |
| 👨‍⚕️ **Doctor module** | Phone + PIN login, daily availability toggling, visible to staff in real time |
| 🔒 **Auth** | Three separate JWT flows — Staff (PIN, 8h), Patient (session, 24h), Doctor (phone + PIN + bcrypt, 24h) |
| 🕒 **Registration windows** | Configurable time-restricted windows (e.g. Sat 06:00 → Sun 06:00 IST) or 24/7 mode |
| 🔢 **Queue tokens** | Auto-incrementing, atomic counter per registration window |
| 📇 **Patient directory** | Full CRUD, searchable by name, phone, village, or case number |
| 📊 **Validation & logging** | Zod schema validation at the API layer, structured logging via Pino |

**Architecture:** the Flutter app and Next.js dashboard both talk to an Express 5 + TypeScript API over REST, with a parallel Socket.IO server handling real-time events; node-cron drives scheduled jobs; everything persists to MongoDB via Mongoose.

**Stack:** `Node.js` `Express 5` `TypeScript` `MongoDB` `Mongoose` `Socket.IO` `Next.js 15` `React 19` `Tailwind CSS` `Flutter` `Dart` `JWT` `bcrypt` `Zod` `Pino` `node-cron` `Luxon`

**Repo:** [github.com/Vihangpatil37/NGO](https://github.com/Vihangpatil37/NGO) · **License:** MIT

<br/>

## 🚀 Other Projects

<div align="center">

| Project | Description | Stack |
|---|---|---|
| 🧠 **[SCPR](https://github.com/Vihangpatil37/SCPR)** — Smart Career Path Recommendation System | Explainable, three-stage AI pipeline (deterministic eligibility/trait engine → multi-LLM re-ranking) guiding Indian Class 10 & 12 students to a career path; being written up for IEEE submission | `React` `NestJS` `Django` `MongoDB Atlas` `Scikit-learn` `XGBoost` `SHAP` `Gemini` `Groq` `Mistral` `GLM` |
| 🏎️ **[APEX F1](https://github.com/Vihangpatil37/APEX)** — Engineering Speed | F1-inspired web experience built around high-performance UI and motion design | `React` `Vite` `Tailwind` `Framer Motion` |
| 📚 **[Comic](https://github.com/Vihangpatil37/Comic-)** — Data Science, Illustrated | A data science education comic series, structured page-by-page to teach concepts like data preprocessing through story and character | `Markdown` `Gemini (image gen)` |

</div>

<br/>

## 🛠️ Tech Stack

<div align="center">

**Languages**
<br/>
<img src="https://skillicons.dev/icons?i=javascript,typescript,python,dart" />

**Frontend**
<br/>
<img src="https://skillicons.dev/icons?i=react,nextjs,html,css,tailwind,flutter" />

**Backend**
<br/>
<img src="https://skillicons.dev/icons?i=nodejs,express,nestjs,django" />

**Data, ML & Real-Time**
<br/>
<img src="https://skillicons.dev/icons?i=mongodb,python,pytorch,socketio" />

**Tools & Infra**
<br/>
<img src="https://skillicons.dev/icons?i=git,github,docker,bash,postman,figma,vercel" />

</div>

**Backend & real-time toolkit:** Express 5 · Socket.IO · JWT/bcrypt auth · Zod validation · Pino logging · node-cron
**AI/ML toolkit:** Scikit-learn · XGBoost · Pandas · SHAP (Explainable AI) · Multi-LLM orchestration (Gemini, Groq, Mistral, GLM) · Agentic AI design

<br/>

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Vihangpatil37&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="180"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vihangpatil37&layout=compact&theme=tokyonight&hide_border=true" height="180"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Vihangpatil37&theme=tokyo-night&hide_border=true&area=true" width="100%"/>

<img src="https://streak-stats.demolab.com?user=Vihangpatil37&theme=tokyonight&hide_border=true" />

<img src="https://github-profile-trophy.vercel.app/?username=Vihangpatil37&theme=tokyonight&no-frame=true&margin-w=10&row=1" />

</div>

<br/>

## 🌐 Connect With Me

<div align="center">

<a href="https://github.com/Vihangpatil37"><img src="https://img.shields.io/badge/GitHub-Vihangpatil37-black?style=for-the-badge&logo=github"/></a>
<a href="https://protfoliov.vercel.app"><img src="https://img.shields.io/badge/Portfolio-Liquid%20Glass%20Cosmos-38BDF8?style=for-the-badge&logo=vercel&logoColor=white"/></a>
<a href="mailto:vihangpatil37@gmail.com"><img src="https://img.shields.io/badge/Email-vihangpatil37%40gmail.com-red?style=for-the-badge&logo=gmail"/></a>

<br/><br/>

### 💭 Build. Break. Learn. Improve. Repeat.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,50:0f172a,100:1e3a8a&height=110&section=footer" width="100%"/>

</div>
