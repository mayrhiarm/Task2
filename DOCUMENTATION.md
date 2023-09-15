# API Documentation

Welcome to the documentation for the **HNGx Person API**. This API provides basic CRUD operations for managing persons.
hosted url - [Person API](https://mayrhiarm.onrender.com)
## Table of Contents

- [API Endpoints](#api-endpoints)
  - [Create a New Person](#create-a-new-person)
  - [Fetch Details of a Person](#fetch-details-of-a-person)
  - [Update Details of a Person](#update-details-of-a-person)
  - [Remove a Person](#remove-a-person)
- [Request and Response Formats](#request-and-response-formats)
- [Known Limitations](#known-limitations)

## API Endpoints

### Create a New Person

**Endpoint:** `/api`

**Method:** POST

**Request Format:**
```json
{
  "name": "Mariam"
}
```
**Response Format (Success - HTTP 201 Created):**
```json
{
  "id": 1,
  "name": "Mariam",
  "response": "Mariam created successfully",
  "username": "Mariam466"
}
```


**Response Format (Error - HTTP 400 Bad Request):**
```json
{
  "response": "1 contains an integer, not allowed",
  "status_code": 400
}
```

## Fetch Details of a Person
**Endpoint:** /api/<person_id>

**Method:** GET

**Response Format (Success - HTTP 200 OK):**
```json
{
  "id": 1,
  "name": "Mariam",
  "username": "Mariam466"
}
```


**Response Format (Error - HTTP 404 Not Found):**
```json
{
  "error": "No Result with id=9 Found"
}
```
## Update Details of a Person
**Endpoint:** /api/<person_id>

**Method:** PUT or PATCH

**Request Format:**
```json
{
  "name": "John",
}
```
**Response Format:**
```json
{
  "id": 1,
  "name": "John",
  "response": "user update",
  "status_code": 201,
  "username": "Mariam466"
}
```

## Remove a Person
**Endpoint:** /api/<person_id>

**Method:** DELETE

**Response Format (Success - HTTP 204 No Content):**

No response body.

**Response Format (Error - HTTP 404 Not Found):**

```json
{
  "response": "user with 3 has been deleted"
}
```


## Request and Response Formats
All API endpoints accept and return data in JSON format.
Ensure that the request and response data adhere to the specified formats mentioned above.

## Known Limitations

- The API does not support pagination.
- The API does not support filtering.
- The API does not support sorting.
- This documentation assumes a local development setup.
- Authentication and authorization mechanisms are not implemented

