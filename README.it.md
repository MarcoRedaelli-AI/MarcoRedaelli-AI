<div align="center">

[English](README.md) · **Italiano**

# Marco Redaelli

### AI Engineer & Runner

Costruisco prodotti AI, software e business digitali.<br>
Fondatore di **[iLeader](https://illeader.vercel.app/)** (consulenza AI per PMI italiane) e **[Marc_fitandrun](https://marcfitandrun.com)** (coaching per la corsa basato sui dati).

[![Website](https://img.shields.io/badge/iLeader-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://illeader.vercel.app/)
[![Marc_fitandrun](https://img.shields.io/badge/Marc__fitandrun-FC5200?style=for-the-badge&logo=strava&logoColor=white)](https://marcfitandrun.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/marco-redaelli-b26237221)
[![X](https://img.shields.io/badge/@Marco10Reda-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Marco10Reda)

</div>

---

## Chi sono

Sono un AI Engineer e vivo vicino al Lago di Como. Lavoro nel punto in cui i **large language model** incontrano i **problemi industriali reali**: aziende che producono oggetti fisici, con un ufficio tecnico che gira ancora su PDF e che non hanno mai messo un modello in produzione.

Nel concreto: pipeline RAG su documentazione interna disordinata, agenti collegati agli strumenti che l'azienda già usa, e training di modelli quando il task lo richiede davvero. In parallelo porto avanti due prodotti miei, e circa 80 km a settimana di corsa.

- Ingegneria della Produzione Industriale — Politecnico di Milano (polo di Lecco)
- PB maratona: **2h50** — che è anche il motivo per cui esiste MARC_AI
- Interessi attuali: workflow agentici, MCP, embodied AI, visibilità sui motori generativi

---

## Progetti in evidenza

### DecAI — Assistente RAG per una PMI manifatturiera

<img src="DecAI.jpg" width="100%" alt="Interfaccia dell'assistente conversazionale DecAI">

Assistente conversazionale interno costruito su una pipeline di **retrieval-augmented generation** sul catalogo tecnico di prodotto — **senza fine-tuning**. Il valore sta nel layer di retrieval, non nei pesi del modello: ingestion e chunking di documentazione tecnica eterogenea, embedding e ricerca vettoriale, reranking, e generazione di risposte ancorate ai documenti sorgente con citazioni verificabili.

Supporta la forza vendita nella qualificazione tecnica e nella costruzione dell'offerta, rispondendo sulla base del catalogo reale e non della memoria del modello.

<table>
  <tr>
    <td width="50%"><img src="DecAI1.jpg" width="100%" alt="DecAI vista retrieval"></td>
    <td width="50%"><img src="DecAI2.jpg" width="100%" alt="DecAI risposta con fonti"></td>
  </tr>
</table>

`Python` · `RAG` · `Vector Search` · `LangChain` · `LLM APIs`

---

### Altri progetti

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/3D-Editor-Deca-S.r.l.">
        <img src="3d-editor.png" width="100%" alt="Editor 3D GLB web">
      </a>
      <h3>Configuratore 3D di prodotto</h3>
      <p>Editor GLB in browser per la personalizzazione interattiva del prodotto. Gestione varianti, cambio materiali e rendering in tempo reale — pensato per sostituire il catalogo PDF statico in un processo di vendita B2B.</p>
      <p><code>React</code> <code>Three.js</code> <code>WebGL</code> <code>Cloudflare Pages</code></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/Unitree-G1-Robot">
        <img src="unitree-g1.png" width="100%" alt="Simulazione umanoide Unitree G1">
      </a>
      <h3>Unitree G1 — RL su umanoide</h3>
      <p>Integrazione SDK, simulazione e ambienti di reinforcement learning per l'umanoide Unitree G1. Training di policy di locomozione in Isaac Lab e MuJoCo, più script di configurazione e deploy.</p>
      <p><code>Python</code> <code>Isaac Lab</code> <code>MuJoCo</code> <code>RL</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://marcfitandrun.com">
        <img src="Immagine%202026-07-30%20150557.jpg" width="100%" alt="Sito Marc_fitandrun — home">
      </a>
      <a href="https://marcfitandrun.com">
        <img src="Immagine%202026-07-30%20150748.jpg" width="100%" alt="Sito Marc_fitandrun — piani di allenamento">
      </a>
      <h3>MARC_AI — Training Intelligence</h3>
      <p>Il motore dietro il mio brand di coaching. Legge la telemetria Strava e un profilo atleta a 18 variabili, poi genera e adatta i piani di allenamento. Include una pipeline automatica Strava → Instagram Stories.</p>
      <p><code>Python</code> <code>FastAPI</code> <code>Strava API</code> <code>PIL</code> <code>Claude API</code></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/marco2024redaelli-hash/Visualizzatore-STEP">
        <img src="step-viewer.png" width="100%" alt="Visualizzatore file STEP">
      </a>
      <h3>Visualizzatore STEP</h3>
      <p>Parser e viewer Python per file CAD STEP: estrazione geometrie, lettura metadati e conversione in mesh. Base per pipeline automatiche da CAD a web.</p>
      <p><code>Python</code> <code>OpenCascade</code> <code>CAD</code></p>
    </td>
  </tr>
</table>

**Anche qui:** [Openclaw](https://github.com/marco2024redaelli-hash/Openclaw) — guida HTML interattiva per installare e configurare OpenClaw su Raspberry Pi 4 · [Claude Project](https://github.com/marco2024redaelli-hash/Claude-Project) — esperimenti costruiti con le API Anthropic e MCP.

---

## Cosa so costruire

**Sistemi RAG** — l'intera pipeline: ingestion di documentazione reale e disordinata, strategie di chunking che tengono su contenuti tecnici, embedding e ricerca vettoriale, reranking, e generazione di risposte ancorate alle fonti recuperate anziché alla memoria del modello.

**Training di modelli** — fine-tuning di LLM open-weight (LoRA / QLoRA) quando il task lo richiede davvero, e reinforcement learning per il controllo robotico in Isaac Lab e MuJoCo. Ho imparato a essere onesto su quando serve addestrare e quando invece bastano retrieval o un prompting migliore.

**3D sul web** — configuratori di prodotto interattivi e viewer GLB/CAD in React e Three.js, comprese le pipeline che portano la geometria dal CAD al browser.

**Automazioni agentiche con Claude** — oltre un anno di lavoro quotidiano con Claude, da Claude 3 Opus fino a Opus 5: API, Claude Code e connettori MCP per collegare agenti ai sistemi che l'azienda già usa. La maggior parte di ciò che rilascio nasce così.


## Cosa faccio

**AI Engineering @ Deca Srl** — *2025 → 2026*<br>
Ho costruito **DecAI**, assistente conversazionale interno basato su una pipeline RAG sul catalogo prodotti — retrieval, reranking e generazione ancorata alle fonti con citazioni — a supporto della forza vendita nella qualificazione tecnica e nella costruzione dell'offerta. Ho realizzato anche il configuratore 3D web qui sopra e un'implementazione completa di **GEO** (`llms.txt`, dati strutturati JSON-LD, riscrittura dei contenuti), perché il catalogo aziendale venisse interpretato e citato correttamente dai motori di ricerca generativi.

**iLeader** — *Founder*<br>
Consulenza AI e sviluppo su misura per PMI italiane: assistenti conversazionali, RAG sulla documentazione interna e automazioni agentiche costruite su Claude con connettori MCP verso i sistemi che il cliente già usa — CRM, mail, gestionale, storage documentale. In aggiunta, lavoro di visibilità sui motori generativi.

**Marc_fitandrun** — *Founder & Running Coach*<br>
Coaching data-driven per corsa su strada e trail. Audit telemetrici della performance, programmi di coaching continuativo e uno stack di marketing che si automatizza da sé: contenuti social generati dalle attività Strava, newsletter settimanale e funnel di onboarding che alimenta direttamente MARC_AI.

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

### Parliamone

Disponibile per ruoli di AI engineering e progetti di consulenza — integrazione LLM, sistemi RAG, automazioni agentiche per PMI.

**marco2024redaelli@gmail.com**

<sub>Lecco, Italia · <i>Looking for the English version? <a href="README.md">Here</a>.</i></sub>

</div>
