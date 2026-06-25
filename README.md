# Rama Charan

AI/ML Engineer · Bengaluru

Building applied AI for Indic languages — LLM pipelines, evals, and the
backend that holds them up in production. Recently shipped Setu V2 at
Pratilipi, a multi-stage LLM adaptation pipeline now in org-wide review
for rollout across 12 Indic languages.

**Reach me:** rama.charan.official@gmail.com · [LinkedIn](https://www.linkedin.com/in/rama-charan-50425021b/) · [Resume](link-to-resume-if-hosted)

---

## What I work on

- Multi-stage LLM pipelines with evals — decomposition over monolithic prompting
- Multilingual NLP for Indic languages (translation, classification, TTS)
- Backend that makes ML actually ship — FastAPI, async, auth, deployment
- Eval and guardrail design for non-deterministic systems

## Selected work

**Setu V2** (private, Pratilipi) — 3-pass source-blind LLM adaptation pipeline
replacing a single-pass V1. Authored a 7-dimension evals benchmark; 58% fewer
adaptation defects on blind A/B with LLM-as-judge validated against human
reviewers. In org-wide review for rollout.

**ContentClosureFlow** (private, Pratilipi) — Multilingual author-abandonment
classifier (multilingual-e5-large + logistic regression) productionized as
a daily AWS Step Function. 90.5% cross-lingual accuracy after diagnosing
and fixing a label-leakage issue that took the first-pass score from 44.5%.

**[KhetAI](https://github.com/Epik-Whale463/Capital-One_KhetAI)** — Tool-augmented LLM
assistant for Indian agriculture queries. Intent-classified routing across
6 live API tools (weather, mandi prices, plant disease ID, geolocation,
news, LLM). Validated with 10 farmers near my college. Live as an Android APK.

**[SpeechT5 Telugu TTS](https://huggingface.co/Epikwhale/speecht5_finetuned_telugu_charan)** —
Fine-tuned SpeechT5 on 8,576 IndicTTS Telugu samples using a Telugu-to-Latin
transliteration shim so the English-trained tokenizer could process Telugu.
Validation loss 0.67 → 0.45. Open-sourced on Hugging Face; 600+ downloads.
Loss-based evaluation only — see model card for limitations.

## Stack

Python, TypeScript · PyTorch, Hugging Face, scikit-learn · FastAPI, Next.js,
async · AWS (Step Functions, S3, ECR), GCP · PostgreSQL, MySQL, MongoDB,
Qdrant · Auth0, SQLAlchemy

## Background

B.Tech AI/ML, VVIT (2026) · AI/ML Engineer Intern at Pratilipi (Feb-Jun 2026,
Firebolts team) · Full-stack AI Intern at AI4Bharat / IIT Madras (Oct 2025 –
Feb 2026)

AWS Certified AI Practitioner · NPCI Bharat AI Quest 2025 finalist ·
ISRO Bharatiya Antariksha Hackathon 2025 shortlist
