# GitHub API Documentation (Sample)

This documentation provides an overview of basic GitHub REST API endpoints.  
These APIs allow users to manage repositories, users, and issues programmatically.

---

## 🧠 Overview

**Base URL:** `https://api.github.com`  
**Authentication:** Token-based (Bearer Token)

Example header:
```bash
Authorization: Bearer YOUR_GITHUB_TOKEN
1️⃣ GET /users/{username}

Retrieves public information about a GitHub user.

Example Request:

GET https://api.github.com/users/octocat


Response:

{
  "login": "octocat",
  "id": 1,
  "public_repos": 8,
  "followers": 3932
}


Response Code: 200 OK

2️⃣ POST /user/repos

Creates a new repository for the authenticated user.

Headers:

Authorization: Bearer YOUR_GITHUB_TOKEN
Content-Type: application/json


Request Body:

{
  "name": "my-new-repo",
  "description": "This is a test repository created via API",
  "private": false
}


Response:

{
  "id": 123456,
  "name": "my-new-repo",
  "full_name": "vishal160703/my-new-repo",
  "private": false
}


Response Code: 201 Created

3️⃣ DELETE /repos/{owner}/{repo}

Deletes a repository owned by the authenticated user.

Example:

DELETE https://api.github.com/repos/vishal160703/test-repo


Response Code: 204 No Content
