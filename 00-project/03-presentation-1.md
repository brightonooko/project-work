---
project_outline: "[[00-project/01-project-outline]]"
---

<!-- 5xl -->
# Design and Performance Optimization of an EV Charging Network Database with AI Support

The database will manage the main information required by a charging network, including charging stations, charging points, users, electric vehicles, reservations, charging sessions, energy consumption, tariffs, payments, and technical faults. To investigate how a relational database performs when it contains a large amount of charging-network data with AI being used to generate optimization suggestions, which are reviewed and evaluated through practical experiments.

Author: Brighton Onyango Ooko  
Neptun: J2ADF0  
Supervisor: Anett LENART  
Project ID: 2026-LA-01

---

<!-- 2xl -->
## Problem

Electric vehicle charging networks manage connected data about stations, charging points, users, vehicles, reservations, charging sessions, energy measurements, tariffs, payments, and technical events.

As data volume grows, poor database design and inefficient SQL queries can make reporting and operational analysis slower.

This project will use **Microsoft SQL Server** to build a normalized relational database and investigate how SQL query design and indexing affect performance.

It will also evaluate whether AI-generated optimization suggestions are correct and measurably useful.

---

<!-- 2xl -->
## Target users

- **Charging-network operators** — monitor stations, charging-point availability, sessions, and technical events.
- **Operations and business analysts** — analyse energy consumption, demand, tariffs, and revenue.
- **Database administrators and developers** — maintain data integrity and improve query performance.
- **Researchers and students** — study relational database design, SQL optimization, and AI-assisted development.

---

<!-- 2xl -->
## Planned scope: Database design

- Design at least **10 related tables**.
- Normalize the schema to at least **Third Normal Form (3NF)**.
- Model stations, charging points, users, vehicles, reservations, sessions, energy measurements, tariffs, payments, and technical events.
- Define primary keys, foreign keys, uniqueness rules, and business constraints.
- Use **Microsoft SQL Server and T-SQL**.

---

<!-- 2xl -->
## Planned scope: Data and queries

- Generate reproducible synthetic data containing at least **100,000 charging sessions**.
- Generate at least **1,000,000 timestamped measurement or status records**.
- Implement at least **10 analytical SQL queries**.
- Use joins, aggregation, time-interval filtering, subqueries or CTEs, and window functions.
- Implement at least one T-SQL stored procedure or function.
- Add a trigger only if it is justified by a database requirement.

---

<!-- 2xl -->
## Planned scope: Performance and AI

- Record baseline execution plans, execution times, and logical reads.
- Use SQL Server tools such as Actual Execution Plan, `SET STATISTICS IO`, and `SET STATISTICS TIME`.
- Compare indexing strategies and query rewrites using repeatable tests.
- Evaluate AI optimization suggestions for at least **three queries**.
- Manually check each suggestion for correctness, SQL Server compatibility, and measured performance.
- Review privacy and security risks before sharing schema or query information with an external AI service.

A complete charging application, complex user interface, and custom-trained AI model are outside the required scope. AI-generated SQL will never be executed automatically without review.

---

<!-- 2xl -->
## Functional requirements — Database and Queries

**1. Manage charging-network data**: Store stations, charging points, users, vehicles, reservations, sessions, measurements, tariffs, payments, and technical events.

**2. Maintain database integrity**: Implement at least **10 related tables**, targeting **3NF**. Define appropriate primary keys, foreign keys, relationships, and business constraints.

**3. Generate test data**: Use a reproducible generator to create at least **100,000 charging sessions** and **1,000,000 timestamped measurement or status records**.

**4. Develop complex SQL queries**: Implement at least **10 queries** across the query set using multi-table joins, aggregation, time-interval searches, subqueries or CTEs, and window functions.

**5. Implement business logic**: Implement at least one stored procedure or function using **T-SQL**. Add a trigger only where justified.

---

<!-- 2xl -->
## Functional requirements — Performance and AI

**6. Analyse query performance**: Document baseline execution plans and performance measurements for at least **five queries**.

**7. Optimize queries**: Compare at least **two indexing or query-optimization approaches**, using execution times and execution plans.

**8. Automate measurements**: Build a custom script or application component that records repeatable performance measurements before and after optimization.

**9. Evaluate AI suggestions**: Obtain AI-generated optimization suggestions for at least **three queries**. Check each suggestion for correctness, executability, SQL Server compatibility, and measured performance.

**10. Document AI security**: Document privacy and security risks when sharing information with external AI services. Manually review AI-generated SQL before execution; do not execute suggestions automatically.

---

<!-- 2xl -->
## Initial user journey 1: Analyse charging-network activity

1. An analyst chooses a time period and one or more charging stations.
2. The database retrieves relevant sessions and energy measurements.
3. SQL queries summarize session counts, energy delivered, and station utilization.
4. The analyst compares activity across stations or time periods.

**Expected outcome:** reliable summaries that help explain charging-network activity.

---

<!-- 2xl -->
## Initial user journey 2: Investigate and optimize a slow query

1. A developer runs an analytical query on the baseline dataset.
2. The developer records execution time, logical reads, and the execution plan.
3. The developer tests an appropriate index or query rewrite.
4. The same query is measured again under comparable conditions.
5. The developer compares the results and documents the performance difference.

**Expected outcome:** evidence showing whether the optimization improved query performance.

---

<!-- 2xl -->
## Initial user journey 3: Evaluate an AI optimization suggestion

1. A developer provides a selected query and relevant schema details to an AI service, considering privacy and security.
2. The AI proposes a query rewrite or indexing strategy.
3. The developer reviews the suggestion for correctness and SQL Server compatibility.
4. The suggestion is tested against the same dataset and conditions as the baseline.
5. Its execution plan and measurements are compared with the original query and the developer's own solution.

**Expected outcome:** a measured assessment of the AI suggestion, not an assumption that it is better.

---

<!-- 2xl -->
## Next steps

1. Finalize the requirements, entities, relationships, and business rules.
2. Set up SQL Server and the version-controlled project structure.
3. Design and validate the normalized schema.
4. Build repeatable synthetic-data generation scripts.
5. Implement and validate the analytical queries.
6. Capture baseline execution plans and performance measurements.
7. Test and compare indexes and query rewrites.
8. Evaluate AI suggestions and document results, limitations, and security considerations.
