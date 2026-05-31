# DopaReboot

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![GitHub Stars](https://img.shields.io/github/stars/dopareboot/dopareboot?style=social)
![Version](https://img.shields.io/badge/version-0.6.0--beta-brightgreen)

Rebuild your drive. Reclaim your reward system.  
DopaReboot is a privacy-first, open-source platform that helps you track, plan, and recover from dopamine desensitisation, anhedonia, and amotivational syndrome using evidence-backed protocols.

---

## Overview

Whether you’re recovering from stimulant overuse, managing treatment-resistant depression, or simply trying to optimise motivation and libido without tolerance, DopaReboot translates complex neuroscience into a daily companion app.

It combines:

- A **symptom & motivation tracker** that measures anhedonic and amotivational dimensions (consummatory vs anticipatory anhedonia).
- A **supplement & medication log** with half-life reminders, cycle scheduling (e.g., 9-Me-BC 30‑day cycles, low‑dose naltrexone ramp‑up), and tolerance‑break alerts.
- **Behavioural protocol templates** (dopamine detox, exercise dosing, cold exposure, sleep resensitisation).
- **Data visualisation** showing trends in mood, libido, energy, and receptor‑sensitivity proxies.
- **Local-first, end‑to‑end encrypted** storage – you own your data, no telemetry, no pharma ties.

DopaReboot is not medical advice; it’s a digital notebook built on the same dopaminergic recovery principles outlined in the scientific literature.

---

## Features

- 📊 **Daily drive & pleasure log** – Separate rating scales for anticipatory and consummatory anhedonia (based on SHAPS/TEPS).
- 💊 **Medication & supplement stack manager** – Drag‑and‑drop builder for pramipexole, bupropion, bromantane, uridine, NAC, etc., with dosing windows and half‑life warnings.
- 🔄 **Cycle & protocol wizard** – Pre‑loaded, editable protocols (post‑stimulant repair, DAWS taper, libido optimisation) with progress milestones.
- 🌡️ **Lifestyle tracking** – Log cold plunge sessions, HIIT workouts, sleep timing, sunlight exposure; correlates them with dopamine tone scores.
- 📈 **Correlation charts** – Automatically identify which interventions (e.g., morning light, tyrosine) correlate with your best days.
- 🧠 **Knowledge base** – Integrated offline wiki explaining mechanisms (D2 upregulation, autoreceptor blocking, BDNF, BH4 cycle) with citations.
- 🔒 **Local‑first privacy** – SQLite/IndexedDB backend, optional encrypted cloud sync via your own server.
- 🧩 **Extensible** – Plugin system for wearables (Oura, Apple Health) and community protocol sharing.

---

## Tech Stack

- **Frontend**: React / Next.js (PWA), Tailwind CSS, Recharts
- **Backend**: Rust (Axum) or Node (Fastify) – optional; fully functional offline
- **Database**: SQLite (local), PostgreSQL (optional sync server)
- **Encryption**: NaCl / libsodium for end‑to‑end sync
- **Containerisation**: Docker, docker‑compose for self‑hosting

---

## Quick Start

```bash
git clone https://github.com/dopareboot/dopareboot.git
cd dopareboot
cp .env.example .env
docker-compose up -d
```

Open `http://localhost:3000` – no account required.  
For a bare‑metal install, see [CONTRIBUTING.md](./CONTRIBUTING.md).

---

## Why DopaReboot?

Most habit trackers and mood apps treat dopamine as a black box. DopaReboot is the first open‑source tool specifically built for the millions of people dealing with:

- Post‑stimulant anhedonia (amphetamine, cocaine, caffeine overuse)
- Dopamine agonist withdrawal syndrome (DAWS)
- SSRI‑induced emotional blunting
- Treatment‑resistant depression with low drive

By putting the recovery protocols in your hands, we aim to create a transparent, clinician‑friendly ecosystem where users can safely experiment, learn, and heal – without vendor lock‑in or predatory marketing.

---

## Roadmap

| Milestone | Features |
|-----------|----------|
| **v0.6** (current beta) | Manual mood/motivation tracking, supplement log, basic protocol templates (bromantane cycle, LDN ramp) |
| **v0.7** | AI‑powered journal (local LLM via Ollama) that suggests interventions based on your logs and anhedonic subtype |
| **v0.8** | Community protocol marketplace – users can publish anonymised, evidence‑backed stacks; peer review via voting |
| **v0.9** | Biomarker integration – manual entry of prolactin, TSH, iron studies; correlation engine for lab‑to‑mood mapping |
| **v1.0** | Full wearable integration (Oura, Whoop, Apple Health) – automatic import of sleep stages, HRV, body temp |
| **v1.2** | Telehealth bridge – encrypted export for clinicians, pramipexole/MAOI scheduling alerts with prescription reminder |
| **v1.5** | Multi‑user support for researchers – aggregate anonymised data to identify real‑world recovery patterns |
| **v2.0** | Clinical‑grade digital therapeutic (pending regulatory compliance) – CBT‑based modules for anhedonia, guided behavioural activation |

---

## Contributing

We welcome contributors with expertise in neuroscience, addiction medicine, UX, or security. Start by reading our [CONTRIBUTING.md](./CONTRIBUTING.md) and the [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).

First good issues: protocol template builder improvements, chart library migration, language translations.

---

## Disclaimer

DopaReboot is an educational and self‑tracking tool only. It does not replace a doctor. Always consult a qualified healthcare professional before starting, stopping, or modifying any treatment. Data entered is not protected health information (PHI) unless you choose to self‑host in a compliant environment.

---

**License**: MIT  
**Project Link**: [https://github.com/dopareboot/dopareboot](https://github.com/dopareboot/dopareboot)

---

Let me know if you’d like me to flesh out any section further, or tailor the roadmap to a specific audience (e.g., clinicians, researchers, biohackers).
