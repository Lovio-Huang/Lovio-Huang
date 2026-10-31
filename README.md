## Hi, I'm Yitai

I'm an MS Computer Science student at **Northeastern University** (San Jose, graduating Dec 2028) and I build
backend systems, mostly in Java and Spring Boot. I'm looking for **Summer 2027 software engineering internships**.

### Featured projects

| Project | What it is |
|---|---|
| [**Tally**](https://github.com/Lovio-Huang/tally) | Double-entry ledger API where PostgreSQL itself guarantees the books balance: deferred constraint triggers, append-only history, overdraft CHECKs. Idempotency keys, holds, reversals and reconciliation; 3,000+ transfers/s on a laptop with the books re-verified after every load test. As of Oct 31, 2026: 304 Python tests and 11 JavaScript tests, from raw-SQL attacks to concurrency races and Hypothesis model-based tests, the important ones checked against planted bugs; coverage 98.2% of statements, 94.5% of branches, 97.6% combined. *Python · FastAPI · PostgreSQL · Hypothesis · Docker* |
| [**TicketRush**](https://github.com/Lovio-Huang/ticketrush) | Flash-sale ticketing backend with atomic Redis Lua reservations, idempotent requests and Kafka order processing into MySQL, the source of truth. CI includes a concurrent load test that verifies accepted orders are persisted and Redis/MySQL inventory counts agree; 130 tests. *Java 21 · Spring Boot · Redis · Kafka · MySQL · Testcontainers* |
| [**Sourced**](https://github.com/Lovio-Huang/sourced-rag) | RAG service that answers questions from docs with verifiable citations. Hybrid retrieval (BM25 + embeddings + cross-encoder), measured on a labelled eval set that gates CI. *Python · FastAPI · Claude API · SQLite FTS5 · ONNX* |

### Tools I work with

**Languages:** Java, Python, SQL, C/C++<br/>
**Backend:** Spring Boot, MyBatis, FastAPI, REST APIs<br/>
**Data & messaging:** PostgreSQL, MySQL, Redis, Kafka, SQLite<br/>
**Testing & delivery:** JUnit, Testcontainers, pytest, Hypothesis, Docker, GitHub Actions

### Experience

**Software Engineer Intern, Terra Softech** (Mar – May 2026). Worked on the Spring Boot + MySQL backend of a course and exam platform: hierarchical question categories, REST APIs, and integration testing.

[LinkedIn](https://www.linkedin.com/in/yitai-huang-7bb92642b)
