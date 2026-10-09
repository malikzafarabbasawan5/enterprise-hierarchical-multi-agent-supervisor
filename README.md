
# Enterprise Hierarchical Multi-Agent Supervisor System

A production-grade, non-linear multi-agent orchestration architecture built on **n8n**. Operates via a central Master Supervisor Agent that dynamically decomposes complex enterprise requests into specialized sub-tasks executed in parallel by dedicated Sub-Agents (Research, Analytics, Synthesis), governed by an automated QA Reviewer Gate and feedback loop.

---

## Architecture Highlights

- **Dynamic Task Decomposition:** Master Supervisor breaks incoming payloads into targeted agent instructions.
- **Parallel Sub-Agent Execution:** Concurrent branch processing across specialized LLM agents.
- **Data Aggregation Engine:** Synchronizes asynchronous sub-agent outputs into unified payloads.
- **Automated QA & Evaluation Gate:** Validates quality standards with automatic retry/loop-back capabilities prior to final response delivery.

---

## System Architecture

<img width="1669" height="933" alt="image" src="https://github.com/user-attachments/assets/ad7f17d9-5992-4c16-b622-3a2fe7ca80d0" />


---

## Technical Stack

- **Orchestrator:** n8n
- **LLM Engine:** Google Gemini (1.5 Flash / Pro)
- **Transformations:** JavaScript (Node.js Engine)
- **Interface:** REST Webhooks / JSON Event Streams
