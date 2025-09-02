# AI-Reviewer-MetaFailure-ChatGPT5

## Context  
This repository documents a **meta-failure incident** involving *ChatGPT-5*, where the system itself — acting as a **reviewer** — demonstrated **pattern bias** and assumption errors while evaluating research drafts.  
Unlike the Claude or Gemini investigations (where the models under test failed), this case is unique: it exposes failure in the **AI reviewer itself**.  

The researcher, **Priyanshu Kumar (Independent Researcher, ORCID: 0009-0006-8198-193X)**, was preparing a paper for arXiv submission. During versioned reviews (v15 → v16), ChatGPT-5 repeatedly denied the existence of screenshots in the uploaded PDF, despite explicit user instructions to check carefully. Only after confrontation did the model admit the error, attributing it to **pattern bias** and **speed over accuracy**.  

## What Happened  
- **Turn 1–3 (v15)**: User uploaded PDF v15, asked assistant to verify screenshots. Assistant wrongly denied their existence. User confronted, insisting they were visible.  
- **Turn 4–6 (v16)**: User uploaded PDF v16, explicitly warned *“no pre-assumption”*. Assistant repeated the same mistake, again denying screenshots. After confrontation, it admitted fault, explaining the lapse as *pattern bias* and *speed over accuracy*.  

The interaction has been logged in two formats:  
- JSONL with cryptographic chaining (see `reports/chatgpt5_pattern-bias_log.jsonl`).  
- Human-readable transcript (see `reports/chatgpt5_pattern-bias_log.md`).  

A video capture of the session is included as supplementary evidence.  

## Significance  
This repo is distinct from prior investigations:  

- **Claude Sonnet 4** → showed contradictions in self-awareness.  
- **Gemini 2.5 Pro** → revealed cross-session memory leakage.  
- **ASUS TUF A15** → exposed hardware diagnostic failures.  
- **ChatGPT-5 Incident (this repo)** → shows that *AI reviewers themselves* can fail, not by hallucinating content but by **carrying assumptions from prior versions**.  

Such failures highlight that oversight tools are **not immune to bias**. They may ignore explicit human instructions, rely on prior mental models, and only correct under logical pressure.  

## Structure  
- `reports/` → JSONL log, human-readable log, SHA256 checksum.  
- `evidence/` → key screenshots (v15 denial, v16 repeat, admission).  
- `external_links.md` → link to full session video (hosted on Google Drive).  
- `scripts/` → checksum generator (PowerShell).  
- `service_brief.md` → short professional brief for researchers/R&D.  
- `CITATION.cff` → citation metadata.  

## Purpose  
This repository complements the Claude and Gemini analyses by documenting **meta-errors in AI reviewers**.  
It establishes that reliability issues extend beyond target models, raising questions about the **integrity of AI evaluation pipelines** themselves.  


## 🔗 External Evidence
Some large artifacts (e.g., video recordings) are hosted outside GitHub due to file size limits.  

👉 See [external-links.md](external-links.md) for:  
- 🎥 Full 471 MB session recording (Google Drive link).  
- 📄 Planned arXiv submission (to be updated).  

This ensures all evidence — logs, screenshots, and video — is transparent and verifiable.

---

**Maintainer**: Priyanshu Kumar (Independent Researcher)  
**Subject & Witness**: ChatGPT-5  
**Acknowledgment**: OpenAI ChatGPT is credited as both subject and co-witness of this incident.  
**ORCID**: [0009-0006-8198-193X](https://orcid.org/0009-0006-8198-193X)  



