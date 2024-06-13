# Joke API

This is a RESTful API built with Node.js and Express.js that allows users to interact with a collection of jokes. The API provides various endpoints for retrieving, creating, updating, and deleting jokes.

## Endpoints

### 1. GET /random
Retrieves a random joke from the collection.

### 2. GET /jokes/:id
Retrieves a specific joke by its ID.

### 3. GET /filter?type=<type>
Retrieves a list of jokes filtered by the specified joke type.

### 4. POST /jokes
Creates a new joke. The request body should contain the following properties:
- `text`: The text of the joke.
- `type`: The type of the joke (e.g., "Puns", "Wordplay", "Science", etc.).

### 5. PUT /jokes/:id
Updates an existing joke by its ID. The request body should contain the following properties:
- `text`: The updated text of the joke.
- `type`: The updated type of the joke.

### 6. PATCH /jokes/:id
Partially updates an existing joke by its ID. The request body can contain either the `text` or `type` property, or both.

### 7. DELETE /jokes/:id
Deletes a specific joke by its ID.

### 8. DELETE /jokes/all?key=<masterKey>
Deletes all jokes from the collection. This endpoint requires a master key for authentication purposes.

## Getting Started

To run the API locally, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/joke-api.git`
2. Navigate to the project directory: `cd joke-api`
3. Install dependencies: `npm install`
4. Start the server: `node index.js`
5. The API will be running at `http://localhost:3000`

## Dependencies

The following dependencies are used in this project:

- `express`: Web application framework for Node.js.
- `body-parser`: Middleware for parsing request bodies.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
