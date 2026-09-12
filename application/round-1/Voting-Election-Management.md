---
name: BRIGHTON OOKO
neptun: J2ADF0

---
# Voting Management and Election Web Application

## My interpretation of the brief
The project is a web application that provides a secure and reliable platform for conducting elections, polls, and organizational decision-making. It allows administrators to create and manage elections, voters to securely cast their votes, and auditors to review election activity and verify the integrity of the results.

The platform will support different user roles, including administrators, election officers, voters, and auditors. Key functionality includes voter authentication and eligibility verification, election and candidate management, secure ballot submission, anonymous voting, result management, and audit logging. The goal is to improve election security, transparency, and accessibility while reducing the complexity of managing elections manually.

## Why I am a good fit for this project
I am interested in developing secure and practical software that solves real-world problems. Voting systems provide an opportunity to work with important areas of software engineering such as authentication, authorization, data security, privacy, database design, and system auditing, making this a challenging and valuable final-year project.

## Relevant experience and background
I have experience developing full-stack web applications using frontend and backend technologies, relational databases, authentication, and REST APIs. These skills can be applied to building secure voter management, election administration, ballot handling, result calculation, and audit functionality.

## Proposed approach
I would first define the user roles, election workflow, security requirements, and database structure. Administrators would be able to create elections, manage candidates and eligible voters, configure voting periods, and publish results.

Voters would authenticate and have their eligibility verified before receiving access to an election. They would be able to cast their vote once, while the system would separate voter identity from ballot information where possible to maintain voting privacy.

The backend would use structured REST APIs with PostgreSQL for storing election, voter, and ballot-related data. The frontend would provide responsive dashboards with protected access based on user roles. An audit system would record important election events without exposing the voter's individual choice.

## Initial plan
Define the user roles, election workflow, security requirements, and database schema.
Implement authentication and role-based access control.
Build election, candidate, and voter management.
Implement voter eligibility verification and secure ballot submission.
Add anonymous voting and protection against duplicate voting.
Develop vote counting, turnout statistics, and result management.
Implement an audit log for important election activities.
Test the system with realistic election scenarios for security, accuracy, and usability.

## Additional information
I plan to maintain a Git repository from the start and use structured commits and issue tracking to manage development. The application will focus on security, privacy, data integrity, and ease of use. As additional features, I could include ranked-choice voting, automated election reports, email notifications, cryptographic verification of election results, and real-time election monitoring.