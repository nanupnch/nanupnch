# Nanu Panchamurthy

**Backend software engineer · Los Angeles**

I build backend systems with attention to what happens when requests repeat, updates arrive out of order, or work stops halfway through. I care about keeping state correct, making failures understandable, and giving the next engineer a clear path to recovery.

[LinkedIn](https://www.linkedin.com/in/nanupnch/) · [Email](mailto:nanupnch@gmail.com)

## Selected work

### [LedgerOps](https://github.com/nanupnch/ledgerops)

**Transaction correctness and reliability lab · Go + PostgreSQL**

A double-entry ledger built to test what its correctness guarantees actually cover.

- Saves transfers, ledger entries, balance changes, and successful retry results in one transaction.
- Injects eight faults to distinguish failures that database constraints prevent from corruption that audits detect.
- Tests concurrent retries and opposing transfers, and measures completed work separately from replays and lock conflicts.

Recorded lab benchmarks reached **779 committed transfers/s with uniform traffic** and **175/s with hotspot traffic**. Each run used 32 workers, 1,000 accounts, and a 30-second measurement window; integrity audits were clean before and after both runs.

[Design, fault results, and benchmark details](https://github.com/nanupnch/ledgerops#readme) · [Concurrency and fault tests](https://github.com/nanupnch/ledgerops/blob/main/internal/store/store_test.go)

### [vnf-stroll](https://github.com/nanupnch/vnf-stroll)

**Network optimization experiments · Python**

Exact solvers for placing and migrating virtual network function chains in fat-tree data centers, based on an IPDPS 2022 paper. The project cross-checks solvers, recomputes costs with an independent checker, and records assumptions and reproducible experiments.

[Experiments and findings](https://github.com/nanupnch/vnf-stroll/tree/main/results) · [Independent checker](https://github.com/nanupnch/vnf-stroll/blob/main/vnfstroll/checker.py)

## Professional background

- **Humana · Senior Software Engineer:** Healthcare integrations, including submission identity, partner-message delivery, status reconciliation, and tracing.
- **VMware · Software Engineer → Software Engineer II:** AWS environment provisioning and cleanup, durable background workflows, Kafka delivery, and incident recovery.

MS in Computer Science, California State University, Dominguez Hills.

**Tools I use:** Java / Spring Boot, Go, Python, SQL, PostgreSQL, MySQL, Kafka, AWS, and Docker.

I also write practical frameworks. [Building Software with AI: Check, Context, Consequence](https://github.com/nanupnch/my_frameworks/blob/main/3c_framework.md) asks how a result can be verified, what information the task needs, and what happens if the result is wrong.
