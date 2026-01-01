# 🅿️ BPark - Automated Parking Management System

![Java](https://img.shields.io/badge/Java-17+-orange?style=flat-square&logo=openjdk)
![JavaFX](https://img.shields.io/badge/JavaFX-21-blue?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat-square&logo=mysql&logoColor=white)

A comprehensive parking lot management system with automated vehicle tracking, reservations, and real-time monitoring.

**Developed as part of the Software Engineering course at Braude College.**

---

## Features

**Subscribers** - Login, make reservations, extend parking, view history, RFID tag support

**Staff** - Register subscribers, manage vehicle entry/exit, monitor active parkings

**Managers** - View parking reports, subscriber analytics, availability dashboard

**Automation** - Late detection alerts, email notifications, auto-cancel unused reservations

---

## Quick Start

### Using JAR Files (Recommended)

```bash
# 1. Setup database
mysql -u root -p < G1_Assignment3-DB.sql

# 2. Run server
java --module-path /path/to/javafx/lib --add-modules javafx.controls,javafx.fxml,javafx.media -jar JAR/G1_Server.jar

# 3. Run client
java --module-path /path/to/javafx/lib --add-modules javafx.controls,javafx.fxml,javafx.media -jar JAR/G1_Client.jar
```

### Demo Credentials

| Role | Username | Password |
|------|----------|----------|
| Manager | `manager1` | `hash3` |
| Attendant | `sadran1` | `hash1` |
| Subscriber | `shiraB` | `hash2` |

---

## Project Structure

```
BPark/
├── BPark-code/
│   ├── BPark_Client/    # JavaFX client (controllers, FXML, CSS)
│   ├── BPark_Server/    # Server, DB controller, mail service
│   ├── BPark_Common/    # Shared models (Subscriber, Order, etc.)
│   └── OCSF/            # Client-Server framework
├── JAR/                 # Pre-built executables
├── javadoc/             # API documentation
└── G1_Assignment3-DB.sql
```

---

## Tech Stack

- **Frontend:** JavaFX 21, FXML, CSS
- **Backend:** Java 17+, OCSF Framework
- **Database:** MySQL 8.0
- **Email:** Jakarta Mail (Gmail SMTP)

---

## Configuration

**Database** - Edit connection in `BPark-code/BPark_Server/src/db/DBController.java`

**Email** - Update Gmail credentials in `BPark-code/BPark_Server/src/mailService/MailService.java`

---

## Documentation

Full Javadoc available in `javadoc/doc.rar`

---

## Authors

**Group 1** - Braude College of Engineering

- Amit Derei
- Liron Zino
- Miron Hanukaiev
- Ravid Shalev
- Eliran Melihov
