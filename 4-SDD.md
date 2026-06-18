# Software Design Document (SDD)
## Flight Reservation System

---

## 1. Introduction

This document describes the software design for the Flight Reservation System, including system architecture, data models, entity relationships, and user interface designs. All diagrams are located in the `diagrams/` folder.

---

## 2. Context Diagram

The context diagram shows the system boundary and all external entities that interact with the Flight Reservation System.

**Diagram:** [`diagrams/01-Context-Diagram.png`](diagrams/01-Context-Diagram.png)

External entities interacting with the system:
- **User / Traveler** — searches flights, makes bookings, manages reservations
- **Admin / Airline Staff** — manages flights, pricing, and customer support
- **Payment Gateway** — processes credit/debit card and mobile wallet transactions
- **Email / SMS Service** — delivers booking confirmations and e-tickets
- **Flight Data Provider** — supplies real-time flight status and schedule updates

---

## 3. Logical Data Model

The logical data model defines the abstract entities and their relationships without regard to specific database implementation.

**Diagram:** [`diagrams/02-Logical-Data-Model.jpeg`](diagrams/02-Logical-Data-Model.jpeg)

Core entities:
- **User** — Id, Name, Email, Password, Phone, ProfilePicture
- **Flight** — Id, FlightNumber, Origin, Destination, DepartureTime, ArrivalTime, SeatCapacity, Price, Type
- **Booking** — Id, UserId (FK), FlightId (FK), BookingType, Status, TotalPrice, CreatedAt
- **Payment** — Id, BookingId (FK), Method, Amount, Status, TransactionId
- **Passenger** — Id, FullName, Email, ContactNumber, BookingId (FK)
- **Notification** — Id, UserId (FK), Message, Type, SentAt
- **FlightTracking** — Id, FlightId (FK), Status, GateNumber, DelayMinutes, UpdatedAt

---

## 4. Physical Data Model

The physical data model maps the logical model to actual database tables, column types, and indexes.

**Diagram:** [`diagrams/03-Physical-Data-Model.png`](diagrams/03-Physical-Data-Model.png)

Key implementation details:
- Primary keys are auto-incremented integers
- Passwords stored as bcrypt hashes
- `Price` columns use `DECIMAL(18,2)` for precision
- Foreign key constraints with CASCADE on delete for booking-related tables
- Indexes on `Email`, `FlightNumber`, `DepartureTime` for search performance

---

## 5. ER Diagram

The Entity-Relationship diagram shows all entities and their cardinality relationships.

**Diagram:** [`diagrams/04-ER-Diagram.png`](diagrams/04-ER-Diagram.png)

Key relationships:
- **User** books many **Flights** (via Booking — many-to-many)
- **Booking** has one **Payment**
- **Flight** has many **Passengers** (through Booking)
- **User** receives many **Notifications**
- **Flight** has one **FlightTracking** record

---

## 6. User Interface Designs

The following UI mockups were designed for the system. Each screen is linked below:

| # | Screen | Diagram |
|---|---|---|
| 1 | UI Screen 1 | [`diagrams/05-UI-01.png`](diagrams/05-UI-01.png) |
| 2 | UI Screen 2 | [`diagrams/06-UI-02.png`](diagrams/06-UI-02.png) |
| 3 | UI Screen 3 | [`diagrams/07-UI-03.png`](diagrams/07-UI-03.png) |
| 4 | UI Screen 4 | [`diagrams/08-UI-04.png`](diagrams/08-UI-04.png) |
| 5 | UI Screen 5 | [`diagrams/09-UI-05.png`](diagrams/09-UI-05.png) |
| 6 | UI Screen 6 | [`diagrams/10-UI-06.png`](diagrams/10-UI-06.png) |
| 7 | UI Screen 7 | [`diagrams/11-UI-07.png`](diagrams/11-UI-07.png) |

The UI covers: Welcome, Login/Signup, Home, Booking, Payment, Confirmation, Flight Tracking, Profile, and History screens.

---

## 7. Architecture Overview

```
┌─────────────────────────────────────────────────┐
│                   Client Layer                   │
│         Flutter (Mobile) / React (Web)           │
└───────────────────────┬─────────────────────────┘
                        │ REST API (HTTPS)
┌───────────────────────▼─────────────────────────┐
│                  API Gateway                     │
│              Node.js / Express.js                │
├─────────────┬──────────────┬────────────────────┤
│   Auth      │  Booking     │   Flight Mgmt      │
│  Service    │  Service     │   Service          │
├─────────────┴──────────────┴────────────────────┤
│              Database Layer                      │
│         PostgreSQL (relational data)             │
│         Redis (session/cache)                    │
└─────────────────────────────────────────────────┘
         │                         │
  Payment Gateway           Email/SMS Service
  (Stripe / PayPal)         (SendGrid / Twilio)
```

---

## 8. Technology Stack

| Layer | Technology |
|---|---|
| Mobile Frontend | Flutter (Dart) |
| Web Frontend | ReactJS |
| Backend API | Node.js + Express.js |
| Authentication | Firebase Auth / JWT |
| Database | PostgreSQL / MongoDB Atlas |
| Cache | Redis |
| File Storage | AWS S3 / Cloudinary |
| Payment | Stripe / PayPal SDK |
| Notifications | SendGrid (email) / Twilio (SMS) |
| Hosting | AWS / Firebase / Azure |
| CDN | Cloudflare |
