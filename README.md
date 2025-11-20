# api_chaining
this repository contains mini project ,in which i can run a complete API workflow in one go and can pass variables dynamically and chain requests


•  Your collection name: reqresapi flow automation
•  APIs included:
1.Login successful
Request/api/login
{
    "email": "eve.holt@reqres.in",
    "password": "cityslicka"
}
Extract token from response

2.create user data using this token
Request/api/users
{
    "name": "morpheus",
    "job": "leader"
}
Extract userid from response
3.Put
/api/users/2
{
    "name": "morpheus",
    "job": "zion resident"
}
Update data using userid extract from last field
4.Delete  using userid
reqres.in/api/users/2

5. Add a Pre-request Script in “Login” to print timestamp: (Optional) pm.environment.set("runStartTime", new Date().toISOString()); 
console.log("Run started at:", pm.environment.get("runStartTime")); 

5 Open Collection Runner Use Collection 

6 - Run the Collection and observe 
Token gets stored
 User created
 User fetched
 User deleted
 All tests run automatically 
✅ Expected Output: 
All 4 requests executed in sequence
 Tests show “Passed” 
Token and userid handled dynamically

•  Tools used (Postman)
•  Your GitHub repo name: https://github.com/Manpreet-90/api_chaining.git

