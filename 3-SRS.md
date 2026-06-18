# Software Requirements Specification (SRS)
## Flight Reservation System

---

## 1. Introduction

### 1.1 Purpose

The purpose of this project is to design and develop an advanced Flight Reservation System that provides a seamless and efficient experience for both travelers and airline administrators. The system ensures users can easily search, book, and manage flights while enabling airline staff to oversee flight operations, customer support, and revenue-generating promotions.

### 1.2 Project Scope

The system will consist of two main modules:

- **End User Portal**: Allows travelers to register, search for flights, book tickets, track flights, and manage their bookings.
- **Admin Portal**: Supports flight schedule creation, dynamic pricing, customer service management, and reporting.

The system will also integrate payment gateways, notifications (email/SMS), and enforce modern non-functional attributes like security, scalability, and localization.

### 1.3 Intended Audience

- **System Developers**: Frontend developers, backend developers, testers, and database managers responsible for maintaining system performance and reliability.
- **Project Stakeholders**: Product owners, business analysts.
- **QA Engineers**: Responsible for validating requirements against test cases.

---

## 2. Project Scenario

This project aims to provide users with a seamless and efficient platform to book and manage flights online. Users can:

- Register, log in, and search for flights based on destination, date, and class
- Apply filters like price, duration, and airline
- View detailed flight information and choose between one-way, round-trip, or multi-city bookings
- Complete secure payments through various methods
- Receive e-tickets via email or SMS
- Manage reservations, view booking history, and track real-time flight status
- Receive timely notifications and promotional offers

The system ensures high usability, security, performance, and accessibility across devices.

---

## 3. System Features

| # | Feature | Description | Priority |
|---|---|---|---|
| 1 | User Registration & Login | Allows users to create an account, log in securely, and manage their profile. | High |
| 2 | Flight Search | Enables users to search for available flights based on destination, date, and class. | High |
| 3 | Flight Filtering | Lets users refine search results using filters such as price, duration, layovers, and airline ratings. | Medium |
| 4 | View Flight Details | Displays comprehensive information for selected flights, including seat availability and total fare. | High |
| 5 | Booking Options | Provides flexible booking types including one-way, round-trip, and multi-city itineraries. | High |
| 6 | Payment Integration | Supports multiple secure payment methods like credit/debit cards and mobile wallets. | High |
| 7 | E-Tickets & Confirmation | Automatically sends e-tickets and booking confirmations via email and SMS after payment. | High |
| 8 | Booking Management | Allows users to modify, cancel, or reschedule bookings through their dashboard. | High |
| 9 | Booking History | Enables users to view records of previous bookings and flights. | Medium |
| 10 | Flight Tracking | Provides real-time updates on flight status, including delays or gate changes. | Medium |
| 11 | Notifications | Sends alerts and reminders for flight updates, booking changes, and confirmations. | High |

---

## 4. Functional Requirements

### 4.1 End User Requirements

| Feature | Functional Requirement |
|---|---|
| User Registration & Login | The Users shall be able to register, log in, and securely access their account. |
| Flight Search | The Users shall be able to search flights by destination, date, class, etc. |
| Flight Filtering | The Users shall be able to filter results by price, duration, layover, and airline reputation. |
| View Details | The Users shall be able to view flight info including seat availability, layovers, and prices. |
| Booking Options | The Users shall be able to book one-way, round-trip, or multi-city flights. |
| Payment Integration | The System shall support Credit/Debit Cards, Mobile Wallets. |
| E-Tickets | The System shall generate an e-ticket and send confirmation via email/SMS. |
| Booking Management | The Users shall be able to cancel or reschedule bookings via their dashboard. |
| Booking History | The Users shall be able to view past flights. |
| Flight Tracking | The Users shall be able to access real-time flight status and updates. |
| Notifications | The System shall send flight updates and confirmation alerts. |
| Saved Searches & Favorites | The user shall be able to save searches and favorite flights. |
| Flight Alerts | The user shall be able to set customizable flight alerts / price tracking. |
| Seat Selection Options | The user shall be able to select seat, add-on services, and baggage preferences. |
| Flight Planner | The user shall be able to use a travel flight planner or calendar integration. |
| Personalized Filters | The user shall be able to personalize filters based on travel purpose or profile. |

---

## 5. Non-Functional Requirements

| Category | Requirement |
|---|---|
| Usability | The System UI shall be user-friendly and support both mobile and desktop users. |
| Scalability | The System shall scale to support thousands of simultaneous users. |
| Performance | Search, booking, and payment should complete within 3 seconds under normal load. |
| Security | The System shall use SSL, secure authentication, and encrypted payment processing. |
| Availability | The System shall maintain 99.9% uptime. |
| Reliability | System must reliably process payments and confirm bookings without data loss. |
| Maintainability | The System shall support easy updates to flights and pricing without downtime. |
| Localization | The System shall support multi-language for international users. |
| Biometric Authentication | The System shall have a biometric authentication option (fingerprint/face). |
| Offline Access | The System shall provide offline access to booking history and e-tickets. |

---

## 6. User Interfaces

The system provides UI screens for the following flows (see `diagrams/` folder for mockups):

- Welcome / Landing Screen
- Sign Up / Login
- Forgot Password
- Home (destination cards — Riyadh, Doha, Istanbul, Dubai, Cairo, Japan, Kuwait, Paris)
- Booking Screen (adults, children, price slider, class dropdown)
- Payment (Visa, Mastercard, Bank Transfer)
- Confirmation
- Flight Tracking
- Confirmation Sent
- Rate Us / Feedback
- Profile / Account
- Flight History

---

## 7. Constraints

- The system must comply with international aviation data standards.
- Payment processing must comply with PCI-DSS standards.
- User data must be handled in compliance with GDPR (for international users).
- The system must be accessible on both iOS/Android (Flutter) and web browsers.
