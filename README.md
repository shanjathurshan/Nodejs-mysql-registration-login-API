# node-mysql-registration-login-api

Node.js + MySQL API for User Management, Authentication and Registration

For documentation and instructions see https://jasonwatmore.com/post/2020/08/18/nodejs-mysql-simple-api-for-authentication-registration-and-user-management# Nodejs-mysql-registration-login-API

# How to register a new user with Postman
To register a new user with the api follow these steps:

- Register (POST) - http://localhost:4000/users/register
```
{
    "firstName": "shan",
    "lastName": "jathu",
    "username": "shan",
    "password": "my-super-secret-password"
}
```

- Login (POST) - http://localhost:4000/users/authenticate

```
{
    "username": "shan",
    "password": "my-super-secret-password"
}
```

- How to make an authenticated request to retrieve all users \
 (GET) http://localhost:4000/users \
Select the "Authorization" tab below the URL field, change the type to "Bearer Token" in the type dropdown selector, and paste the JWT token from the previous authenticate step into the "Token" field.

- Get user by Id (GET) - http://localhost:4000/users/1

- update user by Id (PUT) - http://localhost:4000/users/1 
```
{
    "firstName": "shana",
    "lastName": "jathu",
    "username": "jathu",
    "password": "123456"
}
```

Have a good day!
