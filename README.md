# PL-SQL-Collections-Records-and-GOTO-statements
Overview

This repository demonstrates PL/SQL Collections, Records, and GOTO statements through a single, coherent problem: processing and grading student quiz scores with category aggregation, business-rules validation, and exceptional control flow.

The deliverables in the repo:

1. DDL to create schema objects (tables and sample data)

2. PL/SQL package and procedures that use collections, records, and GOTO

3. Test scripts and expected output

---
Problem definition (explicit)

Design a PL/SQL solution for a tutoring center that accepts many quiz submissions per student and:

Aggregates quiz scores by student and by category (e.g., MATH, ENGLISH, SCIENCE).

Calculates per-student final score, weighted by category weights stored in a table.

Detects invalid scores (< 0 or > 100) and uses a GOTO controlled error-handling label to skip the offending record while recording an error row into an errors table.

Uses Records to model each input row and Collections to hold intermediate aggregates and to produce a final sorted student report.

Exposes a packaged API to: load data, process/aggregate, produce a report table, and cleanup.
