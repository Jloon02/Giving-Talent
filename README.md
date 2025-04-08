# Giving Talents - Client Platform

<img src="https://givingtalents.org/wp-content/uploads/2023/05/giving-talents_final-logo_vertical-purple-to-orange-gradient-on-text.png" alt="drawing" width="100"/>

Learn more at [givingtalents.org](https://givingtalents.org/)

## Overview

This Project is a client-server application platform designed for the non-profit organization "Giving Talents." This platform enables users to sign up, manage their profiles, and facilitates volunteer coordination through various features including location tracking and notifications.

## Features

- **User Management**: Secure sign-up and profile management system
- **Volunteer Data Collection**: Internal forms to record volunteer information in PostgreSQL database
- **Real-time Notifications**: Integration with Twilio for phone notifications
- **Location Tracking**: Mapbox API integration to track volunteers' whereabouts
- **Responsive UI**: Modern interface built with Tailwind CSS
- **Full-stack Typescript**: React frontend with TypeScript
- **Robust Backend**: Golang server with GORM for database operations

## Technology Stack

### Frontend
- Design: givingtalents.wordpress.com
- React (TypeScript)
- Tailwind CSS

### Backend
- Golang
- Mapbox API
- GORM (Go ORM)

### Infrastructure
- Google Cloud Platform (GCP) for hosting
- Docker for containerization
- PostgreSQL database (hosted on GCP)
- Neon (for database operations)

### Additional Services
- Twilio for notifications

## Installation

### Prerequisites
- Node.js (v14 or higher)
- Go (v1.16 or higher)
- Docker
- PostgreSQL
- GCP account (for deployment)

### Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/Jloon02/Giving-Talent.git
    ```
2. Frontend Setup:
    ```bash
    npm install
    npm start
    ```
3. Backend Setup:
    ```bash
    cd server/
    go mod download
    go run main.go
    ```
4. Database Setup:
- Ensure PostgreSQL is running
- Update database credentials in the configuration files

5. Environment Variables:
Create a `.env` file in both client and server directories with necessary variables (Twilio credentials, database URL, etc.)

## Deployment

The application is designed to be deployed on Google Cloud Platform:

1. Build Docker images:
```bash
docker build -t server .
```

2. Push to GCP Container Registry

3. Deploy using Google Kubernetes Engine or Cloud Run

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

[MIT License](LICENSE)

## Contact

For questions or support, please contact:
- GitHub: [@Jloon02](https://github.com/Jloon02)

