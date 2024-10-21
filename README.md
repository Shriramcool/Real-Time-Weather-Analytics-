# Real-Time Weather Analytics
### Assignment 2 - Software Engineer Intern - Zeotap

Introducing a dynamic **Real-Time Weather Analytics** system that leverages the **OpenWeatherMap API** to deliver current weather information for various cities across India. This platform not only captures and stores weather data but also includes essential data aggregation and alerts for extreme weather events. The user-friendly frontend is developed using **Vite + React**, while the robust backend is powered by **Node.js + Express.js**, ensuring optimal performance and responsiveness.

## Features

- Displays real-time weather information for selected Indian cities.
- Fetches data from the OpenWeatherMap API at configurable intervals.
- Uses SQLite (or MongoDB) to store weather data.
- Provides weather alerts when temperature thresholds are crossed.
- Visually appealing UI built with Tailwind CSS.

## Technologies Used

- **Frontend**: Vite, React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: SQLite (or MongoDB)
- **API**: OpenWeatherMap API

## Prerequisites

To run this project locally, ensure you have the following installed:

- Node.js (v14 or higher)
- npm (Node Package Manager)

## Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/zeotap-weather-app.git
cd Real-Time Weather Analytics
```

### 2. Set Up Environment Variables

Create a `.env` file in the `backend` directory and add the following content:

```bash
API_KEY=your_openweathermap_api_key
```

- Replace `your_openweathermap_api_key` with your actual API key from OpenWeatherMap.
- **Important**: The `.env` file should **not** be committed to version control. The project has a `.gitignore` to exclude it.

### 3. Install Dependencies

#### Backend

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

#### Frontend

Navigate to the frontend directory and install dependencies:

```bash
cd frontend
npm install
```

### 4. Run the Application

#### Running Backend

To start the backend server, which fetches data from the OpenWeatherMap API and stores it in the SQLite database, run the following command in the `backend` directory:

```bash
npm start
```

The backend server will be running at `http://localhost:5000`.

#### Running Frontend

To start the frontend development server, which displays the weather data, run the following command in the `frontend` directory:

```bash
npm run dev
```

The frontend app will be running at `http://localhost:5173`.

### 5. Viewing the Application

1. Open your browser and navigate to `http://localhost:5173` to view the weather data.
2. You can visit `http://localhost:5000/api/weather` to see the raw API data being fetched by the backend.

### 6. Database

The project utilizes SQLite for storing weather data, with the database file automatically created in the `backend` directory upon running the project. For those who prefer, it can easily be switched to MongoDB by updating the backend configuration.

## Future Enhancements

- **Enhance Weather Data**: Expand the system to include additional weather metrics such as humidity, wind speed, atmospheric pressure, and visibility for a more comprehensive view of current conditions.

- **Implement Weather Forecasting**: Integrate OpenWeatherMap's forecast API to provide users with accurate weather predictions, enabling them to plan ahead based on expected conditions.

- **Historical Weather Data Analysis**: Extend the system to store and analyze historical weather data trends, allowing users to identify patterns and make informed decisions based on past weather behavior.


