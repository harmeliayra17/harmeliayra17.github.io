---
title: "Tixtoria - E-Ticketing Event Website"
date: 2024-12-05 00:00:00 +0800
categories: [Web Project]
tags: [Tixtoria, Event, Ticketing, Web Development, PHP, CRUD]
image: /assets/img/tixtoria-banner.png
---

## Tixtoria - E-Ticketing Event Website

**Tixtoria** is a modern e-ticketing system designed to manage events digitally. This website enables **admins**, **event organizers**, and **visitors** to interact seamlessly in event management and ticket reservations with a structured, secure, and user-friendly experience.

---

## 🎯 Project Overview

This system supports multiple user levels:

### 1. Admin
- Manage all event data, user accounts, and ticket sales reports.
- Delete inactive user accounts.

### 2. Event Organizer
- Add, edit, and delete their own events.
- View ticket reservations for their events.

### 3. Registered User (Visitor)
- Book tickets, save favorite events, and view booking history.
- Cancel bookings if within the cancellation window.

### 4. Guest (Public Visitor)
- Can view event listings and details.
- Must log in/sign up to book or save events.

---

## 🧩 CMS Modules

### 🔐 User Management (Admin)
- **Create/Edit/Delete Users**: name, email, password, role.
- **Validation**: all fields must be valid.
- **User List**: display all users.

### 🎉 Event Management (Admin & Organizer)
- **Create/Edit/Delete Events**: name, description, time, location, price, quota, image.
- Organizers can only manage their own events.

### 🎟 Ticket Management
- **View Bookings**: see all ticket bookings per event.
- **Manage Ticket Status**: approve/cancel tickets.
- **Reports**: real-time ticket sales and status (Admin only).

### 📦 Booking Management (Registered User)
- **Book Tickets**: automatically reduces the quota.
- **Cancel Tickets**: restores quota if canceled in time.
- **View Booking History** and **Save Events to Favorites**.

---

## 🖼 Layout Overview

### 🔑 Login & Register  
- Login: available for admin, organizer, and user.  
- Register: only available for regular users.

![Login Page](/assets/img/event-login.png)  
![Register Page](/assets/img/event-register.png)

---

### 🏠 Homepage (Guest & Registered)
- List of latest/popular events.
- Search bar for name/category/location.
- Login/Register buttons for guests.

![Homepage](/assets/img/event-home.png)

---

### 📅 Event Catalog
- Display all events: name, image, time, location.
- Filter & sort by category, location, or date.

### 📌 Event Detail Page
- Full information: description, price, time, quota, location.
- "Book Ticket" button (only visible to logged-in users).
- "Save to Favorites" button.

---

### 👤 User Dashboard
- **Profile**: edit account information.
- **Booking History**: view past ticket purchases.
- **Favorite Events**: list of saved favorite events.

### ⚙️ Admin Dashboard
- **Manage Users**: CRUD for all users.
- **Manage Events**: CRUD for all events.
- **Reports**: ticket sales and reservation statistics.

### 🧾 Organizer Dashboard
- **My Events**: CRUD for their own events.
- **View Bookings**: see bookings for their events.

---

## 📂 Source Code

👉 [View on GitHub](https://github.com/harmeliayra17/Tixtoria-event-ticketing-laravel-web)

---