# Simple REST API

A simple REST API built with Node.js and Express.

## Installation

1. Install dependencies:
   ```bash
   npm install
   ```

## Running the Server

Start the server:
```bash
npm start
```

For development with auto-reload:
```bash
npm run dev
```

The server will run on http://localhost:3000

## API Endpoints

- `GET /users` - Get all users
- `GET /users/:id` - Get a user by ID
- `POST /users` - Create a new user (body: { "name": "string", "email": "string" })
- `PUT /users/:id` - Update a user (body: { "name": "string", "email": "string" })
- `DELETE /users/:id` - Delete a user

## Testing

You can test the API using tools like Postman or curl.

Example:
```bash
curl http://localhost:3000/users
```