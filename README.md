# 🎬 Movie Ticket Booking System (C++ & MySQL)

## 📌 Overview
This is a **console-based Movie Ticket Booking System** developed in **C++** using **Object-Oriented Programming (OOP)** concepts and integrated with **MySQL** for persistent seat reservation data.

The system allows:
- Viewing seat layout (available/reserved seats)
- Reserving tickets
- Storing and updating seat status in a MySQL database

---

## 🛠 Features
- **OOP-based design** with a dedicated `Seats` class for seat management.
- **Database integration** with MySQL for real-time seat availability.
- **Persistent storage** — reserved seats remain reserved even after restarting the program.
- **Input validation** for seat number and row number.

---

## 📂 Database Schema
**Table:** `Ticket`

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| RowNumber   | INT       | Row number (1–5) |
| SeatNumber  | INT       | Seat number in the row (1–10) |
| Seat        | INT       | `1` = Available, `0` = Reserved |

---

## 📷 Seat Layout Example
1 2 3 4 5 6 7 8 9 10
1 - - - X - - - - - -
2 - - - - - - X - - -
3 - X - - - - - - - -
4 - - - - X - - - - -
5 - - - - - - - X - -

(- = Available, X = Reserved)

---

## 💻 Technologies Used
- **C++** (Core logic, OOP)
- **MySQL** (Database storage)
- **MySQL Connector/C** (`mysql.h`)
