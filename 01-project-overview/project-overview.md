# Ustaad.af - Digital Marketplace for Skilled Workers

## Description

A marketplace connecting customers in Afghanistan with Ustaads such as plumbers, electricians, carpenters, painters, cleaners, AC repair workers and construction workers. These examples describe the domain; actual selectable trades depend on database categories.

## Problem

Customers need a structured way to find skilled help, compare workers and coordinate requests. Workers need visibility and a way to apply for relevant jobs.

## Objective

Verify and refine an existing marketplace through four documented academic Scrum sprints, maintaining truthful requirements and event evidence.

## Target users

Visitors, customers, workers/Ustaads and administrators.

## Scope

The inspected code implements public discovery, authentication, profiles, job posting/editing/cancellation, applications/hiring, messages, completion/reviews, reporting/blocking and admin moderation. Contact enquiries also exist. Assignment verification and documentation are PLANNED; no sprint completion is asserted.

## Expected outcome

A verified integrated workflow, traceable requirements, UML models, four sprint records and genuine meeting recordings/minutes, ready for academic submission. These are expected deliverables, not completed outcomes.

## Technology stack

- Laravel **12.69.2** and Inertia Laravel adapter **2.0.26**
- Vue **3** (`^3.5.13`), Inertia Vue **2** (`^2.0.0-beta.3` declared range), TypeScript and Vite **6** (`^6.0.3`).
- SQLite is the default in MySQL is supported by configuration; production database choice is unverified.
- Eloquent models/policies, Form Requests, controllers and Action classes implement workflows. Pest 3 tests exist; their current results are not claimed here.
