# Rama Charan

**Applied AI Engineer** · Bengaluru, India  
I build AI systems at the point where models meet software: **evaluation, reliability, multilingual NLP, and the backend that makes them usable.**

[Email](mailto:rama.charan.official@gmail.com) · [LinkedIn](https://www.linkedin.com/in/rama-charan-50425021b/) · [GitHub](https://github.com/Epik-Whale463)

---

### The kind of problems I like

```text
A model works once       → Can we make it work repeatedly?
An evaluation looks good → Are we measuring the right thing?
A prototype works        → Can someone actually use it?
```

I gravitate toward the less glamorous parts of applied AI: designing useful evaluations, tracing failure modes, reducing latency, integrating tools, and shipping systems that hold up outside a notebook.

## Selected work

### 01 / Evaluating a voice agent, not just demoing one
**Voice Agent Evaluation** · LiveKit · τ-bench Retail · Deepgram · Python

Built a retail voice agent against the **official τ-bench environment**, keeping its tool layer unchanged. Froze a baseline, identified three reproducible failure patterns, and tested one general prompt revision against the regression suite rather than patching individual tasks.

| What I measured | Result |
| :-- | :-- |
| Speech on progressive-disclosure tasks | **375 → 199 words** (~47% less) |
| Multi-item transaction plan | **Correct $107.09 net charge** |
| Spoken personal information | **Eliminated across 8 evaluated scenarios** |

The interesting part wasn't making the agent sound smarter. It was making it **say less, preserve task correctness, and avoid speaking sensitive information** under repeatable tests.

### 02 / Fine-tuning image generation within 16 GB VRAM
**SDXL Naruto Style Fine-Tune** · PyTorch · Diffusers · LoRA · bitsandbytes

Fine-tuned SDXL for a Naruto-inspired visual style on a **T4 (16 GB)**. Used precomputed VAE latents and CLIP embeddings, 8-bit AdamW, gradient checkpointing, and mixed precision to train at **1024 × 1024** without running out of memory.

```text
SDXL base parameters    2.57B
Trainable LoRA weights  46.4M  (1.78%)
Adapter checkpoint      93 MB
GPU training time       ~2.75 hours
```

A small adapter, not a new foundation model: the goal was to adapt style while retaining the base model's broader capabilities.

### 03 / Speech recognition that stays on your machine
**FlowOSS — Local-first Dictation** · Rust · Tauri · sherpa-onnx · Parakeet · Silero VAD

Built a desktop dictation MVP that captures audio, removes silence with VAD, transcribes **on-device** using an INT8 Parakeet model, and inserts the result into the active application.

The app is organized as a modular Rust workspace, with components for the CLI/daemon, tray, overlay, settings, model downloads, and selected-text assistance. Built platform adapters and packaging scripts for **Windows and Ubuntu/GNOME**.

---

## Previously, in production

**Pratilipi** · AI/ML Engineer Intern · Feb–Jun 2026

- **Setu:** Redesigned a literary-adaptation LLM pipeline for work across **12 Indian languages**. Recorded **58% fewer adaptation defects** at approximately **$0.27/chapter**, evaluated with a seven-dimension quality benchmark I designed.
- **Content classification:** Took an author-abandonment classifier to production on AWS: **90.5% accuracy on Hindi data**, with Kannada applicability despite no Kannada training examples; approximately **6,000 reviews/day**.
- **Performance:** Reduced translation turnaround **43 → 20 minutes** through parallel execution and an async database-session fix.
- **Platform engineering:** Addressed excessive auth-token requests through a Backend-for-Frontend caching approach; implemented scoped machine-to-machine access and cost tracking for a cross-team translation integration.

**AI4Bharat / IIT Madras** · Full Stack AI Intern · Oct 2025–Feb 2026

- Migrated **10 consumer apps** from a shared database design to tenant-isolated routing, data, auth, and onboarding on GCP.
- Shipped a multi-model **text-to-speech workflow** spanning API, backend batch orchestration, and UI controls.

<details>
<summary><strong>More experiments and earlier projects</strong></summary>

<br>

- **[KhetAI](https://github.com/Epik-Whale463/Capital-One_KhetAI)** — Agricultural query assistant with intent routing across six live tools. Tested with 10 farmers near my college and packaged as an Android APK.
- **[SpeechT5 Telugu TTS](https://huggingface.co/Epikwhale/speecht5_finetuned_telugu_charan)** — Fine-tuned on 8,576 Telugu samples, using transliteration to work with an English-oriented tokenizer. Validation loss **0.67 → 0.45**; 600+ model downloads. *Only loss-based evaluation was performed; see the model card for limitations.*

</details>

## My toolkit

| | |
| :-- | :-- |
| **Languages & backend** | Python, TypeScript, Rust, FastAPI, SQLAlchemy, async Python |
| **AI & evaluation** | PyTorch, Hugging Face, scikit-learn, LangGraph, tool use, RAG, LLM evals |
| **Speech & generation** | LiveKit, Deepgram, Diffusers, LoRA, sherpa-onnx |
| **Cloud & data** | AWS, GCP, Docker, PostgreSQL, MySQL, MongoDB, Qdrant, FAISS |

<details>
<summary><strong>Background and recognition</strong></summary>

<br>

**B.Tech, Artificial Intelligence & Machine Learning** · VVIT · 2026 · 8.5 CGPA  
AWS Certified AI Practitioner · NPCI Bharat AI Quest 2025 finalist · ISRO Bharatiya Antariksha Hackathon 2025 shortlist (top 140 teams)

</details>

---

**Currently interested in:** applied AI engineering, agent reliability, evaluation systems, multilingual AI, and local-first ML tools.  
**Reach me:** [rama.charan.official@gmail.com](mailto:rama.charan.official@gmail.com)
