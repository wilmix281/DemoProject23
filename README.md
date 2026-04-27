# DemoProject About SpringBoot with MicroServices





\*\*\*



\# 🎓 Student Fee Management Microservices Application



\## 📌 Project Overview



This project is built using \*\*Spring Boot Microservices architecture\*\* and demonstrates a \*\*Student Fee Management System\*\*.  

The application uses \*\*Feign Client\*\* for inter-service communication and follows RESTful design principles.



It focuses on managing:



\*   Student information

\*   Fee collection

\*   Receipt generation and viewing



For persistence, an \*\*H2 in‑memory database\*\* is used, making the application lightweight and ideal for demos and learning purposes.



\*\*\*



\## 🧩 Microservices Description



\### 1️⃣ Student Management Service



This service is responsible for handling student-related operations.



\*\*Features:\*\*



\*   Add student details

\*   Store and retrieve student information



\*\*Student Fields:\*\*



\*   Student Name

\*   Student ID

\*   Grade

\*   Mobile Number

\*   School Name



\*\*\*



\### 2️⃣ Fee Collection Service



This service manages student fee payments and receipt generation.  

It communicates with the Student Service using \*\*Feign Client\*\* to validate student information.



\*\*Features:\*\*



\*   Collect student fees

\*   Generate receipts

\*   View receipt details using receipt number



\*\*\*



\## 🌐 REST API Endpoints (Postman URLs)



\### 📘 Student Service APIs



\*   \*\*Insert Student Details\*\*

&#x20;       http://localhost:8080/students



\*\*\*



\### 💰 Fee Collection Service APIs



\*   \*\*Insert Fee Collection Record\*\*

&#x20;       http://localhost:8082/fees/collect



\*   \*\*View Receipt Details by Receipt Number\*\*

&#x20;       http://localhost:8082/receipts/RCP-2026-000001



\*\*\*



\## 🗄️ Database Used



\*   \*\*H2 In-Memory Database\*\*

&#x20;   \*   Used for fast setup and demo purposes

&#x20;   \*   No external database installation required

&#x20;   \*   Each microservice maintains its own isolated schema



\*\*\*



\## 📊 Swagger UI (API Documentation \& Testing)



Swagger is enabled for both microservices to allow easy API exploration and testing.



\### 🧑‍🎓 Student Service Swagger UI



\*   Used for inserting and viewing student records



<!---->



&#x20;   http://localhost:8080/swagger-ui/index.html#/



\*\*\*



\### 🧾 Fee Collection Service Swagger UI



\*   Used for:

&#x20;   \*   Collecting student fees

&#x20;   \*   Viewing receipt details by receipt number (e.g., `RCP-2026-000001`)



<!---->



&#x20;   http://localhost:8082/swagger-ui/index.html#/receipt-controller/getReceipt



\*\*\*



