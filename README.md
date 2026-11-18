<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=58A6FF&center=true&vCenter=true&width=700&lines=Huzaifa+Sabah+Uddin;Backend+Engineer+%26+System+Architect;Real-time+Django+platforms%2C+shipped+to+production;%2415.6K%2Fyr+saved+%C2%B7+94%25+cost+cut" alt="Typing SVG" />

  <p>
    <a href="https://iamhuzaifasabahuddin.github.io/Portfolio/"><img src="https://img.shields.io/badge/Portfolio-58A6FF?style=for-the-badge&logo=About.me&logoColor=white" /></a>
    <a href="mailto:huzaifasabah@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
    <a href="https://linkedin.com/in/huzaifa-sabah-uddin"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
    <a href="https://github.com/Iamhuzaifasabahuddin"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  </p>

  <sub><a href="#-live-in-production">Live projects</a> · <a href="#-impact">Impact</a> · <a href="#-how-i-build">How I build</a> · <a href="#-tech-stack">Stack</a> · <a href="#-lets-build-something">Contact</a></sub>
</div>

<br />

```python
>>> from huzaifa import Engineer
>>> me = Engineer()
>>> me.role
'Backend Engineer & System Architect'
>>> me.live_in_production
['TopsoftDigitals Connect', 'Quillnest', 'BlinkDigitally']
>>> me.impact()
{'saas_savings': '$15.6K/yr', 'cost_reduction': '94%', 'revenue_protected': '$92.9K'}
>>> me.deadline_record
'100%: zero missed'
>>> me.motto
'Build systems, not just code. Automate workflows, not just tasks.'
```

---

## 🚀 Live in Production

> Real software, real users, running today. Click through and see it.

<table>
<tr>
<td>

### `01` &nbsp;⚡ TopsoftDigitals Connect
**Real-time project management platform for an agency: workspaces → clients → teams → tasks.**

<a href="https://production.topsoftdigitals.pk/"><img src="https://img.shields.io/badge/●_LIVE-production.topsoftdigitals.pk-2EA043?style=for-the-badge" /></a>

Built to replace Basecamp, Asana, Trello and a pile of Slack bots with **one in-house engine**, cutting tooling spend from **$1,400/mo to $90/mo** (94%) and saving **$15.6K/year**.

- **Real-time everywhere:** WebSocket notifications over Django Channels + Redis pub/sub, Web Push (VAPID) desktop alerts, and a 1:1 live chat with keyset pagination and reconnect handling
- **Approval-orchestrated workflow:** tasks move pending → awaiting approval → completed; clients auto-archive when their work is done
- **8-role RBAC** (admin, manager, PM, marketing, designer, developer, editor, publisher) scoped per workspace
- **Slack hub:** signature-verified slash commands (`/tasks`, `/requests`), batched DM delivery for every notification type, a daily pending-task digest
- **Support tickets with SLA clocks** per priority, breach highlighting and hourly escalation
- **Email alert scanner:** IMAP + Celery flags chargeback/refund/complaint mail with a 438-keyword single-pass regex
- **Sales & payments ledger**, `Ctrl+K` command palette, Asana import, installable PWA
- **Built for speed:** versioned Redis fragment caching with singleflight, zero N+1 in audited views, Brotli-compressed HTML (~70–80% smaller), presigned S3 uploads up to 500 MB, ~780 tests plus Locust and k6 load scenarios

<img src="https://img.shields.io/badge/Django_6.1-092E20?style=flat-square&logo=django&logoColor=white" /> <img src="https://img.shields.io/badge/Channels-WebSockets-4B8BBE?style=flat-square" /> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" /> <img src="https://img.shields.io/badge/Celery_·_gevent-37814A?style=flat-square&logo=celery&logoColor=white" /> <img src="https://img.shields.io/badge/HTMX-3366CC?style=flat-square&logo=htmx&logoColor=white" /> <img src="https://img.shields.io/badge/Slack_API-4A154B?style=flat-square&logo=slack&logoColor=white" /> <img src="https://img.shields.io/badge/Amazon_S3-569A31?style=flat-square&logo=amazons3&logoColor=white" /> <img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />

</td>
</tr>
<tr>
<td>

### `02` &nbsp;🪶 Quillnest · Client Portal
**One shared workspace for a publishing-services team and its clients.** Conversation, files, deliverables, approvals and signed agreements for every project, in one place.

<a href="https://usequillnest.com/"><img src="https://img.shields.io/badge/●_LIVE-usequillnest.com-2EA043?style=for-the-badge" /></a>

Runs **several publishing brands from a single Django app**. Staff see every brand; each client sees only their own brand and their own projects. The guiding idea: *nothing waits unnoticed*.

- **Client approvals:** deliverables complete only when the client approves; answers are final and the files shown are stored as immutable copies. Unanswered requests get reminders at 3 and 7 days
- **Built-in e-sign:** versioned terms, a signing audit trail (name, IP, timestamp, user agent, content hash) and a generated **PDF certificate**
- **"Whose move is it?"** A *Today* view ranks projects by who needs to act; a daily *Digest* surfaces clients who've gone quiet
- **Live chat & notifications** over WebSockets with an HTTP fallback; staff aliases so clients never see internal names
- **File versioning & previews:** image/PDF thumbnails decoded at reduced scale to keep memory low; direct-to-S3 browser uploads
- **No build step:** server-rendered templates + htmx, installable PWA, light/dark theme, `Ctrl+K` palette
- **1,000+ tests** covering access rules, caching, approvals, agreements and live-update paths

<img src="https://img.shields.io/badge/Django_6.1-092E20?style=flat-square&logo=django&logoColor=white" /> <img src="https://img.shields.io/badge/Channels_4.3-0C4B33?style=flat-square" /> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" /> <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" /> <img src="https://img.shields.io/badge/htmx-3D72D7?style=flat-square&logo=htmx&logoColor=white" /> <img src="https://img.shields.io/badge/PyMuPDF_·_fpdf2-555555?style=flat-square" /> <img src="https://img.shields.io/badge/Resend-000000?style=flat-square" />

</td>
</tr>
<tr>
<td>

### `03` &nbsp;📊 BlinkDigitally · Publishing Dashboard
**Production analytics platform (~6,000 LOC) that saves an editorial team 12+ hours a week of manual reporting.**

<a href="https://github.com/Iamhuzaifasabahuddin/BlinkDigitally"><img src="https://img.shields.io/badge/Repository-BlinkDigitally-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

- Real-time data from the Google Sheets API, aggregated across 7 sheets (USA, UK, Audio, Printing, Copyright, A+, Sales)
- Interactive Plotly visualisations, duplicate-client detection, Excel/PDF report generation
- Intelligent caching to keep a large multi-sheet dataset fast

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /> <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" /> <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" /> <img src="https://img.shields.io/badge/Google_Sheets-34A853?style=flat-square&logo=googlesheets&logoColor=white" />

</td>
</tr>
</table>

---

## 📈 Impact

<div align="center">
  <table>
    <tr>
      <td align="center" width="220"><h2>$15.6K</h2><sub>saved per year in SaaS licensing</sub></td>
      <td align="center" width="220"><h2>94%</h2><sub>tooling cost cut<br/>$1,400/mo → $90/mo</sub></td>
      <td align="center" width="220"><h2>$92.9K</h2><sub>revenue protected<br/>across 44 disputes</sub></td>
    </tr>
    <tr>
      <td align="center" width="220"><h2>5 → 1</h2><sub>tools replaced by a single engine</sub></td>
      <td align="center" width="220"><h2>1,700+</h2><sub>automated tests across<br/>the two live platforms</sub></td>
      <td align="center" width="220"><h2>100%</h2><sub>deadline record<br/>zero missed</sub></td>
    </tr>
  </table>
</div>

---

## 🧭 How I Build

```mermaid
flowchart LR
    U([Browser<br/>htmx · WebSocket · PWA]) --> A[ASGI<br/>Django + Channels]
    A --> P[(PostgreSQL)]
    A --> R[(Redis<br/>cache · sessions · pub/sub)]
    R --> W[Celery workers<br/>gevent pool]
    W --> N[Slack · Email · Web Push]
    A --> S[(S3<br/>presigned uploads)]
```

| Principle | What it looks like in practice |
|---|---|
| **Real-time by default** | WebSockets for live updates, with HTTP fallbacks so nothing breaks when a socket drops |
| **Heavy work goes async** | Emails, Slack DMs, scans and exports run in Celery, so requests stay fast |
| **Cache with intent** | Versioned keys bumped on write, TTL jitter, singleflight against stampedes |
| **Lean front end** | Server-rendered HTML + htmx, no SPA build pipeline to maintain |
| **Secure by design** | Role-scoped access rules, rate limits on every POST, sanitised rich text, signed webhooks |
| **Tested, then shipped** | Large isolated test suites, load tests, CI that blocks on missing migrations |

---

## 🛠 Tech Stack

<div align="center">

**Languages**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />

**Backend & Frameworks**<br/>
<img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
<img src="https://img.shields.io/badge/Django_Channels-0C4B33?style=for-the-badge&logo=django&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
<img src="https://img.shields.io/badge/htmx-3366CC?style=for-the-badge&logo=htmx&logoColor=white" />

**Data, Async & Messaging**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" />
<img src="https://img.shields.io/badge/Slack_API-4A154B?style=for-the-badge&logo=slack&logoColor=white" />

**DevOps & Cloud**<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
<img src="https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" />
<img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white" />
<img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />

</div>

---

## 📊 GitHub Analytics

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Iamhuzaifasabahuddin&theme=github_dark" width="95%" alt="Profile Details" />
</div>
<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Iamhuzaifasabahuddin&theme=github_dark" height="170em" alt="Stats" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Iamhuzaifasabahuddin&theme=github_dark" height="170em" alt="Languages" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Iamhuzaifasabahuddin&theme=github_dark" height="170em" alt="Commits" />
</div>

---

## 🔭 Currently Exploring

<div align="center">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Microservices-000000?style=flat-square&logo=protocols.io&logoColor=white" />
</div>

Event-driven architectures with Kafka and RabbitMQ · Kubernetes orchestration · microservice boundaries and scalable APIs · cloud-native deployment on AWS and GCP.

---

## 🤝 Let's Build Something

<div align="center">

I take products from **idea to production**: architecture, backend, real-time features, automation and deployment.<br/>
Open to freelance work, collaborations and technical discussions.

<a href="https://iamhuzaifasabahuddin.github.io/Portfolio/"><img src="https://img.shields.io/badge/Portfolio-58A6FF?style=for-the-badge&logo=About.me&logoColor=white" /></a>
<a href="mailto:huzaifasabah@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://linkedin.com/in/huzaifa-sabah-uddin"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>

<br/><br/>
<img src="https://komarev.com/ghpvc/?username=Iamhuzaifasabahuddin&style=flat-square&color=58A6FF" alt="Profile views" />
<br/>
<sub>Last updated: November 2026</sub>

</div>
