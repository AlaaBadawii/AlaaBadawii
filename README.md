# Hi, I'm Alaa Badawii 👋

**Software & AI Systems Engineer | Building Intelligent Products**

I build software and AI-powered applications using Python, combining backend systems, LLM applications, RAG, and agentic workflows.

I care about the whole system: how its components work together, how data and decisions stay reliable, and what checks are needed to make AI-powered features trustworthy and useful.

📍 Cairo, Egypt · Open to Software Engineering, Backend Engineering, and AI Engineering opportunities.

---

## What I'm Working On

- **Quizey V2** — building the backend foundation of an AI-first assessment and training platform. Current work focuses on assessment versioning, attempt lifecycle, authentication, data integrity, and platform services.
- **AI Agents From Scratch** — implementing agent mechanics in Python to understand tool calling, agent execution, memory, routing, and multi-agent orchestration.
- **Evaluator Core** — developing a two-stage Judge + Critic evaluation engine, with deterministic scoring, validation, and human-review escalation.

---

## Selected Work

### Quizey V2 — AI-First Assessment & Training Platform

*In progress · Private repository*
*But, check description: https://github.com/AlaaBadawii/quizey-platform*

My main software engineering project: an assessment and training platform designed around the idea of understanding what learners already know before guiding them toward the right learning path.

The current implementation focuses on building a reliable backend foundation. AI-powered assessment and learning capabilities are part of the product roadmap.

**Engineering highlights**

- **Modular monolith architecture** using Python, Flask, SQLAlchemy, and MySQL.
- **Copy-on-write exam versioning** to preserve published versions and keep existing attempts consistent.
- **Frozen attempt papers** so grading remains tied to the exact assessment presented to the learner.
- **Attempt lifecycle management** with explicit state transitions and guarded operations.
- **Idempotent submission** to protect against duplicate requests.
- **JWT authentication** with Redis-backed token revocation and fail-closed behavior when the revocation store is unavailable.
- **Database-backed authorization** with the database remaining the source of truth for user roles.
- **Audit logging and transactional integrity** for operations that require reliable state changes.
- **Automated testing** covering business rules, security behavior, and system reliability.

**Current test status:** 1,116 passing tests, plus 181 subtests.

---

### Clinical RAG System — Creativa AI Hackathon
[Repository: AI-Agents](https://github.com/AlaaBadawii/grounded-rag-ng217)

*Team Lead · Five-person team · August 2026*

Led a team of five in developing a clinical Retrieval-Augmented Generation (RAG) system based on NICE NG217 guidelines.

My contribution covered system architecture, the FastAPI backend, hybrid retrieval, cross-encoder reranking, LLM generation, and deterministic citation validation.

**Evaluation results**

- Improved Precision@1 from 35% to 85%.
- Achieved 87.9% Mean Reciprocal Rank (MRR).
- Reached 100% recall.
- Achieved 100% grounded responses.
- Produced 130/130 traceable citations.

The project focused on improving retrieval quality and ensuring generated answers remained grounded in their source material.

---

### Abu Prompt — LinkedIn Personal Branding Agent
[Repository: AI-Agents](https://github.com/AlaaBadawii/PersonalBrandingAgent)

A deterministic-first AI agent designed to support consistent, context-aware LinkedIn content creation through a scheduled workflow rather than a conversational chatbot.

The system combines a personal knowledge base, retrieval-augmented generation (RAG), LLM reasoning, and validation to produce content grounded in the user's actual experience and professional background.

**Engineering highlights**

- **Scheduled execution** using a controlled workflow rather than relying on manual chatbot interactions.
- **RAG-powered personal knowledge base** using Chroma to retrieve relevant context.
- **LLM reasoning** to transform retrieved information into relevant LinkedIn content.
- **Content validation** to keep generated outputs grounded and consistent.
- **Persistent state management** using SQLite.
- **Publishing history** to track previous content and prevent unnecessary duplication.
- **Controlled publishing** with execution limits and safeguards.
- **Deterministic-first design** to keep workflow decisions and important checks outside the LLM.

The project explores how retrieval, reasoning, validation, and workflow automation can work together to build a more reliable AI-powered application.

---

### AI Agents From Scratch

[Repository: AI-Agents](https://github.com/AlaaBadawii/AI-Agents)

A collection of framework-free implementations built to understand the mechanics behind agentic systems rather than hide them behind abstractions.

The repository progresses from individual agents to multi-agent orchestration and AI evaluation.

**Implemented projects**

- **Readme Agent** — explores project inspection, tool registration, and schema generation for README creation.
- **Agent Assistant** — a conversational agent built around the OpenAI-style tool-calling protocol.
- **Multi-Agent System** — an orchestrator and specialized agent for generating and validating multiple-choice questions.

**Evaluator Core — In Progress**

A two-stage AI evaluation engine based on a Judge + Critic workflow.

- Fixed rubric-based evaluation.
- Deterministic scoring recomputed in Python.
- Low-confidence or conflicting evaluations can be escalated for human review.
- Fake-LLM testing to keep tests deterministic and avoid unnecessary API calls.

The implemented agents include Dockerfiles and are integrated into the repository's Docker Compose setup.

---

### DevOps & CI/CD Practice

[devops-lab](https://github.com/AlaaBadawii/devops-lab) · [jenkins-practice](https://github.com/AlaaBadawii/jenkins-practice)

Practical work on making backend applications easier to build, test, and run consistently.

- Docker and Docker Compose.
- Flask + MySQL containerized environments.
- Named volumes and environment-driven configuration.
- Automated testing in container-based workflows.
- Jenkins and GitHub Actions.
- Debugging CI and environment configuration issues.

---

## Technical Toolbox

**Software & Backend Engineering**

Python · Flask · FastAPI · SQLAlchemy · REST APIs · API Design · Software Architecture

**Databases & Data**

MySQL · PostgreSQL · SQLite · Redis · Relational Data Modeling

**AI Engineering**

Large Language Models (LLMs) · RAG · Tool Calling · AI Agents · Multi-Agent Systems · LLM Evaluation · Prompt Engineering

**DevOps & Infrastructure**

Docker · Docker Compose · GitHub Actions · Jenkins · Linux · Bash

**Testing & Quality**

pytest · unittest · API Testing · Concurrency Testing · Postman · Alembic

---

## How I Approach Engineering

- **Think about the whole system.** I care about how APIs, data, business logic, infrastructure, and AI capabilities work together to create a complete product.
- **Make correctness testable.** Important business rules and state transitions should be enforced and verified, not left to assumptions.
- **Keep deterministic work deterministic.** When AI is involved in evaluation or reasoning, calculations and critical validations should still be independently verified in code.
- **Build AI with safeguards.** Retrieval quality, evaluation, validation, and human review matter when AI outputs affect users.
- **Understand the mechanics.** I like exploring how things work underneath before relying on frameworks and abstractions.
- **Prefer reproducible engineering.** Automated tests, migrations, containers, and CI help make changes safer and easier to maintain.

---

## Connect With Me

- **GitHub:** [AlaaBadawii](https://github.com/AlaaBadawii)
- **Portfolio:** [alaabadawii.github.io](https://alaabadawii.github.io)
- **Resume:** [View Resume](https://drive.google.com/drive/folders/1svf-60hjMWKHKH9x_0TeOQ2A6fy18WGZ71)
- **Email:** [alaabadawii404@gmail.com](mailto:alaabadawii404@gmail.com)
- **LinkedIn:** [Alaa Badawii](https://www.linkedin.com/in/alaabadawii/)
