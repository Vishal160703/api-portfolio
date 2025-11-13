# 🧪 How to Test an API using Postman

This guide explains **how to test a REST API using Postman**, one of the most popular tools for API testing.  
By the end, you’ll know how to send GET, POST, PUT, and DELETE requests to an API.

---

## 🎯 Objective
To learn the basics of API testing using the **ReqRes API** (`https://reqres.in`).

---

## 🧰 Prerequisites
- Installed **Postman** (available for free at [https://www.postman.com/downloads](https://www.postman.com/downloads))
- Basic understanding of what an **API** and an **endpoint** are.

---

## 🪜 Step 1: Open Postman

1. Launch **Postman** on your system.  
2. Click on **New Tab** or press `Ctrl + T`.  
3. You’ll see a request builder interface with dropdowns for HTTP methods (GET, POST, etc.).

---

## 🪜 Step 2: Send a GET Request

1. In the URL field, enter:
https://reqres.in/api/users?page=2
2. Select **GET** from the dropdown.
3. Click **Send**.
4. You’ll get a JSON response containing a list of users.

**Response Example:**
```json
{
"page": 2,
"data": [
 {
   "id": 7,
   "email": "michael.lawson@reqres.in",
   "first_name": "Michael"
 }
]
}
✅ Congratulations! You’ve made your first successful API call.
