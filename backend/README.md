Doctor Appointment System
Table of Contents
Project Overview
Installation
Backend Setup
Frontend Setup
Running the Application
Assumptions & Design Decisions
API Endpoints
Deployed Links
Project Overview
The Doctor Appointment System allows users to book, view, edit, and cancel doctor appointments. It features an intuitive UI for managing appointments efficiently.

Installation
Backend Setup
Clone the repository:
git clone https://github.com/neeru0713/babyStepsAssignment.git
cd babyStepsAssignment/backend
Install dependencies:
npm install
Set up environment variables:
Create a .env file in the backend directory and add:
PORT=8080
MONGODB_URL=your_mongodb_connection_string
Start the backend server:
npm start
The backend will run at http://localhost:8080.
Frontend Setup
Navigate to the frontend directory in a new terminal:
cd ../frontend
Install dependencies:
npm install
Start the React app:
npm run dev
The frontend will run at http://localhost:5173.
Running the Application
Start the backend (npm start in backend directory).
Start the frontend (npm run dev in frontend directory).
Open http://localhost:5173 in the browser to use the application.
Assumptions & Design Decisions
Authentication: No Authentication is implemented as per the project scope.
Date & Time Handling: Appointments are stored in UTC format and converted to the user's local timezone on the frontend.
State Management: Redux is used to manage application state.
Styling: Tailwind CSS is used for a responsive UI.
API Calls: Axios is used for making HTTP requests.
Error Handling: Backend and frontend have error-handling mechanisms to handle API failures and validation errors gracefully.
API Endpoints
Appointments
POST /api/appointments - Book an appointment
GET /api/appointments - Get all appointments
PUT /api/appointments/:id - Update an appointment
DELETE /api/appointments/:id - Cancel an appointment
Doctors
GET /api/doctors - Get list of available doctors
GET /api/doctors/:id - Get doctor details
GET /doctors/:id/slots?date=YYYY-MM-DD - Get slots for doctor
Deployed Links
Frontend: Live Application
Backend: API Server
Screenshot 2025-02-21 at 2 50 04 PM Screenshot 2025-02-21 at 2 50 24 PM Screenshot 2025-02-21 at 2 49 44 PM
