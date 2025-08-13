# Alumni Mentorship System Backend

The **Alumni Mentorship System** backend is a REST API that facilitates mentorship relationships for career development among alumni.  
It allows users to connect as mentors and mentees, manage tasks, track mentorship durations, and monitor progress.

## 🚀 Key Features

- User registration and login
- Profile creation, viewing, and editing
- Creation and management of mentorship relationships
- Task creation and tracking within mentorships
- Admin role assignment and management
- Task commenting functionality
- Overview of mentorship statistics

## 🐳 How to Run with Docker

1. Create a `.env` file in the project root with the required environment variables (see `.env.template` for reference).

2. **Build the Docker image:**
docker build -t alumni-mentorship-backend:latest .


3. **Run the Docker container** (expose port 5000):
docker run --env-file .env --env FLASK_APP=run.py -p 5000:5000 alumni-mentorship-backend:latest


4. Open your browser and go to:
http://localhost:5000


## 💻 How to Run Locally (Without Docker)

1. **Create and activate a virtual environment:**
virtualenv venv --python=python3
source ./venv/Scripts/activate # Windows PowerShell

or for Linux/macOS
source venv/bin/activate


2. **Install dependencies:**
pip install -r requirements.txt


3. **Set up environment variables:**
- Create a `.env` file from `.env.template`
- Fill in required values

4. **Start the application:**
python run.py


5. Visit:
http://localhost:5000
