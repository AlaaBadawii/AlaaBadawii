# Hi, I'm Alaa Badawii 👋

**Backend Software Engineer building production-oriented backend and AI systems.**

I build backend systems in Python with a focus on API design, relational data modeling, authentication, correctness, and maintainable architecture. I'm extending that foundation into AI agents and AI-powered systems.

📍 Cairo, Egypt · Open to backend engineering and AI-systems roles

---

## What I'm building now

- **Quizey V2** — re-architecting an exam platform into a production-oriented backend. The core loop is built around versioned exams, auto-grading, JWT authentication, DB-backed RBAC, and a 254-test suite. Phase 2 focuses on attempt lifecycle, timing, idempotent submission, and audit integrity.

- **Evaluator Core** — an AI grading engine using a two-stage Judge + Critic approach. Deterministic scoring is recomputed in code, while AI steps are tested with fake LLMs before real API calls. Currently in progress.

- **DevOps** — building practical CI/CD and containerization experience with Docker, Docker Compose, Jenkins, and GitHub Actions. Kubernetes is the next step in this path.

---

## Featured Work

### Quizey V2 — AI-Assisted Assessment Platform

[`Quizey-V2`](https://github.com/AlaaBadawii/Quizey-V2) · *In progress*

My primary backend engineering project, focused on building an assessment platform with production-oriented design and correctness guarantees.

- **Copy-on-write exam versioning** — editing a published exam creates an immutable version, keeping in-flight attempts consistent and gradable.
- **Attempt lifecycle as a state machine** — `in_progress → paused → submitted → graded → archived`, with transitions guarded at the ORM layer.
- **Idempotent submission under concurrency** — 10 parallel `/submit` calls produce exactly one graded attempt in a test-verified concurrency scenario.
- **Database as the source of truth for roles** — authorization is not dependent on JWT role claims.
- **JWT access + refresh authentication** with DB-backed refresh-token invalidation.
- **Atomic transactions** for operations that must succeed or fail as a unit.
- **Immutable audit logging** at both ORM and database-trigger levels.
- **SQLAlchemy + Alembic** for persistence and schema migrations.
- **254 passing tests** covering the implemented behavior.

### AI Agents

[`AI-Agents`](https://github.com/AlaaBadawii/AI-Agents)

Framework-free implementations built to understand the mechanics behind agentic systems rather than hiding them behind an abstraction layer.

- Agent execution loop
- Tool-calling protocol
- Tool registry
- Memory
- Multi-agent orchestration
- Routing

### Evaluator Core — AI Grading Engine

[`AI-Agents`](https://github.com/AlaaBadawii/AI-Agents) · [`evaluator_core/`](https://github.com/AlaaBadawii/AI-Agents/tree/main/evaluator_core)

An in-progress AI evaluation system designed around a two-stage **Judge + Critic** workflow.

- Fixed rubric-based evaluation
- Deterministic scoring recomputed in Python
- Low-confidence results can be flagged for human review
- Fake-LLM testing to keep tests deterministic and avoid unnecessary API calls
- Designed as the foundation for Quizey's future AI-assisted assessment capabilities

### Docker & CI/CD

[`devops-lab`](https://github.com/AlaaBadawii/devops-lab) · [`jenkins-practice`](https://github.com/AlaaBadawii/jenkins-practice)

Hands-on work around taking backend applications from local development toward reproducible builds and automated testing.

- Docker Compose with Flask + MySQL
- Named volumes and environment-driven configuration
- Tests running inside Docker-based CI
- Jenkins
- GitHub Actions
- Debugging real CI/environment issues rather than only following tutorials

### Quizey V1 — Legacy Assessment API

[`Quizey`](https://github.com/AlaaBadawii/Quizey)

The predecessor to Quizey V2 and an earlier example of my backend work.

- Versioned REST API (`/api/v1`)
- JWT authentication
- Email verification
- PostgreSQL + Alembic
- Automatic grading

---

## Tech Stack

**Backend**  
Python · Flask · FastAPI · SQLAlchemy · REST APIs

**Databases**  
PostgreSQL · MySQL · MongoDB · Redis

**AI**  
LLM Applications · Tool Calling · Agentic Systems · Multi-Agent Orchestration · RAG

**DevOps & Infrastructure**  
Docker · Docker Compose · GitHub Actions · Jenkins · Linux · Bash

**Testing & Tools**  
pytest · unittest · Postman · Git · Concurrency Testing

---

## How I Work

- **Model lifecycle explicitly.** When a domain has meaningful states, I encode those states as a state machine so invalid transitions are prevented rather than handled accidentally.

- **Design and prove correctness.** Idempotent submissions are tested under concurrent requests before being trusted, rather than assuming the implementation is safe.

- **Don't trust an LLM with deterministic work.** AI can evaluate or reason, but deterministic calculations are recomputed and verified in code.

- **Learn mechanics before frameworks.** I build foundational AI concepts without frameworks when possible, then introduce abstractions once I understand what they are solving.

- **Prefer reproducible engineering.** Containers, automated tests, migrations, and CI are part of the development process—not an afterthought.

---

## Links

- GitHub: [AlaaBadawii](https://github.com/AlaaBadawii)
- Portfolio: [AlaaBadawii.github.io](https://github.com/AlaaBadawii/AlaaBadawii.github.io)
- Resume: [Resume](https://drive.google.com/drive/folders/1svf-60hjMWKHKH9x_0TeOQ2A6fy18WGZ71)
- Email: [alaabadawii404@gmail.com](mailto:alaabadawii404@gmail.com)
- LinkedIn: [alaabadawii](https://www.linkedin.com/in/alaabadawii/)
