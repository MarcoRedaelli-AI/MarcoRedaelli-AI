<div align="center">

**English** · [Italiano](README.it.md)

# Marco Redaelli

### AI Engineer & Runner

Building AI products, software and digital businesses.<br>
Founder of **[iLeader](https://illeader.vercel.app/)** (AI consulting for Italian SMEs) and **[Marc_fitandrun](https://marcfitandrun.com)** (data-driven running coaching).

[![Website](https://img.shields.io/badge/iLeader-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://illeader.vercel.app/)
[![Marc_fitandrun](https://img.shields.io/badge/Marc__fitandrun-FC5200?style=for-the-badge&logo=strava&logoColor=white)](https://marcfitandrun.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/marco-redaelli-b26237221)
[![X](https://img.shields.io/badge/@Marco10Reda-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Marco10Reda)

</div>

---

## About

I'm an AI Engineer based near Lake Como, Italy. I work at the intersection of **large language models** and **real industrial problems** — the kind of company that makes physical products, has a paper-based technical office, and has never deployed a model in its life.

My day-to-day is building RAG pipelines over messy internal documentation, wiring agents into the tools a business already uses, and training models when the task actually calls for it. On the side I run two products of my own, and about 80 km a week on the road.

- Industrial Production Engineering — Politecnico di Milano (Lecco)
- Marathon PB: **2h50** — which is also the reason MARC_AI exists
- Currently interested in: agentic workflows, MCP, embodied AI, generative search visibility

---

## Featured Projects

### DecAI — RAG Assistant for a Manufacturing SME

<img src="DecAI.jpg" width="100%" alt="DecAI conversational assistant interface">

An internal conversational assistant built on a **retrieval-augmented generation** pipeline over a technical product catalogue — no fine-tuning involved. The value is in the retrieval layer, not in the weights: document ingestion and chunking of heterogeneous technical material, embedding and vector search, reranking, and grounded answer generation with citations back to the source documents.

It supports the sales team during technical qualification and quoting, answering product questions from the actual catalogue instead of from a model's memory.

<table>
  <tr>
    <td width="50%"><img src="DecAI1.jpg" width="100%" alt="DecAI retrieval view"></td>
    <td width="50%"><img src="DecAI2.jpg" width="100%" alt="DecAI response with sources"></td>
  </tr>
</table>

`Python` · `RAG` · `Vector Search` · `LangChain` · `LLM APIs`

---

### Other work

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/3D-Editor-Deca-S.r.l.">
        <img src="assets/3d-editor.png" width="100%" alt="Web-based 3D GLB editor">
      </a>
      <h3>Web 3D Product Configurator</h3>
      <p>Browser-based GLB editor for interactive product customisation. Variant handling, material swapping and real-time rendering, built to replace static PDF catalogues in a B2B sales process.</p>
      <p><code>React</code> <code>Three.js</code> <code>WebGL</code> <code>Cloudflare Pages</code></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/Unitree-G1-Robot">
        <img src="assets/unitree-g1.png" width="100%" alt="Unitree G1 humanoid simulation">
      </a>
      <h3>Unitree G1 — Humanoid RL</h3>
      <p>SDK integration, simulation and reinforcement learning environments for the Unitree G1 humanoid. Locomotion policy training in Isaac Lab and MuJoCo, plus configuration and deployment scripts.</p>
      <p><code>Python</code> <code>Isaac Lab</code> <code>MuJoCo</code> <code>RL</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://marcfitandrun.com">
        <img src="assets/marc-ai.png" width="100%" alt="MARC_AI telemetry analysis">
      </a>
      <h3>MARC_AI — Training Intelligence</h3>
      <p>The engine behind my coaching brand. Ingests Strava telemetry and an 18-variable athlete profile, then generates and adapts training plans. Includes an automated Strava → Instagram Stories content pipeline.</p>
      <p><code>Python</code> <code>FastAPI</code> <code>Strava API</code> <code>PIL</code> <code>Claude API</code></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/Visualizzatore-STEP">
        <img src="assets/step-viewer.png" width="100%" alt="STEP file viewer">
      </a>
      <h3>STEP File Viewer</h3>
      <p>Python parser and viewer for STEP CAD files — geometry extraction, metadata reading and mesh conversion. Groundwork for automated CAD-to-web pipelines.</p>
      <p><code>Python</code> <code>OpenCascade</code> <code>CAD</code></p>
    </td>
  </tr>
</table>

**Also here:** [Openclaw](https://github.com/marco2024redaelli-hash/Openclaw) — interactive HTML guide for installing and configuring OpenClaw on a Raspberry Pi 4 · [Claude Project](https://github.com/marco2024redaelli-hash/Claude-Project) — experiments built with the Anthropic API and MCP.

---

## What I Can Build

**RAG systems** — the full pipeline: ingesting messy real-world documentation, chunking strategies that survive technical content, embeddings and vector search, reranking, and answer generation grounded in retrieved sources rather than model memory.

**Model training** — fine-tuning open-weight LLMs (LoRA / QLoRA) when a task genuinely needs it, and reinforcement learning for robotic control in Isaac Lab and MuJoCo. I've learned to be honest about when training is the answer and when retrieval or better prompting is.

**3D on the web** — interactive product configurators and GLB/CAD viewers in React and Three.js, plus the pipelines that get geometry from CAD to browser.

**Agentic automation with Claude** — over a year of daily work with Claude, from Claude 3 Opus through Opus 5: the API, Claude Code, and MCP connectors wiring agents into the systems a business already runs. Most of what I ship is built this way.


## What I Do

**AI Engineering @ Deca Srl** — *2025 → 2026*<br>
Built **DecAI**, an internal conversational assistant powered by a RAG pipeline over the product catalogue — retrieval, reranking and grounded generation with source citations — supporting the sales team in technical qualification and quoting. Also delivered the 3D web configurator above, and a full **GEO** implementation (`llms.txt`, JSON-LD structured data, content rewriting) so the company's catalogue is correctly parsed and cited by generative search engines.

**iLeader** — *Founder*<br>
AI consulting and custom development for Italian SMEs: conversational assistants, RAG over internal documentation, and agentic automations built on Claude with MCP connectors into the systems a client already runs — CRM, mail, ERP, document storage. Plus generative search visibility work.

**Marc_fitandrun** — *Founder & Running Coach*<br>
Data-driven coaching for road and trail running. Telemetric performance audits, continuous coaching programmes, and a marketing stack that automates itself: Strava-triggered social content, a weekly newsletter, and an onboarding funnel that feeds straight into MARC_AI.

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

Open to AI engineering roles and consulting work — LLM integration, RAG systems, agentic automation for SMEs.

**marco2024redaelli@gmail.com**

<sub>Lecco, Italy · <i>Se cerchi la versione italiana, <a href="README.it.md">è qui</a>.</i></sub>

</div>
