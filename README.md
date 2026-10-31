## Hi, I'm Yitai

I'm an MS Computer Science student at **Northeastern University** (San Jose, graduating Dec 2028) and I build
backend systems, mostly in Java and Spring Boot. I'm looking for **Summer 2027 software engineering internships**.

### Featured projects

| Project | What it is |
|---|---|
| [**Tally**](https://github.com/Lovio-Huang/tally) | Double-entry ledger API where PostgreSQL itself guarantees the books balance: deferred constraint triggers, append-only history, overdraft CHECKs. Idempotency keys, holds, reversals and reconciliation. Load test (Oct 31, 2026: M5 laptop, Postgres 17 in Docker, 4 API workers, 100 concurrent clients, 5,000 requests per run): 2,160–2,284 completed transfers/s over 4 runs, with the books reconciled after each; payments settled in batches are accepted at 1,944–2,623/s and fully settled at 1,106–1,628/s end to end ([raw results](https://github.com/Lovio-Huang/tally/blob/f9988470d3fd9ccc55c5cd28ede1136b162a9b1f/perf/results/README.md)). As of Oct 31, 2026: 326 Python tests and 11 JavaScript tests, from raw-SQL attacks to concurrency races and Hypothesis model-based tests, the important ones checked against planted bugs; coverage 98.2% of statements, 94.7% of branches, 97.7% combined. *Python · FastAPI · PostgreSQL · Hypothesis · Docker* |
| [**TicketRush**](https://github.com/Lovio-Huang/ticketrush) | Flash-sale ticketing backend with atomic Redis Lua reservations, idempotent requests and Kafka order processing into MySQL, the source of truth. MySQL never sells a ticket twice and every order Kafka acknowledged is persisted; the exceptions are documented. When Redis restarts or comes back with older data, a restart guard stops sales and rebuilds stock from MySQL; Redis commands time out after 2 s and answer `503` instead of hanging; a reused idempotency key with another quantity is refused. CI runs a concurrent load test on every push that fails on a single oversold or lost order. As of Oct 31, 2026: 154 tests, every failure window driven through real Redis, Kafka and MySQL. *Java 21 · Spring Boot · Redis · Kafka · MySQL · Testcontainers* |
| [**Sourced**](https://github.com/Lovio-Huang/sourced-rag) | RAG service that answers questions from Markdown docs and returns, for every cited claim, the exact passage it came from (Claude citations through `search_result` blocks). Hybrid retrieval (BM25 + embeddings + cross-encoder rerank): hit@5 0.98 on 43 labelled questions, with a CI gate that fails below 0.95, and hit@5 1.00 on 24 questions over the Prometheus docs it wasn't written for (not in CI). Two small live Claude runs of 12 questions each: main facts right on all 10 answerable questions, both unanswerable ones declined. As of Oct 31, 2026: 236 offline tests. *Python · FastAPI · Claude API · SQLite FTS5 · ONNX* |

### Tools I work with

**Languages:** Java, Python, SQL, C/C++<br/>
**Backend:** Spring Boot, MyBatis, FastAPI, REST APIs<br/>
**Data & messaging:** PostgreSQL, MySQL, Redis, Kafka, SQLite<br/>
**Testing & delivery:** JUnit, Testcontainers, pytest, Hypothesis, Docker, GitHub Actions

### Experience

**Software Engineer Intern, Terra Softech** (Mar – May 2026). Worked on the Spring Boot + MySQL backend of a course and exam platform: hierarchical question categories, REST APIs, and integration testing.

[LinkedIn](https://www.linkedin.com/in/yitai-huang-7bb92642b)
