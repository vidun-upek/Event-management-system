# 🎟️ EventX – Smart Event Management & Ticketing Platform

EventX is a full-stack event management system built with Spring Boot that enables users to discover events, book tickets, and validate entry using QR codes. The platform also provides real-time analytics and role-based access for organizers and administrators.

---

## 🚀 Features

### 👤 User Features

* User registration and authentication (JWT-based)
* Browse and search events
* Book tickets for events
* Generate and download QR-based tickets

### 🧑‍💼 Organizer/Admin Features

* Create, update, and manage events
* Configure ticket pricing and capacity
* Monitor ticket sales and attendance
* View analytics dashboard (revenue, bookings, trends)

### 🎟️ QR Code Ticketing System

* Unique QR code generated for each ticket
* Secure validation system to prevent duplicate entry
* Real-time verification via backend API

### 📊 Analytics Dashboard

* Total tickets sold per event
* Revenue tracking
* Attendance insights
* Booking trends over time

### ⚡ Real-Time Capabilities

* Live ticket availability updates
* Instant QR validation feedback

---

## 🏗️ Architecture

Frontend (React)
↓
Spring Boot Backend (REST API)
↓
MySQL Database

Optional:

* Redis (Caching)
* WebSockets (Real-time updates)

---

## 🛠️ Tech Stack

**Backend**

* Java 17+
* Spring Boot
* Spring Security (JWT)
* Spring Data JPA

**Frontend**

* React.js

**Database**

* MySQL

**Other Tools**

* ZXing (QR Code Generation)
* WebSocket (real-time updates)
* Docker (optional)

---

## 📂 Project Structure

```
src/
 ├── controller/
 ├── service/
 ├── repository/
 ├── entity/
 ├── dto/
 ├── config/
 └── security/
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/your-username/eventx.git
cd eventx
```

### 2. Configure Database

Update `application.properties`:

```
spring.datasource.url=jdbc:mysql://localhost:3306/eventx
spring.datasource.username=root
spring.datasource.password=yourpassword
```

### 3. Run the Application

```
mvn spring-boot:run
```

---

## 🔐 Authentication

* JWT-based authentication
* Roles:

  * USER
  * ORGANIZER
  * ADMIN

---

## 📊 API Highlights

* `POST /auth/register`
* `POST /auth/login`
* `GET /events`
* `POST /events`
* `POST /tickets/book`
* `GET /tickets/{id}/qr`
* `POST /tickets/validate`

---

## 🎯 Future Improvements

* Payment gateway integration
* Email notifications
* Mobile app for QR scanning
* Advanced analytics with charts
* Microservices architecture

---

## 💡 Motivation

This project was built to simulate a real world scalable event management system with secure ticketing and analytics, demonstrating backend engineering, system design, and problem solving skills.

---

