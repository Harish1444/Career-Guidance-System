# Career Guidance Platform

A full-stack web application that helps users discover their ideal career path through scientific assessments, personalized recommendations, and interactive roadmaps.

## Features

- **User Authentication:** Secure signup and login with JWT-based authentication.
- **Dashboard:** Central hub for users to access all features and track their progress.
- **Psychometric Test:** Scientifically designed test to assess personality traits and preferences.
- **Intelligence Assessment:** Multiple intelligence test to identify users' strengths.
- **Career Matches:** Personalized career recommendations based on assessment results.
- **Career Roadmap:** Step-by-step roadmap for chosen careers, including milestones and resources.
- **Responsive UI:** Modern, mobile-friendly interface using Bootstrap and custom CSS.

## Technologies Used

- **Frontend:**
  - HTML5, CSS3 (custom + Bootstrap 5)
  - JavaScript (client-side logic)
- **Backend:**
  - Node.js with Express.js
  - MySQL (for user and assessment data)
  - JWT for authentication
  - bcryptjs for password hashing
- **Other:**
  - dotenv for environment variables
  - CORS for cross-origin requests

## Project Structure

```
Career Project/
├── css/
│   └── style.css           # Custom styles
├── index.html              # Landing page (auth, intro)
├── dashboard.html          # User dashboard
├── psychometric.html       # Psychometric test UI
├── intelligence.html       # Intelligence test UI
├── careers.html            # Career matches/results
├── roadmap.html            # Career roadmap
├── server.js               # Express backend server
├── package.json            # Node.js dependencies and scripts
```

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd "Career Project"
   ```
2. **Install backend dependencies:**
   ```bash
   npm install
   ```
3. **Configure environment variables:**
   - Create a `.env` file in the root directory with your MySQL credentials and JWT secret:
     ```env
     DB_HOST=localhost
     DB_USER=your_mysql_user
     DB_PASSWORD=your_mysql_password
     DB_NAME=career_guidance
     JWT_SECRET=your_jwt_secret_key
     PORT=3000
     ```
4. **Set up the MySQL database:**
   - Create a database named `career_guidance` and a `users` table as required by the backend.
5. **Run the backend server:**
   ```bash
   npm start
   ```
6. **Open the app:**
   - Open `index.html` in your browser, or serve the static files using the backend (`http://localhost:3000`).

## Usage

- Register a new account or log in.
- Take the psychometric and intelligence tests.
- View your personalized career matches and roadmap.
- Track your progress on the dashboard.

## Screenshots

_Add screenshots of the main pages here (dashboard, tests, results, roadmap, etc.)_

## License

MIT
