# Postman API Testing Project

## Project Overview
This project demonstrates API testing using Postman and the JSONPlaceholder REST API. It includes positive and negative test cases to validate HTTP status codes, response data, and response structure.

## Tools & Technologies
- Postman
- REST API
- JavaScript (Postman Tests)
- JSONPlaceholder API

## Test Scenarios

### 1. Create a Post — POST
**Endpoint:** `https://jsonplaceholder.typicode.com/posts`

Validates:
- Status code is 201
- Created post has the expected title
- User ID is correct

### 2. Get a Single Post — GET
**Endpoint:** `https://jsonplaceholder.typicode.com/posts/1`

Validates:
- Status code is 200
- Post ID is 1
- Title and body are not empty
- Response content type is JSON
- Response fields have the expected data types

### 3. Get Posts List — GET
**Endpoint:** `https://jsonplaceholder.typicode.com/posts`

Validates:
- Status code is 200
- Posts list is not empty
- First post has ID 1

### 4. Get a Missing Post — GET
**Endpoint:** `https://jsonplaceholder.typicode.com/posts/9999`

Validates:
- Status code is 404
- Response body matches the observed empty-object