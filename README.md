# Hasnat Ahmed

**Software Engineer · FinTech & BI Systems · Lahore, Pakistan**

I build the reporting, data pipelines and backend services behind payment systems: SQL that stays fast on large financial datasets, ETL and batch jobs for time-sensitive data, and Java and Python services around them.

- Software Engineer at **i2c Inc.**, working on fintech reporting and analytics, ETL and batch scheduling, and Java Spring Boot services.
- Analytics engineering on the side: real-time data pipelines in Python and MongoDB.
- BS Computer Science, University of Engineering and Technology (UET), Lahore.

## Featured projects

### [PayFlow Lab](https://github.com/hasnaat93/payflow-lab)

A simulated card payment operations platform: authorization, capture and refunds, fee assessment, a double-entry ledger, settlement batching, reconciliation and SQL reporting.

- **Backend:** Java 21, Spring Boot, PostgreSQL, Flyway. A payment state machine, idempotent money-moving requests, integer-only money arithmetic.
- **Database:** an append-only ledger whose balance is enforced by PostgreSQL triggers and constraints; settlement that cannot pay a transaction twice, even under concurrent runs.
- **Reporting:** reports written as plain SQL with CTEs and window functions over reporting views, exportable to CSV.
- **Frontend:** React and TypeScript operations dashboard.
- **Tests:** unit and integration tests running against a real PostgreSQL.

It is an educational simulator with synthetic data only. It is not a payment gateway.

### [PayFlow Warehouse](https://github.com/hasnaat93/payflow-warehouse) · [live dashboard](https://hasnaat93.github.io/payflow-warehouse/)

A daily batch ELT pipeline that loads payment data into a dimensional warehouse and serves BI-ready marts.

- **Modeling:** star schema with an accumulating snapshot fact and a type 2 slowly changing merchant dimension.
- **Pipeline:** raw, staging, warehouse and mart layers in plain SQL, orchestrated in Python as a task graph. Loads are idempotent and handle duplicates, late-arriving records and replays.
- **Data quality:** bad rows are quarantined with a reason code, every delivered row is accounted for, and 22 checks gate each load. A failed check rolls the whole day back.
- **BI:** mart views with CTEs and window functions, exported to Parquet and CSV, plus a static dashboard published by CI.

Built on synthetic data from a seeded simulator.

## What I work with

| | |
|---|---|
| **Backend** | Java, Spring Boot, REST APIs, Python, C#, .NET |
| **Databases** | PostgreSQL, MySQL, Greenplum, Informix, MongoDB |
| **Data engineering** | SQL optimization, ETL/ELT, data warehousing, data modeling, batch scheduling |
| **BI & analytics** | Power BI, Tableau, Metabase, enterprise reporting |
| **Tools** | Git, Docker, AWS |

## Contact

[LinkedIn](https://linkedin.com/in/hasnaat93) · hasnaat93@gmail.com
