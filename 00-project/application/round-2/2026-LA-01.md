---
name: BRIGHTON OOKO
neptun: J2ADF0
id: 2026-LA-01

---
# Electric Vehicle Charging Network Database and Performance Optimization

## My interpretation of the brief

The project is a relational database for managing an electric vehicle charging network. It will store information about charging stations, charging points, users, vehicles, reservations, charging sessions, energy usage, payments, tariffs, and technical faults.
The main focus is not building a complete application, but designing a well-structured database and improving its performance when handling a large amount of data.

## Why I am a good fit for this project

I am interested in database development and performance optimization. This project provides practical experience with database design, SQL queries, indexing, performance measurement, and query optimization. It also introduces AI as a supporting tool while allowing the performance of AI suggestions to be tested using real measurements.

## Relevant experience and background

I have experience working with relational databases, SQL, backend development, and data management. These skills can be applied to designing the database structure, writing complex queries, generating test data, and analyzing query performance.

## Proposed approach

I would first design the database with at least ten related tables while maintaining proper relationships, constraints, and normalization.
I would then generate a large amount of test data, including at least 100,000 charging sessions and one million measurement or status records. After that, I would create complex SQL queries representing common charging-network operations.
For selected queries, I would measure their execution time and examine their execution plans. I would then apply different indexes and query optimizations and compare the results before and after optimization.
AI could also be used to suggest indexes or query improvements for selected queries. These suggestions would be reviewed and tested rather than applied automatically.

## Initial plan

Design and normalize the database structure.
Implement the database and business constraints.
Create automated test-data generation.
Generate large datasets for testing.
Develop at least ten complex SQL queries.
Analyze query execution plans and performance.
Implement and test different indexing strategies.
Add a stored procedure or function for business logic.
Compare performance before and after optimization.
Test and evaluate AI-generated optimization suggestions.
Document the results and make the process reproducible.

## Additional information

The project will be maintained in a Git repository with setup instructions, database scripts, test-data generation, and performance measurement tools.
The final evaluation will focus on measurable improvements in query performance, changes in execution plans, and whether the proposed optimizations actually work.
Possible future extensions include database partitioning, location-based charging-station searches, materialized views, or a simple monitoring interface.
