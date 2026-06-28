# Flight Reservation System — Full System Study

## Overview

This repository contains a complete software engineering documentation suite for the **Flight Reservation System** — a full-stack web/mobile platform for searching, booking, and managing flights. The documentation covers every phase of the software development lifecycle, from initial feasibility analysis through system design.

This is a **full system study** written in proper software engineering form, including:

- Feasibility Study (economic, technical, operational, and scheduling analysis)
- Requirement Gathering (survey + interview methodology with derived requirements)
- Software Requirements Specification (SRS) — industry-standard format
- Software Design Document (SDD) — with context diagram, data models, ER diagram, and UI mockups
- Requirements Traceability Matrix (RTM) — linking every UI component to test cases and pass/fail status

## Repository Structure

```
SRS-for-flight-system/
├── What is Flight Reservation System Documentation.md   ← this file
├── 1-Feasibility-Study.md                               ← economic & technical analysis
├── 2-Requirement-Gathering.md                           ← survey & interview requirements
├── 3-SRS.md                                             ← Software Requirements Specification
├── 4-SDD.md                                             ← Software Design Document
├── 5-Traceability-Matrix.md                             ← Requirements Traceability Matrix
└── diagrams/                                            ← all design diagrams
    ├── 01-Context-Diagram.png
    ├── 02-Logical-Data-Model.jpeg
    ├── 03-Physical-Data-Model.png
    ├── 04-ER-Diagram.png
    ├── 05-UI-01.png  (User Interface mockups)
    ├── 06-UI-02.png
    ├── 07-UI-03.png
    ├── 08-UI-04.png
    ├── 09-UI-05.png
    ├── 10-UI-06.png
    └── 11-UI-07.png
```

## System Summary

The Flight Reservation System provides two portals:

- **End User Portal** — register, search, filter, book (one-way / round-trip / multi-city), pay, receive e-tickets, track flights, manage bookings, and view history
- **Admin Portal** — manage flight schedules, dynamic pricing, customer support, and reporting

### Key Features

| Feature | Priority |
|---|---|
| User Registration & Login | High |
| Flight Search & Filtering | High |
| Booking (one-way, round-trip, multi-city) | High |
| Secure Payment (cards, wallets) | High |
| E-Ticket Generation & Confirmation | High |
| Booking Management (cancel/reschedule) | High |
| Real-time Flight Tracking | Medium |
| Notifications (email/SMS) | High |
| Booking History | Medium |
| Saved Searches & Favorites | Medium |
| Seat & Baggage Selection | Medium |

## Documentation Files

| File | Description |
|---|---|
| `1-Feasibility-Study.md` | ROI analysis, cost estimates, tech stack, scheduling plan |
| `2-Requirement-Gathering.md` | Survey-derived + interview-derived requirements (functional & non-functional) |
| `3-SRS.md` | Full Software Requirements Specification |
| `4-SDD.md` | Software Design Document with references to all diagrams |
| `5-Traceability-Matrix.md` | Complete RTM mapping UI screens → requirements → test cases → pass/fail |
| `diagrams/` | Extracted design diagrams from the SDD |
