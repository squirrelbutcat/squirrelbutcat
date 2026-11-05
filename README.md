### Polina Severyukhina · BI & Data Analytics

3rd-year student at NUST MISIS (Computer Science, *Intelligent Data Analysis in the Digital Economy*). I work with SQL and Python and build data pipelines, from raw data to warehouse layers, data marts and dashboards. Open to BI / Data Analytics internships.

📫 polsersev29@gmail.com · Telegram [@parapolli](https://t.me/parapolli)

## Tech stack

| Area | Tools |
|---|---|
| SQL & databases | Trino SQL, T-SQL (MS SQL Server), Spark SQL, SQLite; basic PostgreSQL |
| Data platforms | Apache Iceberg, Trino, Apache Spark, MinIO (S3), Parquet, Docker |
| Data analysis | Python, Pandas, NumPy, Jupyter, Seaborn, Matplotlib, Plotly |
| BI | Yandex DataLens, Excel (basic, coursework level) |
| Development | Git, GitHub, TypeScript, React, Next.js |

## Selected projects

### [Lakehouse: medallion architecture for TPC-H Q16](https://github.com/squirrelbutcat/misis-2026-inf-theory)
`MinIO (S3)` `Apache Iceberg` `Lakekeeper` `Trino` `Spark` `Docker`
- Bronze → Silver → Gold pipeline on **5M rows** (TPC-H sf5), reproducible from shell scripts and step-by-step SQL
- Silver layer **6× smaller** than raw data (22.5 MB vs 139.2 MB); partitioning cuts the query scan to **~16%** of data
- Gold mart validated against the reference query with `EXCEPT` both ways: 27,724 rows, **0 mismatches**
- Benchmarked compression codecs (ZSTD 11% faster reads, GZIP 9% smaller) and engines (Trino 0.8 s vs Spark 7.0 s); demonstrated schema evolution and time travel recovery

### [Bakery database](https://github.com/squirrelbutcat/sql-misis)
`MS SQL Server` `T-SQL`
- 3NF model with **16 tables**, 7 views, 10 functions, 15 stored procedures, 12 triggers, 10 indexes
- Sales reporting with window functions (`RANK`, revenue share via `SUM OVER`, running totals), cost and margin per product
- Stock calculated from source documents; business rules enforced by triggers (no overselling, immutable posted documents, auto-reorder from the cheapest supplier)

### [Students, social media and mental health: EDA](https://github.com/squirrelbutcat/Analysis-student)
`Python` `Pandas` `NumPy` `Seaborn` `Plotly` `SQLite`
- Pipeline: Kaggle API → cleaning (5,000 rows × 13 features) → SQLite → 8 SQL queries (CTE, `CASE`, `HAVING`) → interactive Plotly dashboard
- Strong negative correlation between social media time and sleep (r = −0.81), reported as correlation, not causation

### [Network Explorer](https://github.com/Homosanians/NetworkExplorer) (team project)
`Next.js` `React` `TypeScript`
- My part: frontend (AS search, interactive relationship graph, admin panel) and the Dinic max-flow algorithm with unit tests, on CAIDA and PeeringDB data

## Currently learning
SQL query design · BI and data visualization · data warehousing and data processing
