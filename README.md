# Bostman

A **service-oriented web application** developed as part of the *Aspects and Service Oriented Programming* course.
The project demonstrates the design and implementation of a modular backend using RESTful services and aspect-oriented programming, paired with a responsive frontend to interact with the services.

---

## 🧠 Overview

Bostman is a full-stack application that showcases:

- **Service-Oriented Architecture** — clean separation of concerns via REST APIs.
- **Aspect-Oriented Programming (AOP)** — applied to handle cross-cutting concerns such as logging, error handling, and validation.
- **Frontend-Backend Integration** — a web UI consuming backend APIs.
- **Database Persistence** — structured data storage using MySQL.

---

## 🚀 Features

**Backend**
- RESTful API endpoints for core app functionality.
- Aspect-Oriented modules for logging, validation, and cross-cutting logic.
- Structured with modular service classes for maintainability.

**Frontend**
- Web interface to interact with backend services.
- Dynamic data display and form submission using JavaScript.

**Database**
- MySQL schema for storing application data.
- SQL scripts included to bootstrap database schema.

---

## 🛠️ Technologies

| Layer         | Technology                   |
|---------------|-----------------------------|
| Backend       | Java, Spring (or equivalent) |
| AOP           | Aspect-Oriented Programming |
| Frontend      | HTML, CSS, JavaScript       |
| Database      | MySQL                       |
| Build / Tools | Maven / Gradle *(if used)*  |

---

## 🛠️ Getting Started

### Prerequisites

Before running the project, make sure you have:

- Java JDK (version 8+)
- MySQL installed and running
- A browser to view the frontend

---

### 🗄️ 1. Database Setup

1. Open MySQL and create a database:

   ```sql
   CREATE DATABASE bostman_db;
   ```

2. Import the provided schema file:

   ```bash
   mysql -u <your-username> -p bostman_db < MySQL.sql
   ```

3. Update database credentials in the backend configuration file (e.g., `application.properties`):

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/bostman_db
   spring.datasource.username=YOUR_USERNAME
   spring.datasource.password=YOUR_PASSWORD
   ```

---

### ⚙️ 2. Run the Backend

1. Navigate to the backend project folder:

   ```bash
   cd bostman
   ```

2. Build the project:

   ```bash
   mvn clean install
   ```

3. Start the server:

   ```bash
   mvn spring-boot:run
   ```

The backend should now be running at:

```
http://localhost:8080
```

---

### 🌐 3. Launch the Frontend

1. Go to the frontend folder:

   ```bash
   cd bostman-frontend
   ```

2. Open `index.html` in your browser  
   *(or use a live server extension if needed).*

The frontend will now communicate with the backend APIs.

