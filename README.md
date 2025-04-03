# MyMirro Backend

This is the backend implementation for MyMirro, a fashion recommendation platform that provides personalized outfit suggestions based on user preferences.

## Features
- User authentication (JWT-based).
- Dynamic recommendations based on user preferences.
- MongoDB database integration.
- RESTful API endpoints for user management, clothing items, and recommendations.

## Tech Stack
- Node.js with Express.js (Backend Framework)
- MongoDB (Database)
- JWT (Authentication)
- Docker (Containerization)

## Setup Instructions

### Prerequisites
- Node.js v18+
- MongoDB (Local or Atlas)
- Postman (for API testing)

### Installation
1. Clone this repository:
    ```
    git clone https://github.com/yourusername/mymirro-backend.git
    cd mymirro-backend
    ```

2. Install dependencies:
    ```
    npm install
    ```

3. Create a `.env` file in the root directory and add:
    ```
    MONGODB_URI=mongodb://localhost:27017/mymirro
    JWT_SECRET=your_secret_key
    PORT=3000
    ```

4. Start the server:
    ```
    node app.js
    ```

5. The server will be running at `http://localhost:3000`.

## API Endpoints

### Authentication
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Log in an existing user.

### Recommendations
- `GET /api/recommendations`: Fetch personalized recommendations.

### Clothing Items
- `GET /api/items`: Retrieve clothing items based on filters.

## Testing APIs with Postman
1. Import the provided Postman collection (`MyMirro.postman_collection.json`) into Postman.
2. Test endpoints by sending requests with required headers and body data.

## Contribution Guidelines
Feel free to fork this repository and submit pull requests for improvements or bug fixes.

## License
This project is licensed under the MIT License.
