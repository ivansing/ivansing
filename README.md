# Ivan Duarte | Full-Stack Software Engineer

## About Me

Full-Stack Software Engineer and founder of ByteUp LLC, based in Bogotá, Colombia. Programming since 2011 (14 years), with 5+ years of focused production experience since 2021 — shipping SaaS products under the ByteUp brand and delivering contract engagements for clients in the US, Mexico, and Colombia.

My formal foundations came from NextU (Web Development, 2016), the UBC Software Development MicroMasters (Java, object-oriented design, software construction, 2017), and certifications from edX (Cloud Native Applications), CodeAcademy (Computer Science), and freeCodeCamp (Backend APIs). But the real education has been the active portfolio of ByteUp products and client systems I've shipped — 40+ real projects, with the majority kept private for client confidentiality or ongoing product development.

## Currently Working On

- **FixDoc** (v0.11.0 → v1.0.0) — multi-tenant document verification SaaS for mortgage and insurance
- **TroveTrends** ([trovetrends.com](https://trovetrends.com)) — live content platform, ongoing content and infrastructure work
- **Migratex** — maintaining the ETL CLI tool as a reusable product
- **Enterprise API integration contracts** — active Upwork and direct-client engagements (NDA)

## Featured Showcase Repositories

Public technical showcases for the ByteUp product line. Each repository contains architecture documentation, diagrams, metrics, and engineering details. Source code is proprietary — contact contact@byteup.co for demos or licensing.

| Product | Repository | Stack | Status |
|---|---|---|---|
| **FixDoc** — Document verification SaaS | [fixdoc-showcase](https://github.com/ivansing/fixdoc-showcase) | Next.js 16 · React 19 · TypeScript · Supabase · Stripe · OpenAI GPT-4o | Active development |
| **TroveTrends** — Content platform | [trovetrends-showcase](https://github.com/ivansing/trovetrends-showcase) | Next.js · TypeScript · Firebase Firestore · SendGrid · Tailwind | Live |
| **Migratex** — ETL CLI tool | [migratex-showcase](https://github.com/ivansing/migratex-showcase) | Python · Pandas · PostgreSQL · Supabase · Click | Production-ready |
| **Stripe Payment Links** — REST API | [stripe-payment-links-showcase](https://github.com/ivansing/stripe-payment-links-showcase) | Python · FastAPI · Stripe · SQLAlchemy 2.0 | Production-ready |
| **Voice Assistant** — IoT platform | [voice-assistant-showcase](https://github.com/ivansing/voice-assistant-showcase) | Python · Flask · React · Whisper · Piper · Raspberry Pi | Production v1.1.0 |

I specialize in SaaS platforms, API integrations, data migration systems, and e-commerce applications. I've built payment systems with both Stripe and PayPal, deployed across Vercel, Firebase, GCP, and AWS, and worked with databases ranging from PostgreSQL and MongoDB to Firebase Firestore and SQLite.

I work architecture-first. Before writing any code, I produce diagrams, roadmaps, and technical specs — C4 Model, DFD, UML, ERD — whatever the project needs to have a solid blueprint before development starts. That approach has saved me and my clients from costly rework every single time.

## Technical Stack

### Languages & Frameworks
- **Daily drivers:** TypeScript, JavaScript, Python, Node.js
- **Frontend:** Next.js (App Router), React, Tailwind CSS, shadcn/ui
- **Backend:** Next.js API Routes, Express.js, FastAPI, Flask
- **Mobile:** Flutter/Dart (Firebase + Bloc state management)
- **Foundational:** Java (UBC MicroMasters — OOP, software construction)

### Databases & Data Layer
- **PostgreSQL** — Supabase, Neon, Cloud SQL (RLS, triggers, Edge Functions, complex migrations)
- **MongoDB** — Mongoose ODM, aggregation pipelines, document modeling
- **Firebase Firestore** — compound indexes, security rules, real-time sync
- **SQLite / SQLAlchemy** — lightweight applications and API backends

### Auth & Security
- Supabase Auth, Firebase Auth, NextAuth.js, Google OAuth
- JWT sessions, OAuth2 (PKCE), Row Level Security
- Role-based access control, account lockout, audit logging

### Payments
- **Stripe** — subscriptions, checkout sessions, webhooks, customer portal, usage tracking, payment links with idempotent webhook handling
- **PayPal** — SDK integration, checkout flow, transaction capture, order management

### APIs & Integrations
- RESTful API design, Zod/Pydantic validation, OpenAI API, SendGrid, Twilio
- Shopify webhooks, third-party API integration with OAuth2 token management
- Rate limiting, retry logic with exponential backoff, error handling patterns

### Deployment & Infrastructure
- **Vercel** — serverless, edge functions, preview deployments
- **Firebase** — hosting, Cloud Functions, Firestore, Storage
- **Google Cloud Platform** — familiar with the ecosystem through Firebase
- **AWS** — S3, EC2, Lambda, Elasticsearch
- **Docker**, DigitalOcean, Raspberry Pi (IoT deployment)

### DevOps & Tools
- Git, GitHub (feature branch workflow + CI), WSL2 Ubuntu
- Jest, pytest, Postman automation scripts (98 tests on Migratex alone)
- PM2 process manager, Nginx reverse proxy

### AI Workflow
- Claude Code for accelerated implementation
- Claude Desktop with MCP integration for architecture planning and code review
- OpenAI API integration in production (FixDoc AI assistant)

## Production Projects

### FixDoc — Document Verification SaaS (In Development)
Multi-tenant platform for the mortgage industry built on Next.js, TypeScript, Supabase (PostgreSQL + RLS), and Stripe. Currently at v0.11.0 heading toward production release with a full versioned roadmap — 15 releases from v0.1.0 through v1.0.0 with dependency graphs and quality gates.

What's built: authentication with account lockout, multi-tenant organizations with RLS isolation on every table, 6-role RBAC system, CRM module, Stripe billing with 3 subscription tiers, project management with status workflows, document upload with Supabase Vault for PII, 3-layer fraud detection engine, OpenAI-powered AI assistant, real-time WebSocket updates, internal notes system, and admin dashboards with audit logging.

Stack: Next.js 16 · React 19 · TypeScript · Supabase · PostgreSQL · Stripe · Vercel · Zod · TanStack Query
Showcase: [fixdoc-showcase](https://github.com/ivansing/fixdoc-showcase)

### TroveTrends — Content Platform (Live)
Production platform built with Next.js 14, TypeScript, Firebase, Tailwind CSS, and shadcn/ui. Features server-side rendering for SEO, 12+ API route handlers, newsletter system with SendGrid (confirmation flow, welcome emails, unsubscribe), contact forms with Zod validation, React Hook Form, Recharts data visualization, and a full admin dashboard.

Live at trovetrends.com

Stack: Next.js 14 · React 18 · TypeScript · Firebase Firestore · SendGrid · Tailwind CSS · shadcn/ui · Recharts
Showcase: [trovetrends-showcase](https://github.com/ivansing/trovetrends-showcase)

### Migratex — ETL CLI Tool (Production Product)
Production-grade CLI tool I built for extracting, transforming, and loading data from Excel to PostgreSQL/Supabase. Originally developed as the migration framework for a retail client in Mexico that required moving **247,709 records across 99 sheets** from legacy Google Sheets/Zapier infrastructure to PostgreSQL with database triggers, Edge Functions, and Shopify webhook integration — delivered with a **99.96% success rate**. After delivery, I refactored the framework into a standalone reusable product with 98 tests, multi-region phone normalization (US, CO, MX, ES, AR, BR), FK dependency ordering, batch processing with progress tracking, fast COPY mode, and comprehensive validation.

Stack: Python · Pandas · PostgreSQL · Supabase · Shopify API · Click CLI
Showcase: [migratex-showcase](https://github.com/ivansing/migratex-showcase)

### Stripe Payment Links API
REST API for generating and managing payment links with Stripe Checkout integration. Built with FastAPI and SQLAlchemy, features idempotent webhook handling with duplicate event detection, payment status tracking, link expiration support, and clean modular architecture.

Stack: Python · FastAPI · Stripe API · SQLAlchemy · PostgreSQL
Showcase: [stripe-payment-links-showcase](https://github.com/ivansing/stripe-payment-links-showcase)

### Alejo — E-commerce Platform (Full System)
Complete e-commerce system with two applications: an admin dashboard for product/order/category management and a customer-facing storefront with shopping cart, PayPal checkout, and order tracking. Admin includes Google OAuth via NextAuth.js, image uploads to AWS S3 and Firebase Storage, and role-based access control. Frontend features persistent cart state, PayPal SDK integration, and server-side rendering.

Stack: Next.js · React · MongoDB · Mongoose · NextAuth.js · PayPal SDK · AWS S3 · Firebase Storage · Tailwind CSS

### Voice-Enabled Home Assistant (IoT Project)
Privacy-focused home automation system designed for Raspberry Pi deployment. Features offline voice processing (Whisper ASR + Piper TTS), real-time IoT control via GPIO, computer vision with OpenCV, rule-based automation engine, and a React dashboard with WebSocket communication. Built with a hardware abstraction layer for sensor monitoring and device control.

Stack: Python · Flask · React · WebSocket · OpenCV · Raspberry Pi · SQLite · Docker
Showcase: [voice-assistant-showcase](https://github.com/ivansing/voice-assistant-showcase)

### Liquor Store — Mobile E-commerce App
Cross-platform mobile app built with Flutter/Dart for the Colombian market. Features Firebase Firestore backend, Bloc state management, Google authentication, product catalog with category browsing, shopping cart, and admin panel built with React.

Stack: Flutter · Dart · Firebase Firestore · Bloc · React (Admin)

### Enterprise API Integration Projects (NDA)
Delivered production API integration contracts involving OAuth2 authentication with automatic token refresh, rate limit handling with backoff logic, multi-source credential management, and read-only data extraction from REST endpoints. Work included Python ETL pipelines and Java/Spring Boot OAuth2 PKCE implementations with full test coverage, Axios/TanStack Query integration, and documentation for handoff.

### Additional Projects
- **Automated Reporting System** — Python + PostgreSQL (Neon) + SendGrid email automation + PDF generation
- **SEO Assistant Chrome Extension** — JavaScript + Manifest V3, published on Chrome Web Store
- **Active portfolio** — 40+ real projects, the majority private for client confidentiality or ongoing product development

## Education & Certifications

- **UBC Software Development MicroMasters** — Java, object-oriented design, software construction (2017)
- **NextU** — Web Developer, Computer Science (2016)
- **edX** — Developing Cloud Native Applications, verified certificate (2022)
- **CodeAcademy** — Computer Science certification (2020)
- **freeCodeCamp** — Back End Development and APIs certification (2023)

## How I Work

I document before I code. Every project starts with architecture diagrams and technical specs — not because someone told me to, but because I learned the hard way that skipping this step costs 10x more later. My clients have specifically valued this approach, and it's how I built FixDoc from v0.1.0 through the current version without major rewrites.

I use AI tools daily — Claude Code for faster implementation, Claude Desktop for architecture planning and code review — but I drive the code myself. I review every line, I understand every decision, and I test everything before delivery. AI makes me faster, not lazier.

I've been writing about what I learn too — articles on dev.to and Medium covering graph-based data structures, OOP patterns, and development tools. Teaching is how I make sure I actually understand something.

Milestone-based payments preferred. Documentation included with every delivery.

## ByteUp LLC

Founder of ByteUp LLC. Building SaaS products for underserved markets and delivering contract development for clients who value clean architecture and reliable code.

## Connect

- **Company:** ByteUp LLC
- **Portfolio:** trovetrends.com
- **GitHub:** github.com/ivansing
- **LinkedIn:** linkedin.com/in/lance-dev
- **DEV.to:** dev.to/ivansing
- **Email:** contact@byteup.co
