# Real-Time Weather Application 🌤️

A modern weather dashboard that provides real-time weather updates for Indian metropolitan cities and custom locations, with configurable weather alerts.

## ✨ Key Features

- **Pre-configured Cities**: Automatic weather updates for Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad
- **Custom City Search**: Add and monitor any city of your choice
- **Comprehensive Weather Data**:
  - Current temperature (with unit conversion: °C/°F/K)
  - Feels like temperature
  - Wind speed
  - Humidity
  - Daily min/max temperature
  - 5-day forecast with weather icons
- **Smart Alerts System**:
  - Set custom temperature thresholds
  - Monitor specific weather conditions
  - Email notifications
  - 10-minute update frequency

## 📷 Screenshots

### Dashboard
![Dashboard](https://github.com/user-attachments/assets/537e942d-568e-4c5b-a9ce-04c9e6159962)

### Search City
![Search](https://github.com/user-attachments/assets/fbfc9e61-ae01-490f-af04-f575c0caa148)

### Manage Alerts
![Manage alerts](https://github.com/user-attachments/assets/8a25059d-dcf4-4e7c-bf10-d23b5e07c42c)

### Create Alerts
![Adding alerts](https://github.com/user-attachments/assets/6075d2c3-ab2f-4d3f-a037-9a593c0723a2)

### View Alerts
![Viewing alerts](https://github.com/user-attachments/assets/aede28f3-d770-4ad8-9655-0a0306f48191)

### Email Notifications
![mail](https://github.com/user-attachments/assets/efe3ec8e-aff6-457c-990c-9a6800c9739d)

## 🚀 Quick Start Guide

### Prerequisites
- Node.js
- PostgreSQL
- Docker (optional)

### Installation Steps

#### Option 1: Traditional Setup

1. **Clone the Repository**
```bash
git clone https://github.com/SvickyB/Real_Time_Weather_Application.git
cd Real_Time_Weather_Application
```

2. **Set Up Frontend**
```bash
cd frontend
npm install
npm start
```

3. **Set Up Backend**
```bash
cd ../backend
npm install
```

4. **Database Setup**
```sql
CREATE DATABASE weatherapp;
```
Tables will be created automatically on server start.

5. **Configure Environment Variables**
Replace `.env` file in the Root directory:
```env
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
```

6. **Start the Server**
```bash
node server.js
```

#### Option 2: Docker Setup

1. **Clone the Repository**
```bash
git clone https://github.com/SvickyB/Real_Time_Weather_Application.git
cd Real_Time_Weather_Application
```

2. **Configure Environment Variables**
Replace `.env` file in the root directory with the credentials as mentioned above.

3. **Database Setup**
```sql
CREATE DATABASE weatherapp;
```
Tables will be created automatically on server start.

4. **Run with Docker Compose**
```bash
docker-compose up --build
```

This will:
- Build and start the frontend container (accessible at http://localhost:3000)
- Build and start the backend container (accessible at http://localhost:5000)
- Start a PostgreSQL container with the configured database

To stop the containers:
```bash
docker-compose down
```

## 💡 How to Use

### Access the Dashboard
- Open http://localhost:3000 in your browser
- View real-time weather data for metropolitan cities

### Search Cities
- Use the search bar to find any city
- Click the search icon or press Enter

### Configure Alerts
1. Navigate to Alert Management
2. Set up alerts with:
   - City name
   - Temperature thresholds
   - Weather conditions
   - Email address for notifications

### Manage Alerts
- View active alerts
- Check triggered alerts
- Delete unwanted alerts

## 🛠️ Tech Stack

### Frontend
- React
- Tailwind CSS
- Axios

### Backend
- Node.js
- Express
- PostgreSQL
- Additional Tools:
  - Axios for API requests
  - Nodemailer for email alerts

## 📦 Dependencies

### Frontend
- React
- Tailwind CSS
- Axios

### Backend
- Express
- dotenv
- cors
- pg (PostgreSQL client)
- nodemailer

## 🎯 Design Choices

- **React**: Component-based architecture for maintainable UI
- **Tailwind CSS**: Rapid styling and customization
- **Express**: Efficient REST API handling
- **PostgreSQL**: Reliable data storage
- **Nodemailer**: Robust email notification system

## 🔄 Update Frequencies

- Metropolitan cities: Every 5 minutes
- Alert checks: Every 10 minutes

## 🐳 Docker Configuration

The project includes three main Docker configurations:

1. `frontend/Dockerfile`: Builds the React frontend application
2. `backend/Dockerfile`: Builds the Node.js backend server
3. `docker-compose.yml`: Orchestrates all services including PostgreSQL

To modify container configurations, you can adjust the following files:
- `docker-compose.yml`: Service definitions and container linking
- Individual Dockerfiles: Build processes for each service
- `.env`: Environment variables for all services

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
