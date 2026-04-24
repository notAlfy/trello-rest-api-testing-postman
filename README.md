# 🧪 Trello REST API Testing (Postman)
```md
> A hands-on REST API testing project using Postman, demonstrating real-world QA practices including API chaining, validation, and performance testing.

---

## 📌 About the Project

This project demonstrates **end-to-end REST API testing of Trello** using Postman.
It covers core functionalities such as **Boards, Lists, and Cards**, including CRUD operations, request chaining, and automated validation.

The goal of this project is to simulate **real-world QA API testing practices**, including functional, negative, and performance testing.

---

## 🎯 Objectives

* Perform CRUD operations testing on Trello APIs
* Implement **API chaining** using environment variables
* Validate responses using Postman test scripts
* Ensure API reliability through **positive & negative testing**
* Add basic **performance validation**

---

## 📂 Project Structure

```
trello-rest-api-testing-postman/
 ├── trello-api-collection.json
 └── README.md

```

## 🔎 Test Scope

### 📋 Board

* Create a Board
* Get the Board
* Update the Board
* Delete the Board

### 📑 List

* Create a List on Board
* Get the List on Board
* Update the List
* Archive the List

### 📝 Card

* Create a Card
* Get the Card
* Update the Card
* Delete the Card

---

## 🔄 API Workflow (Test Flow)

```text
Create Board → Get Board → Update Board  
        ↓
Create List → Get List → Update List  
        ↓
Create Card → Get Card → Update Card  
        ↓
Delete Card → Verify Deletion  
        ↓
Archive List → Verify Archival
        ↓
Delete Board → Verify Deletion
```

---

## 🧪 Test Scenarios

### ✅ Functional Testing

* Verify successful creation of Board, List, and Card
* Validate retrieval of created resources
* Verify update operations
* Validate deletion of resources

### ⚠️ Edge Case Testing

* Dynamic random data for board/list/card names
* Validation of default/null fields

### ❌ Negative Testing

* Invalid ID handling
* Missing or invalid authentication
* Accessing deleted resources

---

## 📊 Assertions Implemented

* Status code validation
* Response structure validation (`id`, `name`, `url`)
* Data consistency validation using environment variables
* Empty response validation for delete operations
* Response time validation (< 1000ms)

---

## 🔗 Environment Variables

The following variables are used for request chaining:

* `base_url`
* `key`
* `token`
* `boardID`
* `listID`
* `cardID`

---

## ⚡ Performance Testing

A collection-level test ensures:

```javascript
Response time < 1000ms
```

---

## 🛠️ Tools & Technologies

* Postman
* REST API (Trello API)
* JavaScript (Postman test scripts)
* Git & GitHub

```


## ▶️ Getting Started

### 1️⃣ Install Postman

### 2️⃣ Create Trello Account

### 3️⃣ Generate API Key & Token

### 4️⃣ Import Collection JSON file on Postman

### 5️⃣ Setup Environment Variables

Create a new environment and add:

```
base_url = https://api.trello.com/1
key = your_api_key
token = your_token
```

### 6️⃣ Run the Collection

---

## Test Result

<img width="1920" height="1019" alt="Trello APIs result" src="https://github.com/user-attachments/assets/af458914-8517-4db7-b3f0-55129eb00dab" />


## 📈 Key Learnings

* API chaining using environment variables
* Writing reusable test scripts in Postman
* Handling dynamic test data
* Validating API responses effectively
* Performing performance testing

---

## 👨‍💻 Author

**Abrar Nawar Alfy**

🔗 GitHub: https://github.com/notAlfy

---
