# Social-Network-Mongo
NoSQL Challenge: Social Network API
Welcome to the Social Media Startup API documentation. This API is designed to provide the backend functionality for your social network platform, enabling you to handle large amounts of unstructured data using a NoSQL database. The API is built using Express.js for routing, MongoDB for the database, and Mongoose ODM for seamless interaction with the database.

## Getting Started
To set up and run the Social Media Startup API on your local machine, follow these steps:
1. git clone <repository_url>
2. cd social-media-api
3. npm install
4. Configure the MongoDB connection: Open the config.js file and replace the mongoURI with your MongoDB connection string.
5. Start the server and sync Mongoose models to the MongoDB database: "npm start"

## API Routes 
Once the server is up and running, you can interact with the API using the following routes:
GET /api/users

Fetches a list of users from the database.
Response: Formatted JSON containing user data.
GET /api/thoughts

Retrieves a list of thoughts from the database.
Response: Formatted JSON containing thought data.
POST /api/users

Creates a new user in the database.
Request: JSON payload containing user details.
Response: Formatted JSON confirming the creation of the user.
POST /api/thoughts

Creates a new thought in the database.
Request: JSON payload containing thought details.
Response: Formatted JSON confirming the creation of the thought.
PUT /api/users/:userId

Updates user details in the database.
Request: JSON payload containing updated user data.
Response: Formatted JSON confirming the update.
DELETE /api/users/:userId

Deletes a user and associated data from the database.
Response: Formatted JSON confirming the deletion.
DELETE /api/thoughts/:thoughtId

Deletes a thought from the database.
Response: Formatted JSON confirming the deletion.
POST /api/users/:userId/friends/:friendId

Adds a friend to a user's friend list.
Response: Formatted JSON confirming the addition of the friend.
DELETE /api/users/:userId/friends/:friendId

Removes a friend from a user's friend list.
Response: Formatted JSON confirming the removal of the friend.
POST /api/thoughts/:thoughtId/reactions

Adds a reaction to a thought.
Request: JSON payload containing reaction details.
Response: Formatted JSON confirming the addition of the reaction.
DELETE /api/thoughts/:thoughtId/reactions/:reactionId

Removes a reaction from a thought.
Response: Formatted JSON confirming the removal of the reaction.

## Testing
You can use tools like Insomnia or Postman to test the API routes as mentioned in the project requirements. Make sure you have the appropriate request payload and HTTP method when testing each route.

## Conclusion 
Congratulations! You now have a fully functional API for your social network startup that uses a NoSQL database to handle large amounts of unstructured data. If you have any questions or encounter issues, feel free to reach out to our support team.


https://drive.google.com/file/d/1uKjylVw6dYeaEpOuUAr8NTe9e3tkXkmz/view