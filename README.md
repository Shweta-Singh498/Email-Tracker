# Email Tracker

A comprehensive email tracking system that allows you to send emails with tracking capabilities and monitor engagement metrics.

## Features

- **Email Tracking**: Track email opens, clicks, and engagement
- **Dashboard**: Real-time analytics and reporting
- **User Management**: Multi-user support with role-based access
- **Email Templates**: Pre-built templates for common use cases
- **API Integration**: RESTful API for external integrations
- **Real-time Notifications**: Instant alerts for email events

## Tech Stack

- **Frontend**: React.js with TypeScript
- **Backend**: Node.js with Express
- **Database**: PostgreSQL
- **Email Service**: Nodemailer
- **Authentication**: JWT
- **Real-time**: Socket.io
- **Styling**: Tailwind CSS

## Project Structure

```
email-tracker/
├── frontend/                 # React frontend application
├── backend/                  # Node.js backend API
├── database/                 # Database migrations and seeds
├── docs/                     # Documentation
└── docker/                   # Docker configuration
```

## Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd email-tracker
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   cd backend
   npm install
   
   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Set up environment variables**
   ```bash
   # Copy environment files
   cp backend/.env.example backend/.env
   cp frontend/.env.example frontend/.env
   ```

4. **Start the development servers**
   ```bash
   # Start backend (from backend directory)
   npm run dev
   
   # Start frontend (from frontend directory)
   npm start
   ```

## Environment Variables

### Backend (.env)
```
PORT=3001
DATABASE_URL=postgresql://username:password@localhost:5432/email_tracker
JWT_SECRET=your-jwt-secret
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@gmail.com
SMTP_PASS=your-app-password
```

### Frontend (.env)
```
REACT_APP_API_URL=http://localhost:3001/api
REACT_APP_SOCKET_URL=http://localhost:3001
```

## API Documentation

The API documentation is available at `/api/docs` when the backend server is running.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests
5. Submit a pull request

## License

MIT License 
