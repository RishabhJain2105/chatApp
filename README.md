"# chatApp" 

NAME - RISHABH JAIN
UNIVERSITY - Indian Institute of Technology Jammu
Department - Computer Science and Engineering

This is a demo video demonstrating the functionality of the chatapp-
[chatapp demo.webm](https://github.com/user-attachments/assets/c3caaa63-4914-41d7-a58a-73d2cb7a0ce5)\


**ChatApp**
A real-time chat application built using Next.js (full-stack) and MongoDB. It allows users to communicate in private or group chat rooms with real-time updates and notifications.

**Features**
1) Real-time Messaging: Live chat updates powered by WebSockets.
2) User Authentication: Secure login and signup with JWT authentication.
3) Group and Private Chat: Users can create private chats or group rooms.
4) Responsive UI: Mobile-friendly design with a modern user interface.

**Tech Stack**
Frontend & Backend: Next.js
Database: MongoDB
Real-time Communication: Socket.IO
Authentication: JWT (JSON Web Tokens)


**System Design**
1. Architecture Overview
The app follows a full-stack approach using Next.js for both frontend and backend. MongoDB serves as the primary database for storing user information, chat histories, and chat rooms.

- Frontend: Next.js Pages for the user interface.
- Backend: Next.js API routes for backend logic (authentication, messaging, etc.).
- Database: MongoDB with Mongoose for managing and storing data.
- Real-time Communication: Socket.IO for enabling real-time messaging between users.
- 
2. Database Design
Users Collection: Stores user data like username, email, password hash, and status.
Messages Collection: Logs messages sent in chat rooms with sender details and timestamps.
ChatRooms Collection: Keeps track of chat room participants and metadata.

**Setup Instructions**
1. Prerequisites
Node.js (v14 or higher)
MongoDB (running instance either local or cloud)

2. Installation
a) Clone the repository:
git clone https://github.com/RishabhJain2105/chatApp.git
cd chatApp
   
b) Install dependencies:
npm install

c) Set up environment variables: Create a .env.local file in the root directory with the following content:
MONGO_URI=mongodb://localhost:27017/chatapp
JWT_SECRET=your_jwt_secret_key
NEXT_PUBLIC_SOCKET_URL=http://localhost:4000

d) Run MongoDB: Ensure MongoDB is running locally, or provide a valid remote MongoDB URI in .env.local.

e)Start the development server:
npm run dev

3. Running the Application
Frontend & Backend: Next.js serves both the frontend and backend via API routes.
Socket.IO: Provides real-time communication for chats.
Visit http://localhost:3000 to view the application.

Dependencies
Next.js: Full-stack React framework for SSR, routing, and API routes.
MongoDB & Mongoose: For storing and managing user and chat data.
Socket.IO: Enables real-time, bidirectional communication between the client and server.
JWT (JsonWebToken): Provides secure authentication and session management.
