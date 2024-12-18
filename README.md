# PingPals - Real-Time Chat Application

PingPals is a real-time chat application built using the MERN stack, Socket.IO, and Cloudinary, providing a seamless and interactive messaging experience.

## Features

- **User Authentication**: Secure signup and login functionality using JSON Web Tokens (JWT).
- **Real-Time Messaging**: Instant communication powered by Socket.IO.
- **Media Sharing**: Upload and share images using Cloudinary.
- **User Management**: Fetch and display a list of available users to chat with.
- **Responsive Design**: Fully optimized for desktop and mobile devices.

## Technologies Used

### Frontend
- React.js
- HTML5, CSS3
- Axios for API calls

### Backend
- Node.js
- Express.js
- MongoDB (with Mongoose)
- Socket.IO for real-time communication
- Cloudinary for image storage and management

### Others
- JWT for authentication
- CORS for secure cross-origin requests

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/pingpals.git
   cd pingpals
   ```

2. **Backend Setup**:
   - Navigate to the `backend` directory:
     ```bash
     cd backend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Create a `.env` file and configure the following variables:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     CLOUDINARY_CLOUD_NAME=your_cloud_name
     CLOUDINARY_API_KEY=your_api_key
     CLOUDINARY_API_SECRET=your_api_secret
     ```
   - Start the backend server:
     ```bash
     npm start
     ```

3. **Frontend Setup**:
   - Navigate to the `frontend` directory:
     ```bash
     cd ../frontend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the development server:
     ```bash
     npm run dev
     ```

4. **Access the Application**:
   - Open your browser and navigate to: `http://localhost:5173`

## Deployment

The application is deployed on Render. You can access it here: [PingPals](https://pingpals-2.onrender.com).

## Project Structure

- `frontend/`: Contains the React.js frontend code.
- `backend/`: Contains the Express.js backend code, including API routes and Socket.IO configuration.
- `models/`: Defines the MongoDB schemas (e.g., User, Message).
- `controllers/`: Implements the business logic for routes.
- `routes/`: Defines the API endpoints for authentication and messaging.

## API Endpoints

### Authentication
- `POST /api/auth/signup`: User signup
- `POST /api/auth/login`: User login
- `POST /api/auth/logout`: User logout
- `GET /api/auth/check`: Verify authentication status

### Messaging
- `GET /api/messages/users`: Fetch all users
- `GET /api/messages/:id`: Get messages with a specific user
- `POST /api/messages/send/:id`: Send a message to a user

## Future Enhancements

- Implement group chat functionality.
- Add message read receipts.
- Introduce typing indicators for real-time feedback.
- Improve user profile management with editable details.
- Include audio/video calling features.
- Include options to delete/edit messages.


