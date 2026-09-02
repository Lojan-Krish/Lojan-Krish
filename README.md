![Lojan Krishnapillai — Software Engineer, Web Developer, Graphic Designer, Jaffna Sri Lanka](banner.svg)

![Python](https://img.shields.io/badge/Python-171310?style=flat-square&logoColor=FF7A1A&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-171310?style=flat-square&logoColor=FF7A1A&logo=fastapi)
![Flask](https://img.shields.io/badge/Flask-171310?style=flat-square&logoColor=FF7A1A&logo=flask)
![scikit-learn](https://img.shields.io/badge/scikit--learn-171310?style=flat-square&logoColor=FF7A1A&logo=scikitlearn)
![Next.js](https://img.shields.io/badge/Next.js-171310?style=flat-square&logoColor=FF7A1A&logo=nextdotjs)
![React](https://img.shields.io/badge/React-171310?style=flat-square&logoColor=FF7A1A&logo=react)
![Node.js](https://img.shields.io/badge/Node.js-171310?style=flat-square&logoColor=FF7A1A&logo=nodedotjs)
![Express](https://img.shields.io/badge/Express-171310?style=flat-square&logoColor=FF7A1A&logo=express)
![Prisma](https://img.shields.io/badge/Prisma-171310?style=flat-square&logoColor=FF7A1A&logo=prisma)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-171310?style=flat-square&logoColor=FF7A1A&logo=postgresql)
![Socket.io](https://img.shields.io/badge/Socket.io-171310?style=flat-square&logoColor=FF7A1A&logo=socketdotio)
![Celery](https://img.shields.io/badge/Celery-171310?style=flat-square&logoColor=FF7A1A&logo=celery)
![Redis](https://img.shields.io/badge/Redis-171310?style=flat-square&logoColor=FF7A1A&logo=redis)
![Docker](https://img.shields.io/badge/Docker-171310?style=flat-square&logoColor=FF7A1A&logo=docker)
![Azure](https://img.shields.io/badge/Azure-171310?style=flat-square&logoColor=FF7A1A&logo=microsoftazure)
![C#](https://img.shields.io/badge/C%23-171310?style=flat-square&logoColor=FF7A1A&logo=csharp)
![.NET](https://img.shields.io/badge/.NET-171310?style=flat-square&logoColor=FF7A1A&logo=dotnet)
![SQL Server](https://img.shields.io/badge/SQL%20Server-171310?style=flat-square&logoColor=FF7A1A&logo=microsoftsqlserver)
![PHP](https://img.shields.io/badge/PHP-171310?style=flat-square&logoColor=FF7A1A&logo=php)
![WordPress](https://img.shields.io/badge/WordPress-171310?style=flat-square&logoColor=FF7A1A&logo=wordpress)
![MySQL](https://img.shields.io/badge/MySQL-171310?style=flat-square&logoColor=FF7A1A&logo=mysql)
![Tailwind](https://img.shields.io/badge/Tailwind-171310?style=flat-square&logoColor=FF7A1A&logo=tailwindcss)
![GSAP](https://img.shields.io/badge/GSAP-171310?style=flat-square&logoColor=FF7A1A&logo=greensock)
![Git](https://img.shields.io/badge/Git-171310?style=flat-square&logoColor=FF7A1A&logo=git)
![Figma](https://img.shields.io/badge/Figma-171310?style=flat-square&logoColor=FF7A1A&logo=figma)
![Canva](https://img.shields.io/badge/Canva-171310?style=flat-square&logoColor=FF7A1A&logo=canva)

**Jaffna, Sri Lanka** — open to roles in the UK and Europe, and remote freelance work worldwide.

BEng (Hons) Software Engineering — London Metropolitan University (UK), in progress.

![One person, no handoff: design, front end, back end, performance, technical SEO, DNS and mail](pipeline.svg)

![15+ production sites, 90+ PageSpeed, 446k lines of C#, 24k lines of PHP, 11 domains](stats.svg)

![Company work at BBK Partnership, and my own solo project](work.svg)

# My own projects

### Built solo — no client, no employer, no team

<details open>
<summary><b>CampusHub</b> — intelligent university management ecosystem · <b>~208,000 lines</b> · Next.js 14 · Express · Prisma · Python Flask · scikit-learn · Socket.io</summary>

My final-year BEng project: one platform covering grades, attendance, timetables, assignments, examinations, communication and student engagement across **nine roles** — Student, Parent/Guardian, Lecturer, Head of Department, Administrator, Registrar, Finance Officer, Librarian and Support/IT — with a machine-learning service that predicts GPA and flags at-risk students early.

| | |
|---|---|
| **Front end** | 608 files, **185,491 lines** — Next.js 14, 505 pages, 64 shared components, TailwindCSS |
| **Back end** | 136 files, **22,134 lines** — Express with 48 route modules over **83 Prisma models** |
| **ML service** | Python Flask, 502 lines — `RandomForestRegressor` (120 trees) trained on ~2,000 students, predicts end-of-semester GPA and maps it to LOW / MEDIUM / HIGH / CRITICAL risk with a confidence score, with a heuristic fallback if the model is unavailable |
| **Plagiarism** | TF-IDF + cosine-similarity matrix over submission texts, with automatic flagging |
| **Access control** | Capability-based RBAC — roles map to capabilities, so staff roles reuse admin features without hard-coding |
| **Auth** | One unified login that auto-routes by role: JWT, bcrypt, rate limiting, account lockout, email-OTP 2FA, SSO scaffolding |
| **Sessions** | Revocable device sessions and login history in a Security Centre — see active devices, sign out one or all others |
| **Smart attendance** | Rotating QR codes (30-second, TOTP-style) plus optional GPS radius verification, with manual override as fallback |
| **Timetable** | Automatic conflict detection across room, lecturer and offering overlap |
| **Online exams** | MCQ / true-false / short-answer builder, countdown, auto-grading, fullscreen and tab-switch violation logging, auto-submit, answer autosave and resume |
| **Real time** | Socket.io module channels, persisted history, typing indicators, live notifications |
| **Gamification** | XP, levels, streaks, 8 achievement badges, leaderboard |
| **Public site** | Full marketing site on the same app — 6 faculties, searchable course catalogue, news, events calendar, blog, research and publications, careers with CV upload, student-loan application |
| **Motion** | Hand-built GSAP + Lenis layer — smooth scroll, scroll-triggered reveals, magnetic buttons; honours `prefers-reduced-motion` with a `<noscript>` fallback |
| **SEO** | Per-page metadata, Open Graph and Twitter cards, JSON-LD, `sitemap.xml`, `robots.txt` |
| **Privacy** | Policy pages aligned to Sri Lanka's PDPA No. 9 of 2022 |
| **Tests** | Jest on the backend, Cypress on the front end |
| **Deployment** | Dockerfiles per service, `docker-compose` for the full stack |

The two parts I would defend hardest: the rotating QR attendance code, because a static QR is just a photograph somebody can send to a friend; and capability-based roles, because nine roles hard-coded as nine special cases becomes unmaintainable by the third one.

</details>

<details>
<summary><b>SmartMed Pharmacy Management System</b> · <b>446,000 lines</b> · C# 7.3 · .NET Framework 4.8 · Windows Forms · SQL Server · ADO.NET</summary>

| | |
|---|---|
| **Size** | 446,000 lines of hand-written C# across 871 files and 1,362 classes |
| **Hand-built UI** | Only 2 designer-generated files, so the entire Windows Forms interface is written by hand |
| **Architecture** | Four layers — presentation, service, repository over ADO.NET, data |
| **Components** | Owner-drawn custom control library, one BaseForm page pattern every screen inherits |
| **Auth** | PBKDF2-SHA256 password hashing, TOTP two-factor with QR enrolment |
| **Access** | Role-based access control |
| **Audit** | Hash-chained audit log |
| **Search** | Debounced multi-field search with a Levenshtein fallback; complexity documented |
| **SQL** | Parameterised throughout — 1,674 parameter bindings against 774 command executions |

Why hand-code a WinForms UI: the designer generates code you cannot read and will eventually have to debug, an owner-drawn control library gives you one place to change how everything looks instead of 400 forms each with their own idea, and a BaseForm pattern means a new screen inherits behaviour rather than copying it. The honest caveat — it is slower to start and only pays off past a certain size. Below that, use the designer.

</details>

<details>
<summary><b>Sri Lanka lottery results dataset</b> · Python · data pipeline · Excel/CSV</summary>

A clean, reproducible dataset of Sri Lankan lottery draws, built because no tidy version existed.

- **11,476 real draws** assembled from an MIT-licensed archive
- Styled Excel workbook and plain CSV as outputs, so it is usable by analysts and by code
- One update script with three modes — `pull`, `scrape` and `backfill` — so the set stays current without manual editing

The point of the three modes is that data pipelines rot. Pull for the fast path, scrape when the source shape changes, backfill when you find a gap in history.

</details>

[lojankrish.com](https://lojankrish.com) — my portfolio, also built and hosted by me.

---

# Company work

### BBK Partnership — Software Engineer &amp; Web Developer · Oct 2023 to present

Chartered accountants, three branches — Jaffna (120 staff), Vavuniya (60) and Colombo (20) — serving 1,000+ companies. Everything in this section was built in my role at the firm. The sites belong to the firm and its partners, not to me; I build them and I keep them running.

<details>
<summary><b>1 · Employee attendance &amp; monitoring platform</b> — internal, in development · Python 3.11 · FastAPI · PostgreSQL 15 · React 18 · Azure · Docker</summary>

Internal platform for 200 staff across three branches on six shift patterns running 9am to 1am.

| | |
|---|---|
| **Backend** | 99 Python files, 7,168 lines — 76 FastAPI routes across 18 endpoint modules, 18 SQLAlchemy models, 13 services |
| **Front end** | 67 files, 24,309 lines — 35 React pages, Vite, TailwindCSS |
| **Languages** | Trilingual i18n throughout — English, Sinhala, Tamil |
| **Identity** | Microsoft 365 SSO through Azure AD, OTP second factor |
| **Integrations** | Microsoft Teams camera-status monitoring via Graph API, TSheets attendance, automated email reporting |
| **Async** | Celery for scheduled work, Redis broker, WebSocket for live state |
| **Security** | AES-256 at rest, RBAC with an explicit access matrix, audit log on every action |
| **Deployment** | Azure (Singapore region), Docker, nginx, docker-compose with start/stop scripts |
| **Docs** | Six documents — API, ARCHITECTURE, DATABASE_SETUP, SECURITY, SETUP, TEAMS_API_SETUP |

</details>

<details>
<summary><b>2 · Support Our Schools — Sri Lanka Map plugin</b> · PHP · MySQL · REST API · PWA · i18n · Gutenberg</summary>

A WordPress plugin that became an application living inside WordPress. Currently v1.45.124 — that number is 124 patch releases of finding out what I got wrong.

| | |
|---|---|
| **Size** | 24,325 lines of PHP across 65 files, 18 module classes, one responsibility each |
| **Data** | 8 custom MySQL tables — schools, campaigns, events, supporters, activity log |
| **Surface** | 28 shortcodes, 30 AJAX endpoints, 7 REST API routes under its own namespace |
| **Roles** | Custom editor role with one capability — content yes, settings and secrets no |
| **No lockout** | Administrators hold that capability implicitly through a `user_has_cap` filter, so a migration or bad deactivation can never strip it and lock everyone out |
| **Offline** | PWA service worker and manifest |
| **Blocks** | Gutenberg blocks for the map and campaign embeds |
| **Ops** | XLSX export, scheduled digests, backup, cross-site sync |
| **Languages** | Full Tamil localisation (ta_LK, ta_IN) alongside English |

</details>

<details>
<summary><b>3 · HR data collection system</b> · Google Workspace · Apps Script</summary>

Staff data intake for all three branches, without buying a product for it.

- Google Forms front end, Apps Script behind it
- Creates a **private per-staff Drive subfolder** automatically on submission
- Branch-specific routing — Jaffna, Vavuniya and Colombo each land in their own folder tree

</details>

<details>
<summary><b>4 · Domain, hosting and mail migrations</b> · DNS · registrar transfers · zero-downtime cutover</summary>

- **LCN → Hostinger** — multiple live domains transferred, including supportourschool.org, with cancellation handled at the old registrar
- **Cloudflare → Hostinger** — tamilaid.org
- Registrar-locked and disputed-ownership recoveries, including declaration-form and identity verification processes
- MX cutovers planned so mail keeps flowing during the change

The interesting part of a migration is never the transfer itself. It is the order you do things in so that DNS propagation, SSL reissue and MX records do not leave a gap.

</details>

## Every domain I run

![11 domains: jaffnastallion.com and three aliases on one install, supportourschool.org and one alias, bbkca.lk, and four in progress](domains.svg)

| Domain | Serves | Status |
|---|---|---|
| [bbkca.lk](https://bbkca.lk) | BBK Partnership Chartered Accountants | Live · canonical |
| [jaffnastallion.com](https://jaffnastallion.com) | Jaffna Stallions Cricket Academy | Live · canonical |
| jaffnastallions.com | same install as above | Live · parked alias |
| jaffnastallion.lk | same install as above | Live · parked alias |
| jaffnastallions.lk | same install as above | Live · parked alias |
| [supportourschool.org](https://supportourschool.org) | Support Our Schools — education charity | Live · canonical |
| supportourschools.org.uk | same install as above | Live · parked alias |
| inovatejaffna.com | Zoho Mail live, staff mailboxes issued | Site in progress |
| in0v8jaffna.com | — | Site in progress |
| jaffnaartfestival.com | — | Site in progress |
| jaffnadirectory.com | — | Site in progress |

**Why aliases and not 301s.** A 301 sends the visitor somewhere else — second request, extra round trip, every alias a hop away from the real site. A parked domain alias serves the same WordPress install directly. The catch nobody mentions: several domains serving identical content is a duplicate-content problem unless the canonical tag points every variant at one preferred URL. So aliases for speed, canonical tags for search, and one place where the content actually lives.

**Mail.** Zoho Mail on inovatejaffna.com issues multiple staff mailboxes. Every other domain runs Hostinger's one-site-one-mailbox setup.

**Hosting.** Hostinger hPanel throughout — DNS records (A, CNAME, MX), SSL/TLS certificates, parked-domain configuration and mail routing are all mine to manage.

## Results across those builds

| | |
|---|---|
| **90+** | Google PageSpeed on 100% of deployments |
| **8s → under 2s** | load time, by WebP conversion first, then critical CSS inlined, then lazy loading, then server-side caching last |
| **60% faster / 20% lower bounce** | on the 360 Accountants rebuild |
| **150%** | organic search visibility lift for a client |
| **15+** | production sites shipped since 2023, every one from a blank page, every one still maintained |

---

# Previously

### 360 Accountants — Web Developer · Mar to Oct 2023

Rebuilt the company website. Pages around 60% faster, bounce rate down about 20%, roughly 50 defects cleared, organic search visibility up 150%, delivered in a fixed window. A different developer has taken it on since, so the live site may no longer be my build.

### Raks Engineering &amp; Technologies (Pvt) Ltd — Work Coordinator · Jan 2021 to Mar 2023

---

## What I work with

| | |
|---|---|
| **Backend & cloud** | Python 3.11 · FastAPI · Flask · Express · SQLAlchemy · Prisma · PostgreSQL · Celery · Redis · WebSocket · Socket.io · Docker · nginx · Azure · Azure AD SSO |
| **Machine learning** | scikit-learn · RandomForest regression · TF-IDF · cosine similarity |
| **Front end** | Next.js 14 · React 18 · Vite · TailwindCSS · GSAP · Lenis · JavaScript (ES6+) · HTML5 · CSS3 · i18n |
| **WordPress** | Custom themes · plugin engineering · modular components · multi-tenant hosting · Gutenberg blocks |
| **Also** | PHP · C# · .NET Framework · MySQL · SQL Server · MongoDB · REST APIs · Microsoft Graph API · Google Apps Script · Git |
| **Testing** | Jest · Cypress |
| **Performance & SEO** | Core Web Vitals · critical CSS · WebP · lazy loading · JSON-LD · canonical tags · sitemaps · Search Console |
| **Infrastructure** | hPanel/cPanel · DNS (A/CNAME/MX) · SSL/TLS · parked-domain aliases · registrar transfers · Zoho and Hostinger mail |
| **Design** | Canva (advanced, end to end) · Figma (UI layouts and prototypes) · Adobe Photoshop |

## Education

**BEng (Hons) Software Engineering** — ESOFT Metro Campus Jaffna, validated by London Metropolitan University (UK). In progress; final-year project **CampusHub** above.

---

## Reach me

[lojankrish.com](https://lojankrish.com) · [LinkedIn](https://linkedin.com/in/lojankrish) · lojankrish360@gmail.com · Jaffna, Sri Lanka
