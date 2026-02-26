#  E-Commerce API Testing Project (Postman + Newman + Custom API)

## 📌 Project Overview

This project demonstrates complete end-to-end API Testing of an E-Commerce system using Postman and Newman.

It includes:

✔ Public API Testing (DummyJSON)  
✔ Custom API Creation using json-server  
✔ Functional & Negative Testing  
✔ Schema Validation  
✔ Data Driven Testing  
✔ Automation Execution & HTML Reporting  

This project simulates real-world QA API testing workflow.

---

#  Tools & Technologies Used

- Postman (API Testing & Automation)
- Newman (CLI Execution)
- Node.js (Runtime Environment)
- json-server (Mock REST API Creation)
- DummyJSON (Public Fake API)
- GitHub (Project Hosting)

---

# 🌐 Part 1: Public API Testing (DummyJSON)

Base URL:
https://dummyjson.com

Modules Tested:

- Authentication (Login API)
- Get All Products
- Get Product by ID
- Add to Cart
- View Cart
- Update Cart
- Order Simulation
- Negative Test Cases

Testing Techniques Used:

- Status Code Validation
- Response Body Validation
- Schema Validation
- Performance Validation (Response Time Check)
- Dynamic Variable Chaining
- Environment Variables
- Pre-request Scripts

---

#  Part 2: Custom API Creation (Using json-server)

A custom REST API was created locally using json-server.

## Steps Performed:

1️⃣ Installed json-server globally:

npm install -g json-server

2️⃣ Created a db.json file containing sample data.

Example:

{
  "products": [
    { "id": 1, "name": "Laptop", "price": 50000 },
    { "id": 2, "name": "Mobile", "price": 30000 }
  ]
}

3️⃣ Started local API server:

json-server db.json

4️⃣ Local API Base URL:

http://localhost:3000

Available Endpoints Automatically Created:

- GET /products
- GET /products/1
- POST /products
- PUT /products/1
- DELETE /products/1

5️⃣ Tested all endpoints using Postman.

---

#  Types of Testing Performed

## ✅ Functional Testing
Verified correct response for valid requests.

##  Negative Testing
Tested invalid scenarios:
- Invalid product ID
- Invalid cart ID
- Empty request body
- Wrong HTTP method

## 📦 Schema Validation
Validated:
- Required fields
- Data types
- JSON structure

## 🔄 Dynamic Testing
- Saved response data in environment variables
- Used dynamic IDs in chained requests

##  Data Driven Testing
Executed requests using CSV file in Collection Runner.

## ⏱ Performance Testing
Validated response time under defined threshold.

---

#  Automation Using Newman

Collection executed via Newman CLI.

Command Used:

newman run collection.json -e env.json -r htmlextra

Generated:

- Detailed HTML Execution Report
- Test Case Summary
- Pass/Fail Status
- Response Time Analysis

---

#  Project Structure

E-Commerce-API-Testing

├── Postman Collection JSON

├── Environment JSON

├── db.json (Custom API Data)

├── HTML Report

├── Screenshots

└── README.md

---

#  Learning Outcomes

Through this project, I gained hands-on experience in:

- Creating REST APIs using json-server
- Understanding request-response lifecycle
- Writing Postman test scripts (JavaScript)
- Schema validation techniques
- API automation using Newman
- Generating professional test reports
- Structuring API testing project for portfolio

---

#  Why This Project Matters

This project demonstrates:

✔ Ability to create APIs  
✔ Ability to test APIs  
✔ Automation knowledge  
✔ Professional documentation skills  
✔ Understanding of backend architecture  

---

#  Author

Mueza  
Manual & API Tester
