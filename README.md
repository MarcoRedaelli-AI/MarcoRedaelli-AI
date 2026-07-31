<div align="center">

**English** · [Italiano](README.it.md)

# Marco Redaelli

### AI Engineer & Runner — Lecco, Italy

Building AI products, software and digital businesses.<br>
Founder of **[iLeader](https://illeader.vercel.app/)** (AI consulting for Italian SMEs) and **[Marc_fitandrun](https://marcfitandrun.com)** (data-driven running coaching).

[![Website](https://img.shields.io/badge/iLeader-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://illeader.vercel.app/)
[![Marc_fitandrun](https://img.shields.io/badge/Marc__fitandrun-FC5200?style=for-the-badge&logo=strava&logoColor=white)](https://marcfitandrun.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/marcoredaelli-ai)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/Marco20262026)
[![X](https://img.shields.io/badge/@Marco10Reda-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Marco10Reda)

</div>

---

## About

I'm Marco Redaelli, an AI Engineer based near Lake Como, Italy. I work at the intersection of **large language models** and **real industrial problems** — the kind of company that makes physical products, has a paper-based technical office, and has never deployed a model in its life.

My day-to-day is building RAG pipelines over messy internal documentation, wiring agents into the tools a business already uses, and training models when the task actually calls for it. On the side I run two products of my own, and about 80 km a week on the road.

- Industrial Production Engineering — Politecnico di Milano (Lecco)
- Based in Valgreghentino, province of Lecco — working with SMEs across Lombardy
- Marathon PB: **2h50** — which is also the reason MARC_AI exists
- Currently interested in: agentic workflows, MCP, embodied AI, generative search visibility

---

## Featured Projects

Three of these were built for **Deca Srl**, a manufacturer of industrial feeding systems: a retrieval assistant, a 3D sales tool, and a generative-search visibility layer. The fourth is my own product.

---

### 1 · DecAI — RAG Assistant for a Manufacturing SME

<img src="DecAI_1.png" width="100%" alt="DecAI conversational assistant answering product questions from a technical catalogue">

An internal conversational assistant built on a **retrieval-augmented generation** pipeline over a technical product catalogue — no fine-tuning involved. The value is in the retrieval layer, not in the weights: document ingestion and chunking of heterogeneous technical material, embedding and vector search, reranking, and grounded answer generation with citations back to the source documents.

It supports the sales team during technical qualification and quoting, answering product questions from the actual catalogue instead of from a model's memory. The assistant is scoped to the company's own products: it declines rather than improvises when a question falls outside the catalogue.

`Python` · `RAG` · `Vector Search` · `LangChain` · `LLM APIs`

---

### 2 · DECA 3D Editor — Product Configurator with an Embedded AI Assistant

<a href="https://glb-3d-editor.pages.dev/"><img src="3d-editor_3.png" width="100%" alt="Browser-based GLB product configurator with the DecAI assistant docked alongside the 3D viewport"></a>

A browser-based GLB/GLTF editor for industrial feeding systems, built to replace a static PDF catalogue in a B2B sales process. Variant handling, material swapping, real-time rendering, a shareable viewer, and 3D generation from a photo or a text description.

In its current version the configurator and the RAG assistant are a single product: DecAI sits inside the editor, so a prospect can ask which size fits their application, have the model opened in the 3D viewer from the answer itself, and go from there to a quote request — without leaving the page or waiting on a sales rep.

`React` · `Three.js` · `WebGL` · `Cloudflare Pages` — [live demo](https://glb-3d-editor.pages.dev/) · [repository](https://github.com/MarcoRedaelli-AI/3D-Editor-Deca-S.r.l.)

---

### 3 · GEO — Making a Manufacturer Machine-Readable

<img src="geo-deca.png" width="100%" alt="ChatGPT, Claude and Gemini — the generative engines this structured-data work targets">

Generative engines cite what they can parse. This manufacturer's delivered systems lived in two places that never spoke to each other: a spreadsheet of case-study records, and a network archive of 3D models organised by component rather than by job order. Nothing connected a record to its actual project files, and nothing on the public pages told a model what any of it was.

I inventoried the archive component by component and linked every record to its real files, then built a navigable prototype catalogue — a hundred pages across 35 product families, grouped by product acronym so that site, spreadsheet and archive finally share one hierarchy.

Then the finding that mattered. Forty-two structured-data files had been written and were valid — and not one of them was on a page. No `application/ld+json` block existed anywhere in the published source. Correct content, living in a spreadsheet, invisible to every crawler.

So I generated the real thing: a single linked graph of **65 nodes** covering the company entity, the collection page, 19 per-family lists and 42 product schemas. Twelve invented properties — outside the schema.org vocabulary, therefore silently ignored by validators — became **334 `PropertyValue` entries** under `additionalProperty`: same content, correct container. Standard properties the models actually read (`url`, `sku`, `brand`, `manufacturer`, `isSimilarTo`) were populated from data already sitting in the sheet. Verified before delivery: 65 unique identifiers, 294 internal references resolved, zero terms outside the vocabulary.

The point isn't keywords. It's that a supplier's real, specific, verifiable work becomes retrievable evidence a model can ground an answer in.

`JSON-LD` · `Schema.org` · `llms.txt` · `Static Site Generation` · `Firebase Hosting`

---

### 4 · MARC_AI — Training Intelligence

<a href="https://marcfitandrun.com"><img src="marc-ai.png" width="100%" alt="Marc_fitandrun coaching platform powered by the MARC_AI training engine"></a>

The engine behind my own coaching brand. It ingests Strava telemetry and an 18-variable athlete profile, then generates and adapts training plans. Around it sits a marketing stack that runs itself: a Strava-triggered pipeline that renders activity data into Instagram Stories, a weekly newsletter, and an onboarding funnel that feeds straight back into the model.

`Python` · `FastAPI` · `Strava API` · `PIL` · `Claude API` — [marcfitandrun.com](https://marcfitandrun.com)

---

### Other work

- [**Unitree G1 — Humanoid RL**](https://github.com/MarcoRedaelli-AI/Unitree-G1-Robot) — SDK integration, simulation and reinforcement learning environments for the Unitree G1 humanoid. Locomotion policy training in Isaac Lab and MuJoCo. `Python` `Isaac Lab` `MuJoCo` `RL`
- [**STEP File Viewer**](https://github.com/MarcoRedaelli-AI/Visualizzatore-STEP) — Python parser and viewer for STEP CAD files: geometry extraction, metadata reading, mesh conversion. Groundwork for CAD-to-web pipelines. `Python` `OpenCascade` `CAD`
- [**Openclaw**](https://github.com/MarcoRedaelli-AI/Openclaw) — interactive HTML guide for installing and configuring OpenClaw on a Raspberry Pi 4.
- [**Claude Project**](https://github.com/MarcoRedaelli-AI/Claude-Project) — experiments built with the Anthropic API and MCP.

---

## What I Can Build

**RAG systems** — the full pipeline: ingesting messy real-world documentation, chunking strategies that survive technical content, embeddings and vector search, reranking, and answer generation grounded in retrieved sources rather than model memory.

**Model training** — fine-tuning open-weight LLMs (LoRA / QLoRA) when a task genuinely needs it, and reinforcement learning for robotic control in Isaac Lab and MuJoCo. I've learned to be honest about when training is the answer and when retrieval or better prompting is.

**3D on the web** — interactive product configurators and GLB/CAD viewers in React and Three.js, plus the pipelines that get geometry from CAD to browser.

**Generative search visibility (GEO)** — structured data, `llms.txt`, and content architecture that makes a company's real work retrievable and citable by AI search engines rather than invisible to them.

**Agentic automation with Claude** — over a year of daily work with Claude, from Claude 3 Opus through Opus 5: the API, Claude Code, and MCP connectors wiring agents into the systems a business already runs. Most of what I ship is built this way.

---

## What I Do

**AI Engineering @ Deca Srl** — *2025 → 2026*<br>
Delivered the three projects above: DecAI, the 3D configurator, and the GEO implementation — a retrieval assistant for the sales team, a browser-based sales tool replacing the PDF catalogue, and a structured-content layer that makes the company's production history citable by generative search engines.

**iLeader** — *Founder*<br>
AI consulting and custom development for Italian SMEs: conversational assistants, RAG over internal documentation, and agentic automations built on Claude with MCP connectors into the systems a client already runs — CRM, mail, ERP, document storage. Plus generative search visibility work.

**Marc_fitandrun** — *Founder & Running Coach*<br>
Data-driven coaching for road and trail running. Telemetric performance audits, continuous coaching programmes, and the automated marketing stack described above.

---

## Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Claude](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=three.js&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

</div>

---

<div align="center">

### Let's talk

Open to AI engineering roles and consulting work — LLM integration, RAG systems, generative search visibility, agentic automation for SMEs.

**marco2024redaelli@gmail.com**

<sub>Marco Redaelli · Lecco, Italy · <i>Se cerchi la versione italiana, <a href="README.it.md">è qui</a>.</i></sub>

</div>
