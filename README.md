# REST-API-TASK-4
This is a simple Flask REST API for managing users. It supports creating, reading, updating, and deleting users using an in-memory dictionary.

## Setup

Install Flask:

```bash
pip install flask
```

Run the application:

```bash
python app.py
```

Server URL:

```text
http://localhost:5000
```

## Available Endpoints

### Get All Users

```http
GET /users
```

### Get Total User Count

```http
GET /users/count
```

### Get User by ID

```http
GET /users/<id>
```

### Add a User

```http
POST /users
```

Request Body:

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john@example.com"
}
```

### Update a User

```http
PUT /users/<id>
```

### Delete a User

```http
DELETE /users/<id>
```

## Sample Response

```json
{
  "message": "User added",
  "user": {
    "name": "John Doe",
    "email": "john@example.com"
  }
}
```

## Important

* Data is stored in an in-memory dictionary.
* Restarting the server will remove all stored users.
* This project is intended for learning Flask REST APIs.


User data is stored in memory and will be lost when the server is restarted.
