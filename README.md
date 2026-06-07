# 📊 Employee Management System (Full-Stack)

A robust, full-stack **CRUD (Create, Read, Update, Delete)** application built to efficiently manage employee information. This project features a responsive user interface built with **React** and a secure, structured **RESTful API** powered by **Spring Boot and MySQL**. 

Originally built as a personal development project, this application has been fully adopted and is currently utilized by a local community sports club.

---

## 📋 Table of Contents
1. [Links & Repositories](#-links--repositories)
2. [Aims and Motivation](#-aims-and-motivation)
3. [Tech Stack & Architecture](#-tech-stack--architecture)
4. [Key Features](#-key-features)
5. [API Testing & Custom Exceptions](#-api-testing--custom-exceptions)
6. [Application Walkthrough (UI)](#-application-walkthrough-ui)

---

## 🔗 Links & Repositories
* **Front-end Repository (React):** [Employee-Management-Frontend]()
* **Back-end Repository (Spring Boot):** [Employee-Management-System]()

---

## 🎯 Aims and Motivation
* **Full-Stack Integration:** The primary goal was to master end-to-end web development by successfully bridging a Java-based enterprise backend with a modern JavaScript frontend framework.
* **Continuous Learning:** Driven by a passion for self-improvement, this project was meticulously designed, refined, and tested during personal time to understand production-grade RESTful API patterns, data persistence, and state synchronization.

---

## ⚙️ Tech Stack & Architecture

### Architectural Overview
The system follows a traditional client-server architecture. The React client communicates asynchronously with the Spring Boot server using Axios HTTP promises, which in turn queries and persists structural data into a MySQL relational database.

![spring-boot-react-crud-example-rest-api-architecture](https://github.com/Saad1929/Employee-Management-System/assets/108022733/9951b53f-cf9c-4bf8-830f-654fa135789f)

### Technologies & Software Tools
* **Languages:** Java, JavaScript (ES6+), HTML5, CSS3, JSON, SQL
* **Back-end Framework:** Spring Boot (Java)
* **Front-end Library:** React.js
* **Database Management:** MySQL (via MySQL Workbench & DataGrip)
* **Styling & Layout:** Bootstrap (For responsive navbar structures and data tables)
* **API Client:** Postman (End-point simulation and mutation verification)

### Core Dependencies (Frontend Package Manager)
* `axios` — Handles asynchronous HTTP requests (`GET`, `POST`, `PUT`, `DELETE`) and intercepts JSON payload transformations.
* `react-router-dom` — Handles client-side routing using structural elements like `<BrowserRouter>`, `<Routes>`, and `<Route>` to maintain seamless page navigation.

---

## ✏️ Key Features

### Back-end Design
* **Object-Relational Mapping (ORM):** Leveraged **Jakarta Persistence API (JPA)** annotations (`@Entity`, `@Id`, `@GeneratedValue`) to bind standard Java classes natively to MySQL schemas.
* **Robust Exception Handling:** Programmed custom global exceptions to elegantly intercept database anomalies, such as attempting to fetch or mutate an Employee record utilizing an invalid or non-existent User ID.

### Front-end Design
* **Responsive UI:** Styled entirely via Bootstrap to guarantee proper grid scaling across mobile, tablet, and desktop viewports.
* **Real-time Data Sync:** Combined React hook state arrays with Axios endpoint listeners to dynamically re-render view states immediately following data mutations.

---

## 🧪 API Testing & Custom Exceptions

**Postman** was heavily utilized as our API validation workbench to ensure payload schemas adhered closely to REST conventions before frontend connection took place.

![postman](https://github.com/Saad1929/Employee-Management-System/assets/108022733/e045a6d9-48a6-46d8-8c78-daa6cb444606)

### Postman Test Suite Assertions

#### 1. GET Request (Standard Resolution)
Fetches a list of all active employee profiles inside the relational system.
<img width="800" alt="GET" src="https://github.com/Saad1929/Employee-Management-System/assets/108022733/6f37bf38-071f-4d61-b4a7-7569e4730129">

#### 2. GET Request (Custom Exception Triggered)
Demonstrates custom exception mapping. Querying a non-existent account ID properly returns a tailored error payload instead of crashing the stack.
<img width="800" alt="GET ERROR" src="https://github.com/Saad1929/Employee-Management-System/assets/108022733/ec068261-bc66-4f0e-b36f-d38889d2ae12">

#### 3. POST Request (Resource Creation)
Submits a brand-new JSON object to persist record properties seamlessly onto the backend database layer.
<img width="800" alt="Get   Post" src="https://github.com/Saad1929/Employee-Management-System/assets/108022733/ada4d1d1-fc66-4223-ac29-434f0d8fc446">

#### 4. PUT Request (Resource Mutation)
Modifies specific property sets safely across established schema values using id-targeted endpoint hooks.
<img width="1440" alt="PUT" src="https://github.com/Saad1929/Employee-Management-System/assets/108022733/2d978d20-75d9-43a1-96e2-d05f067df848">

#### 5. DELETE Request (Exceptional Scope Resolution)
Fails cleanly when trying to strip a non-existent database key index.
<img width="800" alt="DELETE ERROR" src="https://github.com/Saad1929/Employee-Management-System/assets/108022733/7c54018f-ee71-4e11-a222-70e17cd6970a">

---

## 📱 Application Walkthrough (UI)

Below are operational visual captures showcasing layout flow, interactive client features, and interface component structures.

### Main Control Dashboard (Home View)
A structured Bootstrap table displaying all compiled system entities along with action routing anchors.
<img width="800" alt="Home Page" src="https://github.com/Saad1929/Employee-Management-Frontend/assets/108022733/72a9d9bc-72d9-4fdd-8831-aaca7be66f5b">

### Register New User Interface
An intuitive input form that dynamically maps fields to a new database entity payload via state handlers.
<img width="800" alt="Register User Page" src="https://github.com/Saad1929/Employee-Management-Frontend/assets/108022733/df315549-767e-4ceb-81d4-28027ab0afb1">

### Isolated Record Detail Viewer
Renders single records cleanly in an organized card layout to view a specific user's properties.
<img width="800" alt="View User Details Page" src="https://github.com/Saad1929/Employee-Management-Frontend/assets/108022733/eaa864f1-6f93-4bde-960e-00e7f078cfe9">

### Edit / Modify Record Form
Pre-populates active database attributes inside context input elements, ready for live record mutation updates.
<img width="800" alt="Edit User Page" src="https://github.com/Saad1929/Employee-Management-Frontend/assets/108022733/8db8229f-f421-4cfa-8ae5-1e5a37b2758c">
