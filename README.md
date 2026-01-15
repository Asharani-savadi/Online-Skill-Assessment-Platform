
# Online Skill Assessment Platform

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js Version](https://img.shields.io/badge/node-%3E%3D14.0.0-brightgreen)](https://nodejs.org/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()
[![Contributors](https://img.shields.io/badge/Contributors-Welcome-blue.svg)]()

A comprehensive, scalable web-based platform designed to assess and evaluate professional and technical skills through interactive tests, quizzes, practical coding challenges, and performance analytics.

[Live Demo](#) • [Documentation](./docs) • [Report Bug](#contact) • [Request Feature](#contact)

</div>

---

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [API Documentation](#api-documentation)
- [Database Schema](#database-schema)
- [Deployment](#deployment)
- [Security](#security)
- [Performance](#performance)
- [Troubleshooting](#troubleshooting)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## ✨ Features

### Core Assessment Features
- **Multiple Assessment Types**
  - Multiple choice questions with single/multiple correct answers
  - Free-text and short answer questions
  - Coding challenges with automated evaluation
  - Practical project submissions with peer/instructor review
  - Drag-and-drop matching questions
  - Image/diagram-based questions

- **Intelligent Testing Engine**
  - Adaptive difficulty levels based on performance
  - Time-limited assessments with auto-submission
  - Question randomization and shuffling
  - Question banking and versioning
  - Custom scoring algorithms
  - Partial credit support

- **User Authentication & Management**
  - Secure JWT-based authentication
  - Role-based access control (Admin, Instructor, Student, Guest)
  - Social login integration (Google, GitHub, LinkedIn)
  - User profile management with avatars
  - Account security with 2FA support

### Analytics & Reporting
- **Real-time Feedback**
  - Instant score calculation and breakdown
  - Detailed performance analytics with visual charts
  - Progress tracking across multiple assessments
  - Comparative analysis (peer benchmarking)
  - Learning path recommendations

- **Admin Analytics Dashboard**
  - Comprehensive student performance reports
  - Assessment difficulty analysis
  - Question effectiveness metrics
  - Custom report generation
  - Export to PDF/Excel

### Instructor Features
- **Assessment Creation Suite**
  - WYSIWYG question builder
  - Rich text editor with LaTeX support
  - Question import from CSV/JSON
  - Question tagging and categorization
  - Question preview and testing

- **Class Management**
  - Student grouping and sections
  - Batch assessment assignments
  - Deadline management
  - Plagiarism detection
  - Grading and feedback tools

### Student Features
- **Learning Portal**
  - Personalized dashboard
  - Assessment recommendations
  - Skill progress visualization
  - Certificate generation
  - Learning resource library

## 🛠 Tech Stack

### Frontend
- **Framework**: React.js / Vue.js / Angular (v16+)
- **Styling**: Tailwind CSS / Material-UI / Bootstrap
- **State Management**: Redux Toolkit / Zustand / Pinia
- **Testing**: Jest / Vitest / Cypress
- **Build Tool**: Vite / Webpack
- **Package Manager**: npm / yarn / pnpm

### Backend
- **Runtime**: Node.js v14+
- **Framework**: Express.js / NestJS / Fastify
- **Language**: TypeScript (recommended)
- **Database**: PostgreSQL / MongoDB / MySQL
- **ORM**: Sequelize / TypeORM / Prisma
- **Authentication**: JWT / Passport.js / Auth0
- **API Documentation**: Swagger/OpenAPI

### Infrastructure & DevOps
- **Containerization**: Docker & Docker Compose
- **Orchestration**: Kubernetes (optional)
- **CI/CD**: GitHub Actions / GitLab CI / Jenkins
- **Version Control**: Git
- **Cloud Platform**: AWS / Azure / GCP / DigitalOcean
- **Monitoring**: Prometheus / Grafana / ELK Stack
- **Caching**: Redis
- **Message Queue**: RabbitMQ / Kafka

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v14.0 or higher) - [Download](https://nodejs.org/)
- **npm** (v6.0+) or **yarn** (v1.22+)
- **Git** (v2.0+) - [Download](https://git-scm.com/)
- **PostgreSQL** (v12+) or **MongoDB** (v4.4+)
- **Docker** (optional, for containerized setup)
- **VS Code** or preferred code editor

## 🚀 Installation

### Quick Start with Docker (Recommended)

```bash
git clone https://github.com/yourusername/Online-Skill-Assessment-Platform.git
cd Online-Skill-Assessment-Platform

# Build and run with Docker Compose
docker-compose up -d

# Application will be available at http://localhost:3000
```

### Manual Setup

#### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Online-Skill-Assessment-Platform.git
cd Online-Skill-Assessment-Platform
```

#### 2. Backend Setup

```bash
cd backend

# Install dependencies
npm install

# Copy environment configuration
cp .env.example .env

# Update .env with your settings (see Configuration section)
# nano .env

# Install database
npm run db:migrate
npm run db:seed  # Optional: populate with sample data

# Start backend server
npm run dev
# Server runs on http://localhost:5000
```

#### 3. Frontend Setup

```bash
cd ../frontend

# Install dependencies
npm install

# Copy environment configuration
cp .env.example .env

# Start frontend application
npm start
# Application runs on http://localhost:3000
```

## ⚙️ Configuration

### Backend Environment Variables (.env)

```env
# Server Configuration
NODE_ENV=development
PORT=5000
HOST=localhost

# Database Configuration
DB_TYPE=postgres
DB_HOST=localhost
DB_PORT=5432
DB_NAME=skill_assessment_db
DB_USER=postgres
DB_PASSWORD=your_password

# Authentication
JWT_SECRET=your_super_secret_jwt_key
JWT_EXPIRY=24h
REFRESH_TOKEN_SECRET=your_refresh_token_secret

# CORS Configuration
CORS_ORIGIN=http://localhost:3000

# Email Configuration
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your_email@gmail.com
SMTP_PASSWORD=your_password
SMTP_FROM=noreply@skillassessment.com

# Third-party Services
GOOGLE_CLIENT_ID=your_google_client_id
GITHUB_CLIENT_ID=your_github_client_id
GITHUB_CLIENT_SECRET=your_github_secret

# AWS S3 (for file uploads)
AWS_ACCESS_KEY_ID=your_aws_key
AWS_SECRET_ACCESS_KEY=your_aws_secret
AWS_REGION=us-east-1
AWS_BUCKET_NAME=skill-assessment-files

# Logging
LOG_LEVEL=info
LOG_FILE=logs/app.log
```

### Frontend Environment Variables (.env)

```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_ENVIRONMENT=development
REACT_APP_VERSION=1.0.0
REACT_APP_GOOGLE_CLIENT_ID=your_google_client_id
REACT_APP_GITHUB_CLIENT_ID=your_github_client_id
```

## 📖 Usage

### Running the Application

**Development Mode:**
```bash
# Backend
cd backend
npm run dev

# Frontend (in another terminal)
cd frontend
npm start
```

**Production Mode:**
```bash
# Backend
npm run build
npm start

# Frontend
npm run build
npm run serve
```

### Creating Your First Assessment

1. **Log in as Instructor/Admin**
   - Navigate to `http://localhost:3000`
   - Click "Login" and use instructor credentials

2. **Create Assessment**
   - Go to "Assessments" → "Create New"
   - Fill in basic details (title, description, duration)
   - Set assessment type and difficulty level

3. **Add Questions**
   - Click "Add Question"
   - Choose question type
   - Enter question text, options, and correct answer
   - Set points and difficulty level
   - Repeat for all questions

4. **Configure Settings**
   - Set time limits
   - Enable/disable review after submission
   - Configure passing score
   - Set randomization options

5. **Publish Assessment**
   - Click "Publish" to make it available
   - Select target audience (classes/groups)
   - Set availability dates

### Taking an Assessment (Student Perspective)

1. **Browse Assessments**
   - Log in as Student
   - Go to "Available Assessments"
   - Filter by category, difficulty, or skill

2. **Start Assessment**
   - Click on assessment
   - Review instructions and rules
   - Click "Start Now"

3. **Complete Assessment**
   - Answer questions one by one
   - Use "Review" to check your answers
   - Submit when ready (cannot be undone)

4. **View Results**
   - See score breakdown immediately
   - Review correct answers and explanations
   - Download certificate if applicable

## 📁 Project Structure

```
Online-Skill-Assessment-Platform/
│
├── backend/
│   ├── src/
│   │   ├── controllers/          # Route controllers
│   │   ├── services/             # Business logic
│   │   ├── models/               # Database models/schemas
│   │   ├── routes/               # API routes
│   │   ├── middleware/           # Custom middleware
│   │   ├── validators/           # Input validation
│   │   ├── utils/                # Utility functions
│   │   ├── config/               # Configuration files
│   │   └── app.js                # Express app setup
│   ├── migrations/               # Database migrations
│   ├── seeds/                    # Seed data
│   ├── tests/                    # Unit and integration tests
│   ├── .env.example
│   ├── docker-compose.yml
│   ├── Dockerfile
│   ├── package.json
│   └── README.md
│
├── frontend/
│   ├── public/
│   │   ├── index.html
│   │   └── favicon.ico
│   ├── src/
│   │   ├── components/           # Reusable React components
│   │   ├── pages/                # Page components
│   │   ├── services/             # API client services
│   │   ├── hooks/                # Custom React hooks
│   │   ├── context/              # React context for state
│   │   ├── utils/                # Helper functions
│   │   ├── styles/               # Global styles
│   │   ├── assets/               # Images, fonts, etc.
│   │   ├── App.jsx
│   │   └── index.js
│   ├── tests/                    # Jest tests
│   ├── .env.example
│   ├── Dockerfile
│   ├── package.json
│   └── README.md
│
├── docs/
│   ├── API_DOCS.md               # Detailed API documentation
│   ├── DATABASE_SCHEMA.md        # Database schema details
│   ├── INSTALLATION.md           # Detailed installation guide
│   ├── DEPLOYMENT.md             # Deployment instructions
│   ├── ARCHITECTURE.md           # System architecture
│   └── CONTRIBUTING.md           # Contribution guidelines
│
├── docker-compose.yml            # Docker Compose configuration
├── .gitignore
├── LICENSE
├── README.md
└── CHANGELOG.md
```

## 📚 API Documentation

### Base URL
```
http://localhost:5000/api/v1
```

### Authentication Endpoints

#### Register User
```http
POST /auth/register
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securePassword123",
  "firstName": "John",
  "lastName": "Doe",
  "role": "student"
}
```

#### Login
```http
POST /auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securePassword123"
}

Response:
{
  "accessToken": "jwt_token_here",
  "refreshToken": "refresh_token_here",
  "user": { ... }
}
```

#### Get User Profile
```http
GET /auth/profile
Authorization: Bearer {accessToken}
```

### Assessment Endpoints

#### Get All Assessments
```http
GET /assessments?page=1&limit=10&category=coding
Authorization: Bearer {accessToken}
```

#### Get Assessment Details
```http
GET /assessments/:id
Authorization: Bearer {accessToken}
```

#### Create Assessment (Admin/Instructor only)
```http
POST /assessments
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "title": "JavaScript Fundamentals",
  "description": "Test your JavaScript knowledge",
  "duration": 60,
  "passingScore": 70,
  "category": "programming",
  "difficulty": "intermediate",
  "questions": [...]
}
```

#### Update Assessment
```http
PUT /assessments/:id
Authorization: Bearer {accessToken}
```

#### Delete Assessment
```http
DELETE /assessments/:id
Authorization: Bearer {accessToken}
```

### Questions Endpoints

#### Add Question to Assessment
```http
POST /assessments/:id/questions
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "type": "multiple_choice",
  "questionText": "What is JavaScript?",
  "options": ["Option 1", "Option 2"],
  "correctAnswer": 0,
  "points": 10
}
```

### Results Endpoints

#### Submit Assessment
```http
POST /assessments/:id/submit
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "answers": {
    "question_1": "answer_text",
    "question_2": 2
  }
}
```

#### Get User Results
```http
GET /results?assessmentId=:id
Authorization: Bearer {accessToken}
```

#### Get Result Details
```http
GET /results/:resultId
Authorization: Bearer {accessToken}
```

For complete API documentation with request/response examples, see [API_DOCS.md](./docs/API_DOCS.md)

## 🗄️ Database Schema

### Key Tables

- **users** - User accounts and profiles
- **assessments** - Assessment metadata
- **questions** - Questions with options
- **results** - Assessment submission results
- **answers** - Individual question answers
- **categories** - Assessment categories
- **skills** - Skill tags and mappings
- **classes** - Student groups/classes
- **enrollments** - Class enrollments

For detailed schema diagram and relationships, see [DATABASE_SCHEMA.md](./docs/DATABASE_SCHEMA.md)

## 🚀 Deployment

### Heroku Deployment
```bash
heroku create your-app-name
git push heroku main
heroku config:set DATABASE_URL=postgresql://...
```

### AWS EC2 Deployment
```bash
# Connect to instance
ssh -i key.pem ec2-user@your-instance

# Clone and setup
git clone <repo-url>
cd Online-Skill-Assessment-Platform
npm install

# Run with PM2
pm2 start backend/src/app.js --name "skill-api"
```

### Docker Deployment
```bash
docker-compose -f docker-compose.prod.yml up -d
```

For detailed deployment instructions, see [DEPLOYMENT.md](./docs/DEPLOYMENT.md)

## 🔒 Security

### Best Practices Implemented

- ✅ **JWT-based Authentication** - Secure token-based auth
- ✅ **Password Hashing** - bcrypt with salt rounds
- ✅ **HTTPS/TLS** - Encrypted data in transit
- ✅ **Input Validation** - XSS and SQL injection prevention
- ✅ **Rate Limiting** - DDoS protection
- ✅ **CORS Configuration** - Cross-origin request security
- ✅ **Environment Variables** - No hardcoded secrets
- ✅ **Database Encryption** - Sensitive data encrypted at rest

### Security Checklist
- [ ] Update all dependencies regularly
- [ ] Enable 2FA for admin accounts
- [ ] Set strong JWT secrets
- [ ] Configure HTTPS in production
- [ ] Use environment variables for secrets
- [ ] Regular security audits
- [ ] Implement API key rotation
- [ ] Enable database backups

## 📊 Performance

### Optimization Strategies

- **Caching**: Redis for session and query caching
- **Database**: Indexes on frequently queried columns
- **Frontend**: Code splitting and lazy loading
- **CDN**: Static assets served via CloudFront
- **Compression**: Gzip for API responses
- **Pagination**: Large datasets paginated

### Performance Metrics Target

- Page Load Time: < 2 seconds
- API Response Time: < 200ms
- Database Query Time: < 100ms
- Uptime: 99.9%

## 🐛 Troubleshooting

### Common Issues

**1. Database Connection Failed**
```
Error: ECONNREFUSED 127.0.0.1:5432

Solution:
- Ensure PostgreSQL is running
- Check DATABASE_URL in .env
- Verify database credentials
- Check port availability
```

**2. Port Already in Use**
```
Error: listen EADDRINUSE: address already in use :::5000

Solution:
Kill existing process:
lsof -ti:5000 | xargs kill -9
# or change PORT in .env
```

**3. CORS Errors**
```
Error: Access to XMLHttpRequest has been blocked by CORS policy

Solution:
- Update CORS_ORIGIN in backend .env
- Ensure frontend URL matches
- Check backend is running
```

**4. Module Not Found**
```
Error: Cannot find module 'express'

Solution:
rm -rf node_modules
npm install
```

## 🗺️ Roadmap

### Phase 1 (Current)
- [x] Core assessment platform
- [x] User authentication
- [x] Basic analytics
- [ ] Mobile app development

### Phase 2
- [ ] AI-powered question suggestions
- [ ] Proctored exam support
- [ ] Advanced plagiarism detection
- [ ] Learning path recommendations

### Phase 3
- [ ] Real-time collaboration features
- [ ] Gamification elements
- [ ] Integration with LMS (Canvas, Blackboard)
- [ ] Advanced reporting and insights

## 🤝 Contributing

We welcome contributions from the community! Please follow these steps:

### Getting Started

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Make your changes
4. Commit with descriptive messages
   ```bash
   git commit -m 'Add AmazingFeature: brief description'
   ```
5. Push to the branch
   ```bash
   git push origin feature/AmazingFeature
   ```
6. Open a Pull Request

### Code Standards

- **ESLint**: `npm run lint`
- **Prettier**: `npm run format`
- **Tests**: `npm test`
- **Coverage**: Aim for >80% coverage
- **Comments**: Document complex logic
- **Commits**: Follow conventional commits

### Pull Request Checklist

- [ ] Tests pass locally
- [ ] Code follows style guide
- [ ] Self-reviewed code
- [ ] Comments added for complex logic
- [ ] Documentation updated
- [ ] No breaking changes (or documented)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

- **Project Maintainer**: [Your Name]
- **Email**: your.email@example.com
- **GitHub**: [@yourusername](https://github.com/yourusername)
- **LinkedIn**: [Your Profile](https://linkedin.com/in/yourprofile)

### Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/Online-Skill-Assessment-Platform/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/Online-Skill-Assessment-Platform/discussions)
- **Email Support**: support@skillassessment.com

### Acknowledgments

- Thanks to all contributors and community members
- Special thanks to open-source libraries used in this project
- Inspired by modern EdTech platforms

---

<div align="center">

**[⬆ Back to Top](#online-skill-assessment-platform)**

**Last Updated**: January 15, 2026

Made with ❤️ by the Skill Assessment Team

</div>
