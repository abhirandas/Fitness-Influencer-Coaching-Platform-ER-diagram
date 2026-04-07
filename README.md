# 🏋️ Online Fitness Coaching Platform – ER Diagram

## 📌 Overview

This project represents the database design for an **online fitness coaching platform** where trainers manage clients, offer structured coaching programs, conduct sessions, and track client progress over time.

The system supports both **long-term coaching subscriptions** and **session-based interactions**, along with detailed progress tracking through regular check-ins.

---

## 🧠 Key Features Modeled

* 👤 User management with role-based profiles (Trainer / Client)
* 📦 Coaching plans created by trainers
* 🔁 Subscription system for long-term coaching
* 📅 Session scheduling (consultations & coaching sessions)
* 📊 Weekly check-ins and progress tracking
* 💬 Trainer feedback system
* 💳 Payment tracking for subscriptions

---

## 🧱 Entity Breakdown

### 👤 USER

Base entity representing all users in the system.

* Stores common details like name, email, phone, and role.

### 🧑‍🏫 TRAINER_PROFILE

Contains trainer-specific information such as:

* Bio, experience, and specialization

### 🧑 CLIENT_PROFILE

Stores client-specific data:

* Physical attributes (height, weight)
* Fitness goals and health conditions

---

### 📦 PLAN

Represents coaching programs created by trainers.

* Includes pricing, duration, and type of plan

### 🔁 SUBSCRIPTION

Tracks which client has subscribed to which plan.

* Stores lifecycle details like start date, end date, and status

---

### 💳 PAYMENT

Handles financial transactions related to subscriptions.

* Tracks payment status, method, and timestamps

---

### 📅 SESSION

Represents scheduled interactions between trainer and client.

* Can include consultations or live coaching sessions

---

### 📝 CHECKIN

Represents periodic progress updates submitted by clients.

* Includes weight, notes, and submission date

### 📊 PROGRESS_METRICS

Stores detailed body measurements for each check-in:

* Chest, waist, biceps, body fat percentage

---

### 💬 TRAINER_NOTES

Stores feedback provided by trainers on client check-ins.

---

## 🔗 Relationships Overview

* A **User** can be either a Trainer or a Client (via profile tables)
* A **Trainer** can create multiple Plans
* A **Client** can subscribe to multiple Plans over time
* Each **Subscription** can have multiple Payments, Sessions, and Check-ins
* Each **Check-in** can have associated Progress Metrics and Trainer Notes

---

## 📷 ER Diagram

![Fitness Influencer Coaching Platform](./Fitness%20Influencer%20Coaching%20Platform.png)

---

## 🎯 Design Highlights

* ✅ **Normalized structure** with clear separation of concerns
* ✅ **Role-based user system** using profile tables
* ✅ **Flexible subscription model** supporting multiple plans per client
* ✅ **Scalable progress tracking system** using check-ins and metrics
* ✅ **Real-world practicality** with payments, sessions, and feedback

---

## 🚀 Use Cases Supported

* Onboarding trainers and clients
* Selling coaching programs
* Managing subscriptions and renewals
* Scheduling sessions and consultations
* Tracking client fitness progress over time
* Providing structured trainer feedback

---

## 🏁 Conclusion

This ER diagram provides a scalable and practical foundation for building a real-world **online fitness coaching platform**, covering core business workflows from onboarding to progress tracking.

---
