# Adil Mustafa — Portfolio & Resume (README)

**Headline:** Full Stack & Mobile Engineer · React Native · MERN · Next.js  

**Location:** Pakistan  

**Contact:** *(email · phone + country code · LinkedIn · GitHub — do not commit secrets)*  

---

## How I work (role)

**Primary builder:** I **designed and implemented these products end-to-end** as the **solo lead developer** — architecture, mobile/web clients, APIs, data layer, integrations, and deployment where applicable.

**Contributors:** On **some** repositories, **other developers or collaborators** also committed code (features, reviews, or maintenance). Where that applies, I remained the **main owner** of delivery; you can list names per repo in interviews if needed.

---

## Professional summary

Engineer with a track record of shipping **production mobile apps (React Native / Expo)** and **full-stack web systems** (Next.js, Vite, Node, NestJS, Django). Strong in **REST APIs**, **auth** (JWT, OTP, NextAuth, Supabase), **real-time** (WebSockets, Socket.io, Channels), **payments** (Stripe and others), **object storage** (S3, B2, Cloudinary), and **ops** (PM2, nginx, Docker, AWS-style deploy scripts).

Known for **fixing production defects** (ORM/query bugs, auth edge cases, chart/math errors), **product-minded engineering** (e.g. API-first flows instead of brittle `mailto:`-only UX), and **multi-app monorepos** (marketplace + admin + retail, multi-tenant SaaS, enterprise surfaces).

---

## Core technical skills

| Area | Technologies |
|------|----------------|
| **Languages** | JavaScript, TypeScript, Python, SQL, Dart (Flutter) |
| **Web** | React, Next.js (App Router), Vite, Tailwind, Radix/shadcn, MUI, Ant Design |
| **Mobile** | React Native (CLI & Expo), Expo Router, navigation, performance |
| **Backend** | Express, NestJS, Django, Flask; REST; OpenAPI/Swagger; Joi/Zod |
| **Data** | PostgreSQL, MongoDB, Prisma, Drizzle, Supabase, Redis (where used) |
| **Realtime** | Socket.io, WebSockets, Django Channels |
| **Integrations** | Stripe, PayPal, OAuth/Facebook, Firebase, OneSignal, Livepeer, AI APIs, Pinecone (where used) |
| **Storage** | AWS S3, Backblaze B2, Cloudinary, Multer uploads |
| **Device** | BLE, native modules, maps, push notifications |
| **Quality & ops** | Playwright, Jest/Node tests, Docker, PM2, nginx, ECR/ECS-style scripts |

---

## A. Early / portfolio narrative projects *(mobile & full stack)*

*These are product stories you’ve described in your career narrative; align wording with what you shipped.*

### A1. Voice Changer (BLE)

| Field | Detail |
|-------|--------|
| **Type** | Real-time voice processing mobile app over **Bluetooth Low Energy** |
| **What you built** | BLE device workflow, **native module** hook for audio processing, effect pipeline |
| **Features** | Alien / child voice presets; speed (fast/slow); **only one effect active** at a time with clean switching |
| **Stack** | React Native, BLE (e.g. react-native-bluetooth-plx family), native modules |

### A2. SkillSphere Hub (job matching)

| Field | Detail |
|-------|--------|
| **Type** | Job marketplace + operations |
| **What you built** | Mobile app + APIs + **admin dashboard** |
| **Features** | Jobs, applications, **geo-location**, **notifications**, issue reporting; admin: users, listings, analytics |
| **Stack** | React Native, Node.js, MongoDB |

### A3. Metropolitan Management System

| Field | Detail |
|-------|--------|
| **Type** | Civic **issue reporting** for citizens vs response teams |
| **What you built** | Full MERN application + **SPMP** (software project management plan) documentation |
| **Features** | Report issues, locations, status tracking |
| **Stack** | MERN |

### A4. Mood Checker App (MCA)

| Field | Detail |
|-------|--------|
| **Type** | Mood tracking / engagement |
| **What you built** | **SDD** (software design document), architecture, app implementation |
| **Features** | Mood logging, engagement/analytics direction |
| **Stack** | React Native, Node.js |

### A5. AI + database hybrid system

| Field | Detail |
|-------|--------|
| **Type** | Responses that blend **LLM output** with **database-backed** answers |
| **What you built** | Backend orchestration, secure data paths, contextual retrieval |
| **Stack** | Node.js, AI provider APIs, vector DB (e.g. Pinecone) where integrated |

### A6. AWS S3 file upload system

| Field | Detail |
|-------|--------|
| **Type** | Scalable **image/file upload** |
| **What you built** | Upload APIs (Multer or equivalent), S3 integration, **bucket policies** (public/private) |
| **Stack** | Node.js, AWS S3 |

### A7. EasyStream — backend & deployment

| Field | Detail |
|-------|--------|
| **Type** | Streaming product **backend + DevOps** |
| **What you built** | Environment-based **staging/production**, **nginx**, **PM2**, debugging (e.g. Facebook/OAuth issues) |
| **Stack** | Node.js, MongoDB, Socket.io, Livepeer-related stack, Docker |

### A8. Automated testing (task / todo flows)

| Field | Detail |
|-------|--------|
| **Type** | E2E regression suite |
| **What you built** | **Playwright** tests: create task, toggle complete, delete |
| **Stack** | Playwright |

---

## B. Repository projects — full detail *(solo lead; contributors on some repos)*

Below: **folder path**, **product summary**, **architecture**, **stack**, **notable capabilities** (from README / `package.json`).  

---

### B1. 360 Living — `360-living/`

| Field | Detail |
|-------|--------|
| **Product** | Property / school **housing platform** (Dubai-market positioning): admin + school portals, apartments, leases, invoices, maintenance, community, content/blog |
| **Architecture** | Monorepo: **`360-living-web`** (Next.js) + **`360-living-backend`** (Express API ` /api/v1`) |
| **Web stack** | Next.js 16, App Router, React, **TanStack Query**, **Ant Design**, Formik, Zustand, Tailwind tooling, ESLint/Prettier/Husky |
| **API stack** | Node (ESM), Express, **Prisma**, **Passport JWT**, Joi, Winston, **Swagger** `/api/v1/docs`, PM2, Docker, nginx examples |
| **Domains** | Schools, apartments, leases, financial invoices, **apartment-requests** (persisted), reports, auth (incl. OTP/forgot password), content endpoints |
| **Delivery** | AWS Amplify-oriented web builds; env-specific backend (`development` / `staging` / `production`) |
| **Examples of engineering** | Prisma fixes for **500s** on school/apartment list & detail; **API-first** apartment requests + Gmail fallback vs `mailto:`-only; OTP UI hardening; chart **NaN/single-point** fixes; deploy script patterns |

---

### B2. AgriMarket Connect (ATI) — `agri-market/`

| Field | Detail |
|-------|--------|
| **Product** | **Agricultural marketplace** connecting producers and clients (regional / Cameroon focus in docs); separate **staff/retail** consoles |
| **Architecture** | One **NestJS API** + **three React+Vite** frontends |
| **Backend** | **NestJS 10**, **Prisma**, **PostgreSQL**, **WebSockets** (Socket.io), JWT refresh, **Swagger** `/api`, throttling, scheduling, Google Generative AI dep, Jest |
| **WebApp** (`WebApp Repo /`) | Vite, React, TypeScript, Tailwind, **HashRouter**, **socket.io-client**, PWA plugin, guests + CLIENT + PRODUCER; **blocks staff roles** from consumer app |
| **Admin Panel** | Vite, React, **MUI** (Minimal kit base) |
| **Retail admin** | Vite, React (retail operations) |
| **Pattern** | Clean architecture layers: domain → application → infrastructure → controllers |

---

### B3. BridgeBond — `BridgeBond/`

| Field | Detail |
|-------|--------|
| **Product** | **Enterprise** org hierarchy (orgs → departments → users), **multi-tenant**, RBAC, **OTP** auth, **AI chat**, billing/HRIS/notifications docs |
| **Backend** (`bridge-bond-backend`) | **Express**, **MongoDB/Mongoose 8**, JWT, Joi, **Stripe**, **OpenAI**, **Pinecone**, **AWS S3**, **Merge** API, **Firebase Admin**, Cloudinary, Nodemailer, **OneSignal**, Swagger, Winston, **Jest**, PM2, Docker scripts |
| **bridgebond_web** | Vite, **React 19**, **Tailwind 4**, Ant Design, TanStack Query, Firebase client, i18n, react-hook-form, zod |
| **bridgebond_client_admin** | Vite, React 19, Stripe.js, ApexCharts, OneSignal, Headless UI |
| **bridgebond_super_Admin** | Vite, React 19, Ant Design, ApexCharts, TanStack Query, Tailwind 3 |
| **Other** | `bridgebond_landing_page`, Firebase **functions** subpackage |

---

### B4. EasyStream — `easy-stream/`

| Field | Detail |
|-------|--------|
| **Product** | **Simulcast** streaming (e.g. YouTube + Facebook); webcam/OBS-style flows |
| **Mobile** (`easystream-app`) | **Expo**, **Expo Router**, React Native, **EAS** build scripts, dev client, native Android/iOS workflows |
| **Backend** (`easystream-backend`) | Node (ESM), **Express**, **MongoDB**, **Socket.io**, **Livepeer**, OAuth for platforms, stream CRUD, analytics hooks, PM2 deploy scripts |

---

### B5. Freedoms AI — `freedoms/freedoms-webapp/`

| Field | Detail |
|-------|--------|
| **Product** | **AI journaling** product: notes, **chat**, boards/tasks, projects, automations, **subscription** gating |
| **Stack** | **Next.js 14**, React 18, TypeScript, **Supabase** (Auth, Postgres, RPCs), **Stripe**, **Radix**, **TipTap**, **xyflow**, **dnd-kit**, Markmap, Mixpanel, Vercel Analytics, OneSignal, wavesurfer, TikTok server route patterns |
| **Docs** | Large `docs/`: routes, OpenAPI subset, RLS/RPC, SOW traceability |

---

### B6. Babu ISP — `Babu/`

| Field | Detail |
|-------|--------|
| **Product** | **Multi-tenant ISP SaaS**: super admin, per-tenant admin/staff, customers; plans with customer limits |
| **Web** (`web/`) | **Next.js 15**, **React 19**, **Prisma 6**, **Supabase** DB, **Ant Design**, TanStack Query, **Google GenAI**, Cloudinary, Firebase, Zod+Formik, Recharts, **Playwright** + **Node API tests** — **only** service touching DB |
| **Mobile** (`mobile/`) | **Expo 52**, Expo Router, TanStack Query, Formik, **OneSignal**, Paper, charts — **HTTP to web API only** |

---

### B7. ArbShark — `ARBShark/`

| Field | Detail |
|-------|--------|
| **Product** | **Sports betting arbitrage / +EV** domain: events, markets (odds JSON), opportunities |
| **Backend** (`ArbShark-Backend-main`) | **Express**, **Prisma**, **Supabase Postgres**, JWT, bcrypt, Joi, Helmet, rate limit, Jest, **Docker/ECR/ECS** npm scripts |
| **Frontend** (`ArbShark-Frontend`) | **Vite**, React, **shadcn/Radix**, TanStack Query, **Supabase**, **Stripe** |

---

### B8. Sayber — `Sayber-Ai/`

| Field | Detail |
|-------|--------|
| **Product** | **Healthcare/FHIR-oriented** backend (HIPAA mentioned in README) |
| **sayber-ai-backend** | **TypeScript**, **Express**, **Drizzle**, **PostgreSQL**, **Supabase** client, **OpenAI**, Swagger UI, sessions, multer |
| **Sayber_Windsurf** | Monorepo with `backend/` + root tooling |
| **Sayber_Windsurf_App** | **Gemfile** (Ruby) + **package.json** (JS/RN ecosystem) — mobile or hybrid shell |

---

### B9. Tennis trainer — `Tennis-trainer/`

| Field | Detail |
|-------|--------|
| **Product** | **Video analysis** API + mobile client |
| **tennis-trainer-live** | **Python Flask**, **Docker Compose**, **Redis**, **PM2** inside container, **YOLO/MediaPipe**-class README, deploy scripts |
| **tennis-mobile-app** | **Expo 52**, Expo Router, **Gluestack**, **expo-video**, Jest |

---

### B10. Hydra LAN control — `Hydra/hydra-lan-control-web-app/`

| Field | Detail |
|-------|--------|
| **Product** | LAN/control-style **web dashboard** (local server pattern) |
| **Stack** | **Next.js 16**, **React 19**, **Tailwind 4**, Radix, **better-sqlite3**, bcrypt, **jose**, **Socket.io** + client, **HLS.js**, Recharts, Zod, custom **`server.js`** entry |

---

### B11. pdf-medusa — `pdf-medusa/`

| Field | Detail |
|-------|--------|
| **Product** | **Headless commerce** (Medusa) + Next storefront |
| **pdf_backend** | **Medusa 2.x** framework, **TypeScript**, **AWS S3**, **PayPal** SDK, OpenTelemetry/pg, Jest |
| **pdf_frontend** | **Next.js** starter storefront, **MUI**, **Meilisearch** instant search, **Stripe**, **PayPal**, Medusa JS SDK |

---

### B12. Fruitful Hickory — `fruitful-hickory/`

| Field | Detail |
|-------|--------|
| **Product** | **Expo** app with **maps** and rich DB scripting |
| **Stack** | **Expo ~54**, React Navigation, **Drizzle** + drizzle-kit, **Supabase**, **Mapbox** (`@rnmapbox/maps`), **PostGIS**-related SQL npm scripts, TanStack Query, Neon serverless driver |

---

### B13. Backblaze video backend — `backblaze-backend/`

| Field | Detail |
|-------|--------|
| **Product** | **Video/rushes** hosting API using **B2** |
| **Stack** | **Express**, **backblaze-b2**, **Supabase** JS client, **Socket.io**, multer/busboy, **fluent-ffmpeg**, helmet, rate-limit |

---

### B14. Barbershop Level Up — `barbershop-level-up/`

| Field | Detail |
|-------|--------|
| **Product** | Salon **levelup-salon** web app |
| **Stack** | **Next.js 14**, **NextAuth**, **MongoDB/Mongoose**, Radix, react-hook-form + zod, seed scripts |

---

### B15. Claude Telegram bot (repository name) — `claude-telegram-bot/`

| Field | Detail |
|-------|--------|
| **Product** | Next app with **mobile wrapper** and document tooling |
| **Stack** | **Next.js 14**, **Prisma 7** + **better-sqlite3**, **NextAuth** Prisma adapter, **Capacitor** Android, **react-pdf / jsPDF / html2canvas**, Zustand |

---

### B16. Crane / Fortix — `crane_app_react/`

| Field | Detail |
|-------|--------|
| **Product** | **White-label** Expo app (**Crane** vs **Fortix** via env) |
| **Stack** | **Expo**, **React Native Firebase** (app, auth, firestore, storage), hook-form + zod, native document pickers |

---

### B17. Atlas — `atlas-mobile-app-final-main/`

| Field | Detail |
|-------|--------|
| **Product** | **Two** RN apps: **Atlas** + **AtlasEmployee** |
| **Stack** | **React Native 0.80**, **React 19**, **Firebase** app + messaging, **Notifee**, React Navigation native stack |

---

### B18. GetIn Scanner — `Sacnneer App/`

| Field | Detail |
|-------|--------|
| **Product** | Scanner **Flutter** client + **TypeScript API** |
| **GetIn-ScannerApp** | **Flutter** (`pubspec.yaml`) |
| **Getin-Scanner-be** | **Express**, **TypeScript**, **Prisma**, tsx, PM2-friendly build copy |

---

### B19. Workli — `BD/workli-main/`

| Field | Detail |
|-------|--------|
| **Product** | **Expo** app with location and notifications |
| **Stack** | **Expo 54**, **Expo Router 6**, **React 19**, **Supabase**, maps, **expo-notifications**, **i18next**, hook-form + zod |

---

### B20. LabelMates — `BD/LabelMatesCde/`

| Field | Detail |
|-------|--------|
| **Product** | **Vite** SPA — retail/label **scanning** orientation (barcode/OCR libs in deps) |
| **Stack** | **Vite**, React, TypeScript, **shadcn/Radix**, **Supabase**, TanStack Query, **Stripe** |

---

### B21. AUOST — `BD/AUOST APP/`

| Field | Detail |
|-------|--------|
| **auost-main** | **Flutter** |
| **auost-main-2** | **Vite + React** (template-era README) |

---

### B22. Plateforme de recrutement — `Platefomre-de-recrutement_Mohamed/`

| Field | Detail |
|-------|--------|
| **Product** | Full **recruitment** platform (matching, messaging, payments, gamification, NGO module — per README) |
| **Stack** | **Django 5.2**, **Channels** + **Redis**, **Celery**, **PostgreSQL** (prod) / SQLite dev, **Stripe**, Cloudinary, django-allauth, large Python stack |

---

### B23. AdArt / FineArt — `Personal/adart-updated/`

| Field | Detail |
|-------|--------|
| **Product** | **React Native** client + **Django** API |
| **Stack** | RN CLI, navigation, Android Gradle; **FineArt-Backend** Django (`manage.py` workflows in npm scripts); **Gemfile** for Ruby tooling |

---

### B24. Kinetic Koach — `KineticKoach-project/KineticKoach/`

| Field | Detail |
|-------|--------|
| **Product** | **Flutter** app (`kinetic_koach_mine`) |
| **Stack** | Dart 3.8+, GetX, flutter_svg, etc.; **Firebase functions** package under project |

---

### B25. MyBackend — `MyBackend/`

| Field | Detail |
|-------|--------|
| **Product** | **Starter** Express API (GitHub-style boilerplate name in package.json) |
| **Stack** | Express, **MongoDB/Mongoose**, nodemon |

---

### B26. Next.js Boilerplate — `Next-js-Boilerplate-main/`

| Field | Detail |
|-------|--------|
| **Product** | Opinionated **Next 16** starter (author field references your GitHub handle in manifest) |
| **Stack** | Next 16, **Turbopack** dev, React 19, TanStack Query, Radix, react-hook-form + zod, next-themes, Husky |

---

### B27. demo — `demo/`

| Field | Detail |
|-------|--------|
| **Product** | **Next** app with **Drizzle** migrations & seeds |
| **Stack** | **Next 16**, React 19, **Drizzle** + **pg**, **Supabase** clients, QRCode.react, scripts for migrate/seed |

---

### B28. Nested experiment — `BD/07ba4202-df52-45bd-a303-3a7011452d2b (1)/`

| Field | Detail |
|-------|--------|
| **Note** | Folder contains **root + backend** `package.json` — treat as imported **Node** experiment or client deliverable; describe in interviews if you shipped it |

---

## C. What to exclude from “your projects” on a CV

- **`flutter/`** at repo root if it is the **official Flutter SDK** (thousands of `pubspec` files) — not a personal app.  
- **`.zip` archives**, **`dump/`**, empty shells — unless you actively develop them.  

---

## Education & certifications

- *(Degree, institution, year)*  
- *(Certifications)*  

---

## Languages

- *(e.g. English — professional; Urdu — native)*  

---

## File usage

1. Edit **contact**, **dates**, and **contributors’ names** where you want specificity.  
2. Remove **B28** or any folder you did not lead.  
3. Never commit **`.env`** or live secrets.  

---

*Last update: April 2026 — structured for Adil Mustafa; solo lead framing per your instructions; contributors noted where repos are shared.*
