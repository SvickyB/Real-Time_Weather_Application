Real-Time Weather Application 🌤️
A modern weather dashboard that provides real-time weather updates for Indian metropolitan cities and custom locations, with configurable weather alerts.

✨ Key Features
Pre-configured Cities: Automatic weather updates for Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad
Custom City Search: Add and monitor any city of your choice
Comprehensive Weather Data:
Current temperature (with unit conversion: °C/°F/K)
Feels like temperature
Wind speed
Humidity
Daily min/max temperature
5-day forecast with weather icons
Smart Alerts System:
Set custom temperature thresholds
Monitor specific weather conditions
Email notifications
10-minute update frequency
📷 Screenshots
Dashboard
![Dashboard](https://github.com/user-attachments/assets/537e942d-568e-4c5b-a9ce-04c9e6159962)

Search City
![Search](https://github.com/user-attachments/assets/fbfc9e61-ae01-490f-af04-f575c0caa148)

Manage Alerts
![Manage alerts](https://github.com/user-attachments/assets/8a25059d-dcf4-4e7c-bf10-d23b5e07c42c)

Create Alerts
![Adding alerts](https://github.com/user-attachments/assets/6075d2c3-ab2f-4d3f-a037-9a593c0723a2)

View Alerts
![Viewing alerts](https://github.com/user-attachments/assets/aede28f3-d770-4ad8-9655-0a0306f48191)


Email Notifications
![mail](https://github.com/user-attachments/assets/efe3ec8e-aff6-457c-990c-9a6800c9739d)


🚀 Quick Start Guide
Prerequisites
Node.js
PostgreSQL
Docker (optional)
Installation Steps
Clone the Repository

bash
Copy code
git clone https://github.com/SvickyB/Real_Time_Weather_Application.git
Set Up Frontend

bash
Copy code
cd frontend
npm install
npm start
Set Up Backend

bash
Copy code
cd ../backend
npm install
Database Setup

Create a PostgreSQL database:
sql
Copy code
CREATE DATABASE weatherapp;
Tables will be created automatically on server start
Configure Environment Variables Create a .env file in the backend folder:

env
Copy code
# Database
DB_USER=your_username
DB_HOST=your_host
DB_NAME=your_db_name
DB_PASSWORD=your_password
DB_PORT=5432

# API
WEATHER_API_KEY=your_openweathermap_key

# Server
PORT=5000

# Email
EMAIL_USER=your_email
EMAIL_PASS=your_app_password
Start the Server

bash
Copy code
node server.js
💡 How to Use
Access the Dashboard

Open http://localhost:3000 in your browser
View real-time weather data for metropolitan cities
Search Cities

Use the search bar to find any city
Click the search icon or press Enter
Configure Alerts

Navigate to Alert Management
Set up alerts with:
City name
Temperature thresholds
Weather conditions
Email address for notifications
Manage Alerts

View active alerts
Check triggered alerts
Delete unwanted alerts
🛠️ Tech Stack
Frontend: React, Tailwind CSS
Backend: Node.js, Express
Database: PostgreSQL
Additional Tools:
Axios for API requests
Nodemailer for email alerts
📦 Dependencies
Frontend
React
Tailwind CSS
Axios
Backend
Express
dotenv
cors
pg (PostgreSQL client)
nodemailer
🎯 Design Choices
React: Component-based architecture for maintainable UI
Tailwind CSS: Rapid styling and customization
Express: Efficient REST API handling
PostgreSQL: Reliable data storage
Nodemailer: Robust email notification system
🔄 Update Frequencies
Metropolitan cities: Every 5 minutes
Alert checks: Every 10 minutes
