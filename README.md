Webtoon Library App
Project Overview
This project is a Webtoon Library App created as part of the AnimeMangaToon Internship assignment. The app allows users to browse webtoons, view detailed information about each webtoon, and manage their favorite webtoons after logging in.

The project demonstrates full-stack web development using:

React for the front-end
Node.js/Express for the back-end API
MongoDB for the database
JWT (JSON Web Token) for user authentication
Heroku (or AWS) for deployment
Features
Home Page: Displays a list of popular webtoons with over 50 million views. Each webtoon includes a title, description, and thumbnail image.
Webtoon Detail Page: Provides detailed information about a selected webtoon, including an enlarged image and a comments section.
User Authentication: Allows users to register, log in, and manage their accounts using JWT.
Favorites Page: Allows logged-in users to add webtoons to their favorites and view them on a separate page.
Responsive Design: The app is fully responsive and optimized for both mobile and desktop use.
RESTful API: The back-end API provides data about webtoons and handles user authentication.
Technologies Used
Front-End:
React (JavaScript)
HTML5 / CSS3 (for layout and styling)
Axios (for making API calls)
Back-End:
Node.js
Express.js
MongoDB (with Mongoose)
JSON Web Tokens (JWT) for authentication
Bcrypt.js for password hashing
Deployment:
Heroku (or AWS) for hosting
MongoDB Atlas (for remote database)
Project Structure
bash
Copy code
root/
│
├── client/               # React Front-end
│   ├── src/
│   ├── public/
│   └── package.json
│
├── server/               # Node.js Back-end
│   ├── routes/
│   ├── models/
│   └── server.js
│
├── README.md             # Project documentation
├── package.json          # Back-end dependencies
└── .env                  # Environment variables (e.g., database URI, JWT secret)
How to Run the Project Locally
Prerequisites
Node.js installed on your machine
MongoDB (you can use MongoDB Atlas or a local instance)
Steps
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/webtoon-library-app.git
cd webtoon-library-app
Install dependencies for both front-end and back-end:

bash
Copy code
cd client
npm install   # Install React dependencies

cd ../server
npm install   # Install Node.js dependencies
Create a .env file in the server directory with the following:

bash
Copy code
MONGODB_URI=mongodb://localhost:27017/webtoon-library
JWT_SECRET=your-secret-key
Run the back-end server:

bash
Copy code
cd server
npm start
Run the front-end:

bash
Copy code
cd client
npm start
Access the app by navigating to http://localhost:3000 in your browser.

Deployment
The app is deployed on Heroku (or AWS). You can access the live version of the app here (replace with your actual URL).

API Endpoints
GET /api/webtoons: Retrieve a list of all webtoons.
GET /api/webtoons/
: Retrieve details of a specific webtoon.
POST /api/auth/register: Register a new user.
POST /api/auth/login: Authenticate a user and return a JWT.
POST /api/favorites: Add a webtoon to user’s favorites.
GET /api/favorites: Retrieve user's favorite webtoons.
Future Enhancements
Implement a real-time comments feature for webtoons.
Add pagination for the webtoon list on the home page.
Improve error handling and validation across the app.
License
This project is licensed under the MIT License - see the LICENSE file for details.
