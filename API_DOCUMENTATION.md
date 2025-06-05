
# Users API Summary

**Base URL:** `http://localhost:3000/users`

---

## Endpoints

### 1. Get All Users  
**GET /**  
Returns a list of all users.

---

### 2. Get User by ID  
**GET /:id**  
Returns user details by user ID.  
- Returns 404 if user not found.

---

### 3. Create User  
**POST /**  
Create a new user.  
Request body (JSON):
```json
{
  "name": "Name",
  "email": "email@example.com",
  "age": 30
}
```
- Returns 201 Created on success.

---

### 4. Update User  
**PUT /:id**  
Update user by ID.  
Request body (JSON):
```json
{
  "name": "Updated Name",
  "email": "updated_email@example.com",
  "age": 31
}
```
- Returns 404 if user not found.

---

### 5. Delete User  
**DELETE /:id**  
Deletes user by ID.  
- Returns 404 if user not found.

---

## Notes

- Use header `Content-Type: application/json` for POST and PUT requests.  
- All responses are in JSON format.  
- Make sure your server is running on port 3000 or update the base URL accordingly.
