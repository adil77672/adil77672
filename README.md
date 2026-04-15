# Adil Mustafa — Resume (README format)

**Headline:** Full Stack & Mobile Engineer · React Native · MERN · Next.js  

**Location:** Pakistan  

**Contact:** *(add email, phone with country code, LinkedIn, GitHub — do not commit secrets)*  

---

## Professional summary

Results-driven engineer with deep experience shipping **mobile apps (React Native / Expo)** and **web + API systems** (Node, Express, NestJS, Next.js). Comfortable across the stack: **REST APIs**, **auth (JWT, OTP, NextAuth, Supabase)**, **real-time** (WebSockets / Socket.io), **payments (Stripe)**, **cloud storage (S3, B2, Cloudinary)**, and **deployment** (PM2, nginx, Docker, AWS-oriented scripts).

Known for **production debugging** (Prisma query fixes, auth/OTP edge cases, chart/rendering bugs), **practical UX decisions** (e.g. replacing fragile `mailto:`-only flows with API-backed actions), and **multi-app / monorepo** work (marketplace + admin surfaces, tenant-scoped SaaS).

---

## Core technical skills

### Languages

JavaScript (ES6+), TypeScript, Python (Django ecosystem), SQL, Dart (Flutter — where used)

### Frontend & mobile

- **Web:** React, **Next.js** (App Router), **Vite**, Tailwind, Radix/shadcn, MUI, Ant Design  
- **Mobile:** **React Native** (CLI & Expo), **Expo Router**, navigation patterns, performance (lists, pagination)  
- **UI:** Form stacks (Formik, react-hook-form + Zod), i18n (e.g. i18next, react-native-localize)

### Backend

Node.js, **Express**, **NestJS**, Django, Flask (e.g. ML/API services), REST, OpenAPI/Swagger, Joi/Zod validation

### Data & ORM

**MongoDB** + Mongoose, **PostgreSQL**, **Prisma**, **Drizzle ORM**, **Supabase** (Auth, Postgres, RLS/RPC patterns), Redis (where present in stacks)

### Real-time & integrations

WebSockets, Socket.io, Django Channels, **Stripe**, PayPal (Medusa stacks), Facebook/OAuth flows, **AWS S3**, Backblaze B2, Cloudinary, OneSignal, Firebase (Auth/Firestore/Storage), **Livepeer** (streaming), **AI APIs** (OpenAI, Google GenAI), **vector search (Pinecone)** — *use only where you personally shipped*

### Mobile / device

**BLE** (e.g. react-native-bluetooth workflows), native module integration *(Voice Changer project)*, maps & notifications (Expo/React Native)

### DevOps & quality

Git, **Docker** / Compose, **PM2**, nginx, AWS (S3, ECR/ECS-style scripts in repos), CI awareness (e.g. Amplify), **Playwright** e2e, Node test runners, Jest

---

## Experience framing

**Mobile & full stack developer — freelance / project-based** *(add dates)*  

- Delivered end-to-end features on mobile and backend: APIs, auth, dashboards, deployments.  
- Integrated third-party services (payments, storage, OAuth, push).  
- Hardened production issues: API 500s, fragile client-only flows, OTP/form edge cases.  

*(Add employer names, contracts, and exact dates when you use this for ATS or LinkedIn.)*

---

## Highlight projects (portfolio narrative)

*Short descriptions below mix **your stated work** (BLE, job apps, civic/mood apps, S3, EasyStream ops, Playwright) with **repos present under your machine**. **Verify** you only list what you owned or materially contributed to.*

### Voice Changer (BLE)

**Type:** Real-time audio / Bluetooth mobile app  

**Highlights:** BLE connectivity, native module integration, voice effects (e.g. alien, child, speed), single-active-effect behavior  

**Stack:** React Native, BLE (e.g. react-native-ble-plx), native modules  

### SkillSphere Hub — job matching

**Type:** Job marketplace + admin  

**Highlights:** Listings, applications, geo-location, notifications, issue reporting, admin analytics  

**Stack:** React Native, Node.js, MongoDB  

### Metropolitan Management System

**Type:** Civic issue reporting  

**Highlights:** Citizen reports, status tracking, SPMP documentation  

**Stack:** MERN  

### Mood Checker App (MCA)

**Type:** Mood tracking / engagement  

**Highlights:** SDD, structured architecture, mood logging / analytics direction  

**Stack:** React Native, Node.js  

### AI + database hybrid

**Type:** Intelligent responses combining AI + structured data  

**Highlights:** Secure data flow, contextual retrieval *(Pinecone where applicable)*  

**Stack:** Node.js, AI APIs, vector DB  

### AWS S3 upload pipeline

**Type:** File upload & storage  

**Highlights:** Multer (or equivalent), S3 buckets, public/private policy patterns  

**Stack:** Node.js, AWS S3  

### EasyStream — backend & deployment

**Type:** Streaming product backend / ops  

**Highlights:** PM2, nginx, staging vs production, OAuth/debug work (e.g. Facebook login issues) per your notes  

**Stack:** Node.js, MongoDB, Socket.io, Livepeer ecosystem, Docker/PM2/nginx  

### Automated testing (e.g. task / todo flows)

**Highlights:** Playwright coverage for create, toggle, delete  

**Stack:** Playwright  

---

## Repository-backed projects *(from `~/projects` — confirm ownership)*

Each row is inferred from **README / `package.json`**. Add **your role**, **dates**, and **outcomes** before publishing.

| Project / folder | Role | Stack (summary) |
|------------------|------|------------------|
| **360 Living** (`360-living/`) | Full stack | **Next.js 16**, React, TanStack Query, Ant Design, Formik, Zustand · **Node/Express**, **Prisma**, JWT/Passport, Joi, Swagger `/api/v1`, PM2, Docker, Amplify-oriented web builds |
| **AgriMarket Connect** (`agri-market/`) | *(your role)* | **NestJS**, Prisma, PostgreSQL, WebSockets, JWT · **Vite/React** marketplace + **MUI** admin + retail admin |
| **BridgeBond** (`BridgeBond/`) | *(your role)* | **Express**, **MongoDB/Mongoose**, Stripe, OpenAI, **Pinecone**, S3, Merge, Firebase Admin, OneSignal · multiple **Vite/React** apps (web, client admin, super admin) |
| **EasyStream** (`easy-stream/`) | *(your role)* | **Expo/React Native** app · **Node/Express** backend, MongoDB, Socket.io, Livepeer |
| **Freedoms AI** (`freedoms/freedoms-webapp/`) | *(your role)* | **Next.js 14**, Supabase, Stripe, Radix, TipTap, boards/chat/notes, large internal docs |
| **Babu ISP** (`Babu/`) | *(your role)* | **Next.js 15** + Prisma + Supabase (web API only) · **Expo** mobile · Gemini AI · Playwright + API tests |
| **ArbShark** (`ARBShark/`) | *(your role)* | **Express**, Prisma, Supabase Postgres · Vite/React/shadcn frontend · Docker/ECS scripts |
| **Sayber** (`Sayber-Ai/`) | *(your role)* | **TypeScript/Express**, Drizzle, Postgres, Supabase, OpenAI, Swagger — HIPAA-oriented README |
| **Tennis trainer** (`Tennis-trainer/`) | *(your role)* | **Flask** + Docker + Redis + ML stack README · **Expo** mobile (Gluestack/video) |
| **Hydra** (`Hydra/hydra-lan-control-web-app/`) | *(your role)* | **Next.js 16**, React 19, Tailwind 4, Radix, SQLite, Socket.io, HLS |
| **pdf-medusa** (`pdf-medusa/`) | *(your role)* | **Medusa 2** backend, **Next.js** storefront, MUI, Meilisearch, Stripe/PayPal |
| **fruitful-hickory** (`fruitful-hickory/`) | *(your role)* | **Expo**, Drizzle, Supabase/PostGIS scripts, Mapbox, TanStack Query |
| **backblaze-backend** | *(your role)* | Express, **Backblaze B2**, Supabase client, Socket.io, FFmpeg |
| **barbershop-level-up** | *(your role)* | Next.js 14, NextAuth, MongoDB/Mongoose, Radix |
| **claude-telegram-bot** (repo name) | *(your role)* | Next.js 14, Prisma + SQLite, NextAuth, Capacitor, PDF tooling |
| **crane_app_react** | *(your role)* | Expo, **React Native Firebase**, multi-brand (Crane/Fortix) |
| **atlas-mobile-app-final-main** | *(your role)* | React Native CLI, Firebase messaging, Notifee |
| **GetIn scanner** (`Sacnneer App/`) | *(your role)* | Flutter app · **Express/TypeScript/Prisma** backend |
| **Workli** (`BD/workli-main/`) | *(your role)* | Expo 54, Expo Router, Supabase, maps, i18n |
| **LabelMates** (`BD/LabelMatesCde/`) | *(your role)* | Vite, React, shadcn, Supabase, Stripe, scanning libs |
| **Plateforme de recrutement** (`Platefomre-de-recrutement_Mohamed/`) | *(your role)* | **Django 5.2**, Channels, Celery, Redis, Stripe, Cloudinary |
| **AdArt** (`Personal/adart-updated/`) | *(your role)* | React Native + **Django** backend |
| **KineticKoach** | *(your role)* | Flutter + Firebase functions |
| **MyBackend** | *(your role)* | Express starter, MongoDB/Mongoose |
| **Next-js-Boilerplate-main** | *(your role)* | Next 16, Turbopack, TanStack Query, Radix, zod |
| **demo** | *(your role)* | Next 16, Drizzle, Supabase, pg |

*Exclude **official SDK clones** (e.g. a full `flutter/` SDK checkout) from “your projects” on a CV.*

---

## 360 Living — detailed contributions *(verifiable from this repo)*

**Product:** Property / school housing: admin + school portals, apartments, leases, invoices, maintenance, community, content.  

**Stack:** Next.js (App Router), TanStack Query, Ant Design, Zustand, Formik · Node/Express API **`/api/v1`**, Prisma, JWT/Passport, Joi, Swagger, PM2, Docker, nginx examples.  

**Examples of work themes:**

- Fixed **Prisma** usage that caused **500** errors on school/apartment **list & detail** endpoints.  
- **Apartment capacity requests:** server-backed **`POST /schools/:id/apartment-requests`**, plus **Gmail compose** and optional `mailto` — avoids relying on OS mail alone and reduces confusion with Chrome’s “(canceled)” `mailto` network rows.  
- **Auth:** forgot-password **OTP** UI guarded against undefined state.  
- **Charts:** occupancy/reporting charts hardened against **NaN** / single-point / gradient issues.  
- **Ops:** env-specific deploy patterns, monorepo split (`360-living-web` / `360-living-backend`).  

---

## Education & certifications

- *(Degree, institution, year)*  
- *(Certifications: AWS, Meta, etc.)*  

---

## Languages

- *(e.g. English — professional; Urdu — native; etc.)*  

---

## How to use this file

1. **Copy** to `~/projects/RESUME.md` or your portfolio repo if you prefer it outside 360 Living.  
2. **Delete or shorten** any project you did not work on.  
3. **Add metrics** only when true (latency, error rate, users, revenue).  
4. **Never commit** phone numbers, national IDs, or live API keys; keep `.env` out of git.  

---

## Disclaimer

This README merges **your described project history** with **technical signals from repositories** on your development machine. It is **not** a background check or employment record. Recruiters should verify scope and dates with you.

*Last structured update: April 2026 (assistant-generated; you should edit before sending to employers).*
