---
name: "Brighton Onyango Ooko"
neptun: "J2ADF0"
id: 2026-LA-01
github: "https://github.com/brightonooko/project-work"
---

# Electric Vehicle Charging Network Database with AI-Supported Performance Optimization

This project designs and implements a relational database for an electric vehicle (EV) charging network. The database manages interconnected information about charging stations, charging points, users, vehicles, reservations, charging sessions, energy consumption, tariffs, payments, and technical faults. The project focuses on database design, SQL query performance, indexing strategies, and measurement-based optimization. Artificial intelligence (AI) is used to generate optimization suggestions, which are reviewed and evaluated through practical experiments.

The database will be populated with reproducibly generated test data to simulate a realistic charging network. Complex SQL queries will be developed to answer operational and business questions, such as identifying the most frequently used charging stations, analysing energy consumption, calculating revenue, and detecting charging points with frequent technical faults. By the end of the project, the database will support these operations, and its performance will be evaluated before and after optimization using execution plans and measured results.

## Objectives

- **Primary objective:** Design, implement, and optimize a relational database for an electric vehicle charging network, using practical performance measurements to evaluate different SQL optimization and indexing techniques.
- **Target users / stakeholders:** Charging network operators, database administrators, EV charging service providers, and analysts interested in charging activity, energy consumption, revenue, and system reliability.
- **Measurable success criteria:** Implement at least 10 related tables designed to at least Third Normal Form (3NF), generate at least 100,000 charging sessions and 1,000,000 timestamped measurement or status records, develop at least 10 complex SQL queries, and conduct detailed performance analysis on at least five queries. Evaluate AI-generated optimization suggestions for at least three selected queries.
- **Constraints:** Oracle Database with SQL and PL/SQL, or Microsoft SQL Server with SQL and T-SQL; version-controlled development; reproducible test-data generation and performance measurements; database-specific execution-plan analysis; and no automatic execution of AI-generated SQL or database commands without review.

## Scope

### In scope

- Designing and implementing a normalized relational database for an EV charging network.
- Managing charging stations, charging points, users, vehicles, reservations, charging sessions, energy measurements, tariffs, payments, and technical events.
- Enforcing primary keys, foreign keys, uniqueness, validation rules, referential integrity, and important business constraints.
- Generating reproducible synthetic test data, including at least 100,000 charging sessions and 1,000,000 timestamped measurement or status records.
- Developing at least 10 complex SQL queries involving multi-table joins, aggregations, time-interval searches, subqueries or common table expressions (CTEs), and window functions.
- Implementing at least one stored procedure or function for business logic, and a trigger where justified.
- Analysing execution plans and measuring query performance before optimization.
- Testing simple and composite indexes, query rewrites, and relevant database-specific indexing techniques.
- Comparing the performance of at least five queries before and after optimization.
- Using an automated script or application component to execute queries and record reproducible performance measurements.
- Obtaining AI-generated optimization or indexing suggestions for at least three queries and evaluating their correctness, executability, and measured performance.
- Documenting the experimental process, optimization results, limitations, and security considerations when using an external AI service.

### Out of scope

- Developing a complete EV charging management application.
- Building a web interface or mobile application.
- Integrating with real charging stations, payment gateways, or live electricity providers.
- Using real customer or payment information in the test dataset or sending sensitive data to an external AI service.
- Developing a custom AI model.
- Automatically executing AI-generated SQL, PL/SQL, T-SQL, or database definition statements without review.
- Implementing optional extensions such as spatial station searches, database partitioning, materialized views, or an operator dashboard as mandatory features.

## Notes

The initial implementation will focus on a well-structured relational database, synthetic test data, and a selected set of representative business queries. Performance experiments will establish baseline execution times and plans before applying indexing and query optimization techniques. The same queries and measurement procedures will then be used to compare results after optimization.

AI-generated suggestions will be treated as proposals rather than guaranteed improvements. Each suggestion will be reviewed, checked for correctness, and tested against the student's own solution. The final conclusions will be based on measured results rather than assumptions about which approach should be faster.

The project will use Git for version control and document the database schema, test-data generation, SQL scripts, performance measurements, and experimental findings to make the development and evaluation process reproducible.
