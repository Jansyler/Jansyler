<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Outfit&weight=800&size=38&duration=2500&pause=1000&color=FFFFFF&center=true&vCenter=true&width=800&lines=JAN+HUBAL;FOUNDER+%26+FULL--STACK+ENGINEER;REAL--TIME+SYSTEMS+%C2%B7+AI+%C2%B7+MOBILE;BUILDING+SCALABLE+INFRASTRUCTURE" alt="Typing SVG" />

  <p align="center">
    <strong>Full-Stack Engineer building distributed real-time systems, AI-powered mobile apps, and SaaS products.</strong>
  </p>

  <p align="center">
    <a href="https://hubal.tech"><img src="https://img.shields.io/badge/PORTFOLIO-hubal.tech-FFFFFF?style=for-the-badge&logo=google-chrome&logoColor=000000" alt="Portfolio" /></a>
    &nbsp;
    <a href="mailto:sylerjan@gmail.com"><img src="https://img.shields.io/badge/EMAIL-sylerjan%40gmail.com-FFFFFF?style=for-the-badge&logo=gmail&logoColor=000000" alt="Email" /></a>
    &nbsp;
    <a href="https://linkedin.com/in/jan-hubal"><img src="https://img.shields.io/badge/LINKEDIN-jan--hubal-FFFFFF?style=for-the-badge&logo=linkedin&logoColor=000000" alt="LinkedIn" /></a>
    &nbsp;
    <a href="https://github.com/Jansyler"><img src="https://img.shields.io/badge/GITHUB-Jansyler-FFFFFF?style=for-the-badge&logo=github&logoColor=000000" alt="GitHub" /></a>
  </p>
</div>

<br />

<hr style="border: 0.5px solid #cccccc;" />

<br />

## ✦ SUMMARY

Full-Stack Engineer with 3 years of experience building distributed real-time systems, AI-powered mobile apps, and SaaS products. Founded three projects solo — including **RigRadar**, a live revenue-generating market intelligence platform. I thrive in small teams where I can own problems end-to-end, from scraping pipelines and fault-tolerant backends to cross-platform mobile apps.

> *Note: Most of my client work and proprietary SaaS platforms live in private repositories. This profile is a gateway to my public-facing projects and core competencies.*

<br />

## ✦ STARTUP VENTURES (FOUNDER & LEAD ENGINEER)

# 🛰️ RigRadar — Live Market Intelligence SaaS
> **Solo-built and launched from the ground up.** A distributed, real-time, revenue-generating market intelligence platform that automates web scraping, applies LLM-driven deal scoring, and broadcasts instant price alerts to subscribers.

| 🚀 Live Production SaaS | 💸 Revenue-Generating | 🤖 AI-Powered Forecaster | 🔄 Real-Time WebSockets |
| :--- | :--- | :--- | :--- |

---

## 🛠️ Tech Stack & Architecture

- **Backend Architecture:** Distributed Two-Service System (**Python** for data processing/AI & **Node.js** for API/orchestration)
- **Frontend:** Modern, responsive SPAs built with **JavaScript (ES6+)**, **HTML5**, and styled via **TailwindCSS**
- **Data & Message Layers:** **Redis** (Distributed Work Queue & Cache), **Pusher** (Real-Time WebSockets), **REST APIs**
- **AI/LLM Integration:** **Google Gemini (Google AI Studio)** with structured JSON schema outputs
- **External Monetization & Infrastructure:** **Stripe API** (Usage-Based Billing), **Resend** (Transactional Email), **Vercel** (Hosting & Serverless Deployment), B2B Affiliate Tracking (**Amazon & eBay Partner Networks**)

---

## 🏗️ Technical Deep Dive & System Design

### 1. Distributed Multi-Language Backend & Work Queue
* Designed and executed a decoupled **two-service backend architecture** to exploit the specific strengths of two languages: **Node.js** handles high-concurrency client authentication, API routing, and webhooks, while **Python** operates as the heavy-computational data engine.
* Interconnected both microservices via a high-throughput **Redis-backed work queue**, optimizing background worker distribution and eliminating single points of failure under sudden traffic bursts.
* Implemented a real-time event notification pipeline using **Pusher WebSocket channels**, dropping latency for live deal broadcast alerts to sub-second thresholds for connected active sessions.

### 2. Fault-Tolerant, Anti-Bot Scraping Pipeline
* Engineered a bulletproof ingestion engine capable of scraping volatile marketplace listings at scale while systematically routing requests through **ScraperAPI** to bypass aggressive Cloudflare/Akamai bot-protection walls.
* Built an **adaptive JS-rendering fallback mechanism** that switches to heavy headless browser rendering *only* when static HTML parsers fail, drastically optimizing API execution costs and speeding up scraping runs by up to 4x.
* Fortified the data collection architecture against network partitions and target site downtime by programming **resilient circuit breakers** and setting up a **Dead-Letter Queue (DLQ) retry matrix** with exponential backoff.

### 3. LLM-Driven Deal Scoring & Verification Engine
* Embedded **Google Gemini (via Google AI Studio)** directly into the data pipeline to execute real-time, comparative value-analysis, scoring deals from 1–100 and generating algorithmic price trend forecasts.
* Safeguarded against model hallucination by enforcing **strict output verification schemas** (Pydantic / JSON Schema validation), ensuring raw LLM tokens are structural matches for the database layer before persistence.

### 4. End-to-End Enterprise Monetization
* Constructed a robust, fully automated **Stripe billing ledger** supporting sophisticated **metered/usage-based subscription tiers**, computing costs dynamically based on user api-calls or active webhooks.
* Layered deep programmatic **B2B affiliate attribution tracking mechanisms** mapped to the **Amazon Associate** and **eBay Partner Network** frameworks, converting outbound user traffic into secondary passive revenue streams.

### 📱 TappedIN | AI-Powered E-Commerce Smart Search SaaS
*Dec 2025 – Present · Sole engineer*
# TappedIN | AI-Powered E-Commerce Smart Search SaaS

### 🚀 Project Overview
Traditional e-commerce search bars fail when shoppers search using abstract cultural terms, music artists, or subculture vibes (e.g., searching *"Central Cee look"* or *"Opium aesthetic"*). **TappedIN** is a standalone B2B SaaS platform that seamlessly integrates with Shopify storefronts. It allows shoppers to describe a vibe—or securely connect their streaming profiles—and instantly maps those music subcultures into targeted product recommendations straight from the merchant’s live inventory catalog.

---

### 🛠️ Key Features & Technical Achievements

* **Deterministic AI Extraction Engine:** Built a high-performance Python FastAPI backend utilizing the Google GenAI SDK (`gemini-2.5-flash`). Implemented strict Pydantic schemas (`response_schema`) and zero-temperature configurations to enforce structured JSON outputs, completely eliminating model hallucinations.
* **1-Click Music Profile Syncing:** Integrated Spotify and Apple Music OAuth APIs to securely ingest consumer listening histories (e.g., top 50 heavy-rotation artists) and dynamically translate aggregate subculture tags into automated visual style curations.
* **Data-Dense Merchant Control Room:** Designed a standalone Next.js (TypeScript) platform dashboard mirroring custom telemetry data. The frontend communicates with a PostgreSQL analytics database via FastAPI to draw live, stacked-revenue performance charts using Recharts, proving conversion rate metrics directly to merchants.
* **Automated Catalog Ingestion:** Engineered a lightweight background pipeline that processes raw inventory metadata from Shopify webhook endpoints, indexing product attributes into vector-ready categories for precise LLM semantic matching.

---

### 💻 Tech Stack

* **Backend:** `Python`, `FastAPI`, `Google GenAI SDK (Gemini)`, `Pydantic`, `PostgreSQL`, `Uvicorn`
* **Frontend:** `Next.js`, `React`, `TypeScript`, `Tailwind CSS`, `Recharts`
* **Integrations:** `Shopify Billing API`, `Shopify Admin Webhooks`, `Spotify Developer OAuth API`

### 📐 Sylenar — WordPress Page-Builder Plugin
*Jan 2023 – Jun 2025 · Sole engineer*
* **Visual Editor**: Built a WordPress page-builder plugin that replaces Elementor with an intuitive, MS Paint-style drag-and-drop interface — letting non-technical users design websites visually without code.
* **Engine**: Engineered the visual editor in JavaScript with real-time DOM manipulation and state management; built the plugin architecture in PHP to integrate with WordPress's hook and filter system.
* **Full Lifecycle**: Shipped a complete plugin — database migrations, option storage, custom post types, and the full publishing workflow.

<br />

## ✦ PROFESSIONAL EXPERIENCE

### Multi-Stack Software Engineer — NetMate CZ spol. s.r.o.
*Apr 2023 – May 2026*
* Led development across Java, Python, PHP, and JavaScript for diverse client projects; built automation scripts that reduced manual data-processing overhead.
* Deployed complex web platforms using hybrid WordPress/Elementor + custom PHP/JS stacks.
* Applied Wireshark for deep packet inspection and network troubleshooting across distributed environments.

### Full-Stack Developer & Systems Analyst — Oresi s.r.o.
*May 2024 – Dec 2024*
* Resolved complex latency issues using Wireshark packet analysis within enterprise infrastructure.
* Implemented heatmap analysis to optimize UX flows, directly improving conversion rates on high-traffic landing pages.

<br />

## ✦ CORE SKILL MATRIX

### 📁 Languages
<p align="left">
  <img src="https://img.shields.io/badge/JavaScript-CCCCCC?style=for-the-badge&logo=javascript&logoColor=000000" alt="JavaScript" />
  &nbsp;
  <img src="https://img.shields.io/badge/TypeScript-CCCCCC?style=for-the-badge&logo=typescript&logoColor=000000" alt="TypeScript" />
  &nbsp;
  <img src="https://img.shields.io/badge/Python-CCCCCC?style=for-the-badge&logo=python&logoColor=000000" alt="Python" />
  &nbsp;
  <img src="https://img.shields.io/badge/Java-CCCCCC?style=for-the-badge&logo=openjdk&logoColor=000000" alt="Java" />
  &nbsp;
  <img src="https://img.shields.io/badge/PHP-CCCCCC?style=for-the-badge&logo=php&logoColor=000000" alt="PHP" />
  &nbsp;
  <img src="https://img.shields.io/badge/HTML5%2FCSS3-CCCCCC?style=for-the-badge&logo=html5&logoColor=000000" alt="HTML5/CSS3" />
</p>

### 📁 Frontend & Mobile
<p align="left">
  <img src="https://img.shields.io/badge/React-CCCCCC?style=for-the-badge&logo=react&logoColor=000000" alt="React" />
  &nbsp;
  <img src="https://img.shields.io/badge/Next.js-CCCCCC?style=for-the-badge&logo=nextdotjs&logoColor=000000" alt="NextJS" />
  &nbsp;
  <img src="https://img.shields.io/badge/React_Native-CCCCCC?style=for-the-badge&logo=react&logoColor=000000" alt="React Native" />
  &nbsp;
  <img src="https://img.shields.io/badge/Expo-CCCCCC?style=for-the-badge&logo=expo&logoColor=000000" alt="Expo" />
  &nbsp;
  <img src="https://img.shields.io/badge/Tailwind_CSS-CCCCCC?style=for-the-badge&logo=tailwindcss&logoColor=000000" alt="TailwindCSS" />
</p>

### 📁 Backend & Infra
<p align="left">
  <img src="https://img.shields.io/badge/Node.js-CCCCCC?style=for-the-badge&logo=nodedotjs&logoColor=000000" alt="NodeJS" />
  &nbsp;
  <img src="https://img.shields.io/badge/FastAPI-CCCCCC?style=for-the-badge&logo=fastapi&logoColor=000000" alt="FastAPI" />
  &nbsp;
  <img src="https://img.shields.io/badge/MySQL-CCCCCC?style=for-the-badge&logo=mysql&logoColor=000000" alt="MySQL" />
  &nbsp;
  <img src="https://img.shields.io/badge/Redis-CCCCCC?style=for-the-badge&logo=redis&logoColor=000000" alt="Redis" />
  &nbsp;
  <img src="https://img.shields.io/badge/Distributed_Systems-CCCCCC?style=for-the-badge&logo=apachekafka&logoColor=000000" alt="Distributed Systems" />
</p>

### 📁 AI & ML
<p align="left">
  <img src="https://img.shields.io/badge/LangChain-CCCCCC?style=for-the-badge&logo=langchain&logoColor=000000" alt="LangChain" />
  &nbsp;
  <img src="https://img.shields.io/badge/LangGraph-CCCCCC?style=for-the-badge&logo=langgraph&logoColor=000000" alt="LangGraph" />
  &nbsp;
  <img src="https://img.shields.io/badge/LangFuse-CCCCCC?style=for-the-badge&logo=langfuse&logoColor=000000" alt="LangFuse" />
  &nbsp;
  <img src="https://img.shields.io/badge/RAG-CCCCCC?style=for-the-badge&logo=databricks&logoColor=000000" alt="RAG" />
  &nbsp;
  <img src="https://img.shields.io/badge/OpenAI_API-CCCCCC?style=for-the-badge&logo=openai&logoColor=000000" alt="OpenAI API" />
  &nbsp;
  <img src="https://img.shields.io/badge/Google_AI_Studio-CCCCCC?style=for-the-badge&logo=google&logoColor=000000" alt="Google AI Studio" />
</p>

### 📁 APIs, Protocols & Tooling
<p align="left">
  <img src="https://img.shields.io/badge/REST-CCCCCC?style=for-the-badge&logo=fastapi&logoColor=000000" alt="REST" />
  &nbsp;
  <img src="https://img.shields.io/badge/Stripe-CCCCCC?style=for-the-badge&logo=stripe&logoColor=000000" alt="Stripe API" />
  &nbsp;
  <img src="https://img.shields.io/badge/Pusher-CCCCCC?style=for-the-badge&logo=pusher&logoColor=000000" alt="Pusher" />
  &nbsp;
  <img src="https://img.shields.io/badge/Linux-CCCCCC?style=for-the-badge&logo=linux&logoColor=000000" alt="Linux" />
  &nbsp;
  <img src="https://img.shields.io/badge/Wireshark-CCCCCC?style=for-the-badge&logo=wireshark&logoColor=000000" alt="Wireshark" />
  &nbsp;
  <img src="https://img.shields.io/badge/Git-CCCCCC?style=for-the-badge&logo=git&logoColor=000000" alt="Git" />
</p>

<br />

## ✦ EDUCATION

* **B.Sc. in Computer Science** — Unicorn University *(2025 – Present)*
* **Computer Science & Graphic Design** — High School of Management and Graphic Design *(2021 – 2025)*

<br />

<hr style="border: 0.5px solid #cccccc;" />

<br />

<div align="center">
  <p><strong>✦ Architecting the future, one scalable system at a time. ✦</strong></p>
  <p align="center">
    <a href="https://hubal.tech" style="color: #ffffff; text-decoration: none; font-weight: bold;">PORTFOLIO</a>
    &nbsp;&nbsp;&nbsp;✦&nbsp;&nbsp;&nbsp;
    <a href="mailto:sylerjan@gmail.com" style="color: #ffffff; text-decoration: none; font-weight: bold;">CONTACT</a>
  </p>
</div>
