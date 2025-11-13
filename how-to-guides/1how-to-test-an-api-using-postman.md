# 🧰 How to Test an API using Postman

APIs (Application Programming Interfaces) allow different software systems to communicate.  
As a Technical Writer, understanding how to test an API helps you write accurate and clear documentation.

---

## 🪜 Step 1: Open Postman

1. Go to [https://www.postman.com/downloads/](https://www.postman.com/downloads/)  
2. Install and launch **Postman**.
https://reqres.in/api/users
---

## 🪜 Step 2: Send a GET Request

1. In the Postman address bar, enter:  

2. Select **GET** as the method.  
3. Click **Send**.  
4. You’ll see a response like this:
```json
{
  "page": 1,
  "data": [
    { "id": 1, "email": "george.bluth@reqres.in" },
    { "id": 2, "email": "janet.weaver@reqres.in" }
  ]
}
Send a POST Request

Change the request type to POST.

Enter this URL:

https://reqres.in/api/users


Go to the Body tab → select raw → choose JSON.

Paste this:

{
  "name": "Vishal",
  "job": "Technical Writer"
}


Click Send.

You’ll receive a 201 Created response like:

{
  "name": "Vishal",
  "job": "Technical Writer",
  "id": "123",
  "createdAt": "2025-11-13T10:00:00.000Z"
}
Try Other Methods (Optional)

PUT → to update data

DELETE → to delete a record
Example:

DELETE https://reqres.in/api/users/2


Response Code: 204 No Content🧾 Notes

Always check the response code for success or error.

Save requests in Collections for future reuse.

Use Postman Console (Ctrl + Alt + C) to debug.

📘 Author: Vishal Kasaudhan
🔗 Test API: ReqRes
