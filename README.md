

🚀 Space Exploration Dashboard
A web application built using React.js for the frontend and MongoDB for user management. This platform integrates space event data, satellite information, and related news from external APIs. It allows users to explore space-related events in real-time, offering an engaging experience for space enthusiasts and professionals alike.

🌟 Project Overview
The Space Exploration Dashboard is a web-based platform designed for space enthusiasts. It aggregates real-time data about upcoming space events, satellite information, and space news from external APIs, providing users with a comprehensive view of the latest happenings in space. The app features user authentication, allowing users to personalize their experience by saving preferences.

🔭 Why This Project?
This project stems from my passion for space exploration. I aimed to create a platform where space enthusiasts can explore real-time space events and related news in a user-friendly manner. This dashboard serves as a learning experience for both space lovers and tech developers.

🛠️ Tech Stack
Frontend: React.js
Backend: Node.js (Express)
Database: MongoDB for user management
External APIs: Integrated for fetching space event data, satellite info, and news.
Cloud Storage: Cloudinary for avatar storage.
🎮 How It Works
The application functions by fetching data from external APIs to present real-time space-related information. Users can create profiles, explore upcoming space events, check satellite data, and read the latest news. MongoDB is used for user authentication and preference storage, while React.js ensures a dynamic and responsive user interface.

🚀 Future Scope & Unique Features
The project has scope for further expansion to include:

Space mission details
Astronaut profiles
Educational resources for students
The unique feature of the project is the real-time integration of space events and personalized user experiences, making it a go-to platform for anyone interested in space technology and exploration.

🚧 Challenges Faced
Some challenges faced during development:

Managing real-time data flow from multiple APIs without compromising performance.
Efficient user preference management using MongoDB.
🛠️ Installation Guide: How to Run the Project
Step 1: Clone the Repository
bash
Copy code
git clone https://github.com/<your-username>/spaceExploration.git
Step 2: Backend Setup
Navigate to the API folder and install dependencies:

bash
Copy code
cd api
npm install
Open index.js inside the api folder. Modify the CORS origin for development:

javascript
Copy code
origin: ["http://localhost:5000"]
Step 3: MongoDB Setup
Install MongoDB and open MongoDB Compass on your system.

In MongoDB Compass:

Click on "Connect."
Create a new database by clicking the "+" icon on the left sidebar.
Name the database: exploringSpace and the collection: users.
Copy the connection string from MongoDB Compass:

On the left sidebar in MongoDB Compass, click on localhost:27017 and copy the connection string.
Update index.js with the correct MongoDB connection string:

javascript
Copy code
"mongodb://localhost:27017/exploringSpace"
Step 4: Cloudinary Setup
Sign in to Cloudinary and navigate to your folders.

Create a folder named avatars.

In your Cloudinary account, copy your Cloud Name, API Key, and API Secret.

Create a .env file in the api folder with the following content:

bash
Copy code
CLOUDINARY_NAME=<Your Cloud Name>
CLOUDINARY_API_KEY=<Your API Key>
CLOUDINARY_API_SECRET=<Your API Secret>
Step 5: Frontend Setup
In the client folder, update the package.json file:
json
Copy code
"proxy": "http://localhost:5000"
Step 6: Running the Application
Start the Backend (API): Open a terminal in the api folder and run:

bash
Copy code
nodemon
Start the Frontend (Client): Open a new terminal, navigate to the client folder, and run:

bash
Copy code
cd client
npm install
npm run start
The app should now be running locally:

Backend: http://localhost:5000
Frontend: http://localhost:3000
✨ Contributing
Feel free to fork the project, make improvements, and submit pull requests!
