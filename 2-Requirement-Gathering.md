# Requirement Gathering — Flight Reservation System

## Gathering Methods

Requirements were collected via two methods: **Google Form Survey** and a structured **Interview**.

---

## 1. Survey — Derived Requirements

| # | Derived Requirement |
|---|---|
| 1 | The System shall scale to support thousands of simultaneous users. |
| 2 | The System shall contain different flight categories for different purposes of air travel. |
| 3 | The System UI shall be user-friendly and support both mobile and desktop users. |
| 4 | The System shall be available on different platforms. |
| 5 | The System shall maintain 99.9% uptime. |
| 6 | The Users shall be able to book one-way, round-trip, or multi-city flights. |
| 7 | The Users shall be able to filter results by price and flying class. |
| 8 | The Users shall be able to filter results by price, duration, layover, and airline reputation. |
| 9 | The System shall support Credit/Debit Cards and Mobile Wallets. |
| 10 | The Users shall be able to view flight info including seat availability and prices. |
| 11 | The Users shall be able to cancel or reschedule bookings via their dashboard. |
| 12 | The Users shall be able to access real-time flight status and tracking updates. |
| 13 | The System shall generate an e-ticket and send confirmation via email/SMS. |

---

## 2. Interview — Functional Requirements (5 Questions)

### Q1: Saved Searches & Favorites
**Question:** "Would you like the ability to save your frequent destinations or favorite flights for quicker future bookings?"

**Answer:** "Yes, I'd love that. I often book flights to the same cities, so saving them would save time."

**Derived Requirement:** The user shall be able to save searches and favorite flights.

---

### Q2: Flight Alerts
**Question:** "If you travel often, would it be helpful to set up flight alerts for certain routes or price drops?"

**Answer:** "Absolutely. Getting notified when prices drop for my usual routes would be very helpful."

**Derived Requirement:** The user shall be able to set customizable flight alerts / price tracking.

---

### Q3: Seat & Baggage Selection
**Question:** "Would you prefer the option to choose your seat, baggage options, or meal preferences during booking?"

**Answer:** "Yes, I want to choose my seat and add extra baggage if needed while booking, not after."

**Derived Requirement:** The user shall be able to select add-on services, choose seat, and set baggage preferences during booking.

---

### Q4: Travel Calendar / Itinerary Planner
**Question:** "How would you feel about having a built-in travel calendar or itinerary planner that syncs your bookings?"

**Answer:** "That sounds great! It would help me keep track of flights and manage my travel plans better."

**Derived Requirement:** The user shall be able to use a travel flight planner or calendar integration.

---

### Q5: Personalized Filters
**Question:** "Do you often travel for work or leisure, and would you want the system to offer suggestions based on your purpose?"

**Answer:** "I mostly travel for business. I'd like filters or suggestions that match work travel — quick flights, Wi-Fi on board."

**Derived Requirement:** The user shall be able to personalize filters based on travel purpose or profile.

---

## 3. Interview — Non-Functional Requirements (3 Questions)

### Q1: Biometric Authentication
**Question:** "How would you feel about using biometric login (fingerprint or face recognition) instead of a password?"

**Answer:** "I'd prefer it. It's quicker and feels more secure than typing passwords every time."

**Derived Requirement:** The System shall provide a biometric authentication option.

---

### Q2: Performance Under Load
**Question:** "Have you ever been frustrated by a slow or overloaded booking site? What would you expect in terms of reliability?"

**Answer:** "Yes, especially during holidays. I expect the system to stay fast and not crash even when many people are using it."

**Derived Requirement:** The system shall maintain high performance and responsiveness under peak traffic conditions.

---

### Q3: Offline Access
**Question:** "Would you be interested in using the system offline — such as to view booking history or your e-ticket?"

**Answer:** "Yes, having offline access to my ticket and trip details at the airport would be very helpful."

**Derived Requirement:** The system shall provide offline access to essential features such as viewing booking history and e-tickets.

---

## 4. Functional Requirements Summary

| Feature | Functional Requirement |
|---|---|
| User Registration & Login | Users shall be able to register, log in, and securely access their account. |
| Flight Search | Users shall be able to search flights by destination, date, class, etc. |
| Flight Filtering | Users shall be able to filter results by price, duration, layover, and airline reputation. |
| View Details | Users shall be able to view flight info including seat availability, layovers, and prices. |
| Booking Options | Users shall be able to book one-way, round-trip, or multi-city flights. |
| Payment Integration | The System shall support Credit/Debit Cards and Mobile Wallets. |
| E-Tickets | The System shall generate an e-ticket and send confirmation via email/SMS. |
| Booking Management | Users shall be able to cancel or reschedule bookings via their dashboard. |
| Booking History | Users shall be able to view past flights. |
| Flight Tracking | Users shall be able to access real-time flight status and updates. |
| Notifications | The System shall send flight updates and confirmation alerts. |
| Saved Searches & Favorites | Users shall be able to save searches and favorite flights. |
| Flight Alerts | Users shall be able to set customizable flight alerts. |
| Seat Selection Options | Users shall be able to select seat, baggage, and add-on services. |
| Flight Planner | Users shall be able to use a travel planner or calendar integration. |
| Personalized Filters | Users shall be able to personalize filters based on travel purpose or profile. |

---

## 5. Non-Functional Requirements Summary

| Category | Requirement |
|---|---|
| Usability | The System UI shall be user-friendly and support both mobile and desktop users. |
| Scalability | The System shall scale to support thousands of simultaneous users. |
| Performance | Search, booking, and payment should complete within acceptable response times. |
| Security | The System shall use SSL, secure authentication, and encrypted payment processing. |
| Availability | The System shall maintain 99.9% uptime. |
| Reliability | The System must reliably process payments and confirm bookings without data loss. |
| Maintainability | The System shall support easy updates to flights and pricing. |
| Localization | The System shall support multi-language for international users. |
| Biometric Authentication | The System shall provide a biometric authentication option. |
| Offline Access | The System shall provide offline access to booking history and e-tickets. |
