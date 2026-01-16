# 🎯 Online Skill Assessment Platform

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js Version](https://img.shields.io/badge/node-%3E%3D14.0.0-brightgreen)](https://nodejs.org/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()
[![Contributors](https://img.shields.io/badge/Contributors-Welcome-blue.svg)]()
[![React](https://img.shields.io/badge/React-v18+-61DAFB?logo=react)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-v5+-3178C6?logo=typescript)](https://www.typescriptlang.org/)

**A comprehensive, enterprise-grade platform for assessing and evaluating professional and technical skills**

Transform how you evaluate talent with interactive tests, quizzes, coding challenges, and real-time analytics.

[🚀 Quick Start](#-installation) • [📚 Documentation](./docs) • [🐛 Report Issue](#-contact) • [✨ Request Feature](#-contact)

</div>

---

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🛠 Tech Stack](#-tech-stack)
- [📋 Prerequisites](#-prerequisites)
- [🚀 Installation](#-installation)
- [⚙️ Configuration](#-configuration)
- [📖 Usage](#-usage)
- [📁 Project Structure](#-project-structure)
- [📚 API Documentation](#-api-documentation)
- [🗄️ Database Schema](#-database-schema)
- [🚀 Deployment](#-deployment)
- [🔒 Security](#-security)
- [📊 Performance](#-performance)
- [🐛 Troubleshooting](#-troubleshooting)
- [🗺️ Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [📞 Contact](#-contact)
- [⭐ Quick Links](#-quick-links)

## ✨ Features

### 🎓 Core Assessment Features
- **Multiple Assessment Types**
  - Multiple choice questions with single/multiple correct answers
  - Free-text and short answer questions with AI-powered grading
  - Coding challenges with automated evaluation and test cases
  - Practical project submissions with peer/instructor review
  - Drag-and-drop matching questions
  - Image/diagram-based questions with hotspot detection

- **Intelligent Testing Engine**
  - Adaptive difficulty levels based on real-time performance
  - Time-limited assessments with auto-submission and warnings
  - Advanced question randomization and shuffling
  - Question banking with versioning and A/B testing
  - Custom scoring algorithms and weighted scoring
  - Partial credit support with flexible grading
  - Question explanations and learning materials

- **User Authentication & Management**
  - Secure JWT-based authentication with refresh tokens
  - Comprehensive role-based access control (Admin, Instructor, Student, Guest, Evaluator)
  - Multi-provider social login (Google, GitHub, LinkedIn, Microsoft)
  - Rich user profiles with avatars and achievements
  - Advanced account security with 2FA/MFA support
  - SSO integration for enterprise

### 📊 Analytics & Reporting
- **Real-time Feedback**
  - Instant score calculation with detailed breakdown
  - Interactive performance analytics with dynamic charts
  - Comprehensive progress tracking across multiple assessments
  - Comparative analysis with peer benchmarking
  - Intelligent learning path recommendations
  - Skill gap analysis and improvement suggestions

- **Admin Analytics Dashboard**
  - Comprehensive student performance reports with trends
  - Assessment difficulty and discrimination analysis
  - Question effectiveness metrics and item analysis
  - Custom report generation with filters
  - Batch export to PDF/Excel/CSV
  - Scheduled reporting and automated alerts

### 👨‍🏫 Instructor Features
- **Assessment Creation Suite**
  - WYSIWYG question builder with live preview
  - Advanced rich text editor with LaTeX and markdown support
  - Bulk question import from CSV/JSON/Excel
  - Intelligent question tagging and categorization
  - Question versioning and change history
  - Template library for quick assessment creation

- **Class Management**
  - Flexible student grouping and section management
  - Batch assessment assignments with scheduling
  - Deadline management with automatic reminders
  - Advanced plagiarism detection using ML
  - Intuitive grading and detailed feedback tools
  - Mass communication with students

### 👨‍💻 Student Features
- **Personalized Learning Portal**
  - Customizable dashboard with skill recommendations
  - Smart assessment recommendations based on learning path
  - Interactive skill progress visualization with milestones
  - Automated certificate generation and sharing
  - Achievement badges and leaderboards
  - Learning resource library with curated content

## 🛠 Tech Stack

### Frontend
- **Framework**: React.js / Vue.js / Angular (v16+)
- **Styling**: Tailwind CSS / Material-UI / Bootstrap 5
- **State Management**: Redux Toolkit / Zustand / Pinia
- **Testing**: Jest / Vitest / Cypress / Playwright
- **Build Tool**: Vite / Webpack 5
- **Package Manager**: npm / yarn / pnpm
- **UI Components**: Shadcn/ui, Radix UI, Headless UI
- **Charts**: Chart.js, Recharts, D3.js
- **Forms**: React Hook Form, Formik

### Backend
- **Runtime**: Node.js v14+ (v18+ recommended)
- **Framework**: Express.js / NestJS / Fastify
- **Language**: TypeScript (recommended)
- **Database**: PostgreSQL (primary) / MongoDB / MySQL
- **ORM**: TypeORM / Prisma / Sequelize
- **Authentication**: Passport.js / Auth0 / JWT
- **Validation**: Joi / Yup / Zod
- **API Documentation**: Swagger/OpenAPI / GraphQL
- **Email**: Nodemailer / SendGrid
- **File Storage**: AWS S3 / Azure Blob / MinIO

### Infrastructure & DevOps
- **Containerization**: Docker & Docker Compose
- **Orchestration**: Kubernetes (K8s) / Docker Swarm
- **CI/CD**: GitHub Actions / GitLab CI / Jenkins / CircleCI
- **Version Control**: Git / GitHub / GitLab
- **Cloud Platform**: AWS / Azure / GCP / DigitalOcean / Linode
- **Monitoring**: Prometheus / Grafana / DataDog / New Relic
- **Logging**: ELK Stack / Loki / Sumo Logic
- **Caching**: Redis / Memcached
- **Message Queue**: RabbitMQ / Apache Kafka / AWS SQS
- **Load Balancing**: Nginx / HAProxy / AWS ALB

## 📋 Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Node.js** (v16.0 or higher, v18+ recommended) - [Download](https://nodejs.org/)
- **npm** (v8.0+), **yarn** (v1.22+), or **pnpm** (v7+)
- **Git** (v2.20+) - [Download](https://git-scm.com/)
- **PostgreSQL** (v13+) or **MongoDB** (v5.0+) - [Download](https://www.postgresql.org/)
- **Docker & Docker Compose** (optional, for containerized setup) - [Download](https://www.docker.com/)
- **Code Editor**: VS Code, WebStorm, Sublime Text, or preferred IDE
- **Terminal/Shell**: Bash, Zsh, or PowerShell

### System Requirements
- **RAM**: Minimum 4GB (8GB+ recommended)
- **Storage**: 2GB free space
- **OS**: Windows 10+, macOS 10.14+, or Linux (Ubuntu 18.04+)
- **Network**: Internet connection required for initial setup

## 🚀 Installation

### 🐳 Quick Start with Docker (Recommended)

The fastest way to get up and running:

```bash
# Clone the repository
git clone https://github.com/yourusername/Online-Skill-Assessment-Platform.git
cd Online-Skill-Assessment-Platform

# Build and start all services
docker-compose up -d

# Check service status
docker-compose ps

# View logs
docker-compose logs -f

# Application will be available at:
# Frontend: http://localhost:3000
# Backend API: http://localhost:5000
# Database: localhost:5432
```

**Useful Docker Commands:**
```bash
# Stop services
docker-compose down

# Rebuild images
docker-compose up -d --build

# Execute command in container
docker-compose exec backend npm run db:seed

# View database logs
docker-compose logs db
```

### 🔧 Manual Setup (Development)

For local development without Docker:

#### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Online-Skill-Assessment-Platform.git
cd Online-Skill-Assessment-Platform
```

#### 2. Backend Setup

```bash
cd backend
instal
# Install dependencies
npm install
# or yarn install / pnpm install

# Copy and configure environment variables
cp .env.example .env

# Edit .env with your database and service credentials
nano .env  # macOS/Linux
# or use your editor on Windows

# Run database migrations
npm run db:migrate

# (Optional) Seed database with sample data
npm run db:seed

# Start development server (with hot reload)
npm run dev

# Backend will run on http://localhost:5000
```

#### 3. Frontend Setup (in another terminal)

```bash
# From project root
cd frontend

# Install dependencies
npm install

# Copy and configure environment variables
cp .env.example .env

# Edit .env if needed
nano .env

# Start development server
npm start

# Frontend will run on http://localhost:3000
```

### ✅ Verify Installation

Once everything is running, verify:

```bash
# Check backend API
curl http://localhost:5000/api/health

# Check frontend
curl http://localhost:3000

# Should return 200 OK and health status
```

## ⚙️ Configuration

### Backend Environment Variables (.env)

Create a `.env` file in the `backend/` directory with the following configuration:

```env
# ============================================================================
# SERVER CONFIGURATION
# ============================================================================
NODE_ENV=development           # development | production | staging
PORT=5000                      # API server port
HOST=localhost                 # Server hostname
APP_URL=http://localhost:5000  # Full application URL
API_PREFIX=/api/v1             # API route prefix

# ============================================================================
# DATABASE CONFIGURATION
# ============================================================================
DB_TYPE=postgres               # postgres | mongodb | mysql
DB_HOST=localhost              # Database hostname
DB_PORT=5432                   # PostgreSQL default: 5432, MySQL: 3306
DB_NAME=skill_assessment_db    # Database name
DB_USER=postgres               # Database user
DB_PASSWORD=your_password      # Database password
DB_SSL=false                   # Use SSL for database connection
DB_POOL_SIZE=10                # Connection pool size

# ============================================================================
# AUTHENTICATION & SECURITY
# ============================================================================
JWT_SECRET=your_super_secret_jwt_key_min_32_chars_recommended
JWT_EXPIRY=24h                 # Token expiration time
REFRESH_TOKEN_SECRET=your_refresh_token_secret_min_32_chars
REFRESH_TOKEN_EXPIRY=7d        # Refresh token expiration
SESSION_SECRET=your_session_secret

# CORS Configuration
CORS_ORIGIN=http://localhost:3000,http://localhost:3001
CORS_CREDENTIALS=true

# Rate Limiting
RATE_LIMIT_WINDOW=15           # Window in minutes
RATE_LIMIT_MAX_REQUESTS=100    # Max requests per window

# ============================================================================
# EMAIL CONFIGURATION
# ============================================================================
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_SECURE=false              # true for port 465, false for others
SMTP_USER=your_email@gmail.com
SMTP_PASSWORD=your_app_password
SMTP_FROM=noreply@skillassessment.com
SMTP_FROM_NAME=Skill Assessment Platform

# Alternative: SendGrid
SENDGRID_API_KEY=your_sendgrid_api_key

# ============================================================================
# SOCIAL LOGIN & OAUTH
# ============================================================================
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_REDIRECT_URI=http://localhost:5000/api/auth/google/callback

GITHUB_CLIENT_ID=your_github_client_id
GITHUB_CLIENT_SECRET=your_github_client_secret
GITHUB_REDIRECT_URI=http://localhost:5000/api/auth/github/callback

MICROSOFT_CLIENT_ID=your_microsoft_client_id
MICROSOFT_CLIENT_SECRET=your_microsoft_client_secret
MICROSOFT_REDIRECT_URI=http://localhost:5000/api/auth/microsoft/callback

# ============================================================================
# FILE STORAGE (AWS S3)
# ============================================================================
AWS_REGION=us-east-1
AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
AWS_S3_BUCKET_NAME=skill-assessment-files
AWS_S3_FOLDER=uploads          # Folder prefix in bucket

# Alternative: Local storage
FILE_UPLOAD_PATH=./uploads
MAX_FILE_SIZE=52428800         # 50MB in bytes

# ============================================================================
# CACHING & REDIS
# ============================================================================
REDIS_HOST=localhost
REDIS_PORT=6379
REDIS_PASSWORD=                # Leave empty if no password
REDIS_DB=0
REDIS_TTL=3600                 # Cache TTL in seconds

# ============================================================================
# LOGGING & MONITORING
# ============================================================================
LOG_LEVEL=info                 # error | warn | info | debug | trace
LOG_FORMAT=json                # json | text
LOG_FILE=logs/app.log
LOG_MAX_SIZE=10m               # Max log file size
LOG_MAX_FILES=14               # Max number of log files to keep

# Sentry (Error tracking)
SENTRY_DSN=your_sentry_dsn

# ============================================================================
# FEATURE FLAGS
# ============================================================================
ENABLE_SOCIAL_LOGIN=true
ENABLE_2FA=false
ENABLE_PLAGIARISM_CHECK=true
ENABLE_AI_GRADING=false
ENABLE_PROCTORING=false

# ============================================================================
# MISC
# ============================================================================
TIMEZONE=UTC
JWT_ISSUER=skill-assessment-platform
JWT_AUDIENCE=skill-assessment-web-app
```

### Frontend Environment Variables (.env)

Create a `.env` file in the `frontend/` directory:

```env
# ============================================================================
# API CONFIGURATION
# ============================================================================
REACT_APP_API_URL=http://localhost:5000/api/v1
REACT_APP_API_TIMEOUT=30000    # API timeout in milliseconds

# ============================================================================
# APPLICATION CONFIG
# ============================================================================
REACT_APP_ENVIRONMENT=development    # development | staging | production
REACT_APP_VERSION=1.0.0
REACT_APP_APP_NAME=Skill Assessment Platform

# ============================================================================
# SOCIAL LOGIN
# ============================================================================
REACT_APP_GOOGLE_CLIENT_ID=your_google_client_id
REACT_APP_GITHUB_CLIENT_ID=your_github_client_id
REACT_APP_GITHUB_REPO_URL=https://github.com/yourusername/Online-Skill-Assessment-Platform

# ============================================================================
# ANALYTICS & MONITORING
# ============================================================================
REACT_APP_GOOGLE_ANALYTICS_ID=your_ga_id
REACT_APP_SENTRY_DSN=your_sentry_dsn
REACT_APP_SENTRY_ENVIRONMENT=development

# ============================================================================
# FEATURE FLAGS
# ============================================================================
REACT_APP_ENABLE_DARK_MODE=true
REACT_APP_ENABLE_OFFLINE_MODE=false
```

### Running the Application

**Development Mode:**
```bash
# Terminal 1: Backend
cd backend
npm run dev

# Terminal 2: Frontend
cd frontend
npm start
```

**Production Mode:**
```bash
# Backend
cd backend
npm run build
npm start

# Frontend
cd frontend
npm run build
npm run serve
```

For detailed configuration options, see [CONFIGURATION.md](./docs/CONFIGURATION.md)

## 📖 Usage

### 🎬 Creating Your First Assessment

#### Step 1: Log in as Instructor/Admin
```
1. Navigate to http://localhost:3000
2. Click "Login" button
3. Use instructor credentials (or register as instructor)
4. You'll be redirected to the dashboard
```

#### Step 2: Create Assessment
```
1. Go to "Assessments" → "Create New"
2. Fill in basic details:
   - Title: "JavaScript Fundamentals Quiz"
   - Description: Detailed overview of the assessment
   - Category: Select "Programming"
   - Duration: 60 minutes
   - Difficulty Level: Intermediate
3. Click "Continue"
```

#### Step 3: Add Questions
```
1. Click "Add Question"
2. Choose question type from dropdown:
   - Multiple Choice
   - Short Answer
   - Code Challenge
   - Matching
   - Fill in the Blank
3. Fill in question details:
   - Question text (supports Markdown and LaTeX)
   - Options/choices
   - Mark correct answer(s)
   - Set point value
   - Set difficulty level
4. Click "Save Question"
5. Repeat for all questions
```

#### Step 4: Configure Settings
```
1. Go to "Assessment Settings"
2. Configure options:
   - Allow review after submission: Yes/No
   - Show correct answers: Yes/No
   - Show explanations: Yes/No
   - Set passing score: 70%
   - Allow retakes: How many times
   - Randomize questions: Yes/No
   - Randomize options: Yes/No
3. Click "Save Settings"
```

#### Step 5: Publish Assessment
```
1. Click "Publish" button
2. Select target audience:
   - All students
   - Specific class/section
   - By skill tags
3. Set availability:
   - Start date and time
   - End date and time
4. Configure notifications
5. Click "Publish Assessment"
```

### 👨‍🎓 Taking an Assessment (Student Perspective)

#### Step 1: Browse Available Assessments
```
1. Log in as Student
2. Go to "Assessments" tab
3. Filter/search by:
   - Category (Programming, Business, etc.)
   - Difficulty (Beginner, Intermediate, Advanced)
   - Skill tags
4. Click on assessment to view details
```

#### Step 2: Start Assessment
```
1. Click "Start Assessment" button
2. Review:
   - Instructions and rules
   - Time limit
   - Number of questions
   - Point value
3. Click "Start Now" (cannot be undone)
```

#### Step 3: Complete Assessment
```
1. Answer questions one by one
2. Use "Review" button to check answers
3. Progress bar shows completion status
4. Timer shows remaining time
5. Click "Submit" when ready
   (Warning: Cannot modify answers after submission)
```

#### Step 4: View Results
```
1. Receive score immediately
2. View detailed breakdown:
   - Score vs. passing score
   - Category-wise performance
   - Time spent
3. Review answers:
   - Your answer
   - Correct answer
   - Explanation/learning material
4. Download certificate (if applicable)
5. Share results on social media
```

### 📊 Available CLI Commands

**Backend Commands:**
```bash
# Development
npm run dev              # Start dev server with hot reload
npm run build           # Build for production
npm start               # Start production server

# Database
npm run db:migrate      # Run pending migrations
npm run db:migrate:undo # Undo last migration
npm run db:seed         # Seed database with sample data
npm run db:reset        # Drop all tables and reseed

# Testing
npm test                # Run unit tests
npm test:cov            # Run tests with coverage report
npm test:e2e            # Run end-to-end tests
npm run test:watch      # Watch mode for tests

# Code Quality
npm run lint            # Check code quality
npm run lint:fix        # Fix linting issues
npm run format          # Format code with Prettier
npm run type-check      # TypeScript type checking

# Documentation
npm run docs            # Generate API documentation
npm run docs:serve      # Serve documentation locally
```

**Frontend Commands:**
```bash
# Development
npm start               # Start dev server
npm run dev            # Alternative dev command
npm run build          # Build for production
npm run serve          # Serve production build locally

# Testing
npm test               # Run unit tests
npm test:watch        # Watch mode for tests
npm run test:cov      # Coverage report

# Code Quality
npm run lint           # ESLint checks
npm run lint:fix       # Fix lint issues
npm run format         # Prettier formatting
npm run type-check     # TypeScript checks

# Build
npm run build:analyze  # Analyze bundle size
npm run build:preview  # Preview production build
```

## 📁 Project Structure

```
Online-Skill-Assessment-Platform/
│
├── backend/                          # Express/NestJS backend API
│   ├── src/
│   │   ├── controllers/              # Route request handlers
│   │   ├── services/                 # Business logic layer
│   │   ├── models/                   # Database models/schemas (ORM entities)
│   │   ├── routes/                   # API route definitions
│   │   ├── middleware/               # Express middleware (auth, logging, etc.)
│   │   ├── validators/               # Input validation schemas
│   │   ├── utils/                    # Utility and helper functions
│   │   ├── config/                   # Configuration management
│   │   ├── constants/                # Application constants
│   │   ├── types/                    # TypeScript type definitions
│   │   └── app.ts                    # Express app initialization
│   ├── migrations/                   # Database migration files
│   ├── seeds/                        # Database seeding scripts
│   ├── tests/                        # Unit and integration tests
│   │   ├── unit/
│   │   ├── integration/
│   │   └── e2e/
│   ├── .env.example                  # Environment variables template
│   ├── docker-compose.yml
│   ├── Dockerfile
│   ├── tsconfig.json                 # TypeScript configuration
│   ├── jest.config.js                # Jest testing configuration
│   ├── package.json
│   └── README.md
│
├── frontend/                         # React/Vue frontend application
│   ├── public/
│   │   ├── index.html
│   │   ├── favicon.ico
│   │   └── manifest.json
│   ├── src/
│   │   ├── components/               # Reusable React components
│   │   │   ├── common/               # Shared components (Button, Modal, etc.)
│   │   │   ├── assessments/          # Assessment-related components
│   │   │   ├── dashboard/            # Dashboard components
│   │   │   └── layout/               # Layout components (Header, Sidebar)
│   │   ├── pages/                    # Page-level components
│   │   │   ├── AssessmentPage.jsx
│   │   │   ├── DashboardPage.jsx
│   │   │   ├── ResultsPage.jsx
│   │   │   └── NotFoundPage.jsx
│   │   ├── hooks/                    # Custom React hooks
│   │   │   ├── useAuth.js
│   │   │   ├── useFetch.js
│   │   │   └── useNotification.js
│   │   ├── context/                  # React context for global state
│   │   │   ├── AuthContext.jsx
│   │   │   └── ThemeContext.jsx
│   │   ├── services/                 # API client services
│   │   │   ├── api.js                # Axios instance
│   │   │   ├── assessmentService.js
│   │   │   └── authService.js
│   │   ├── store/                    # Redux/Zustand state management
│   │   │   ├── slices/
│   │   │   └── store.js
│   │   ├── utils/                    # Helper functions
│   │   │   ├── formatters.js
│   │   │   ├── validators.js
│   │   │   └── constants.js
│   │   ├── styles/                   # Global and component styles
│   │   │   ├── globals.css
│   │   │   └── variables.css
│   │   ├── assets/                   # Static assets
│   │   │   ├── images/
│   │   │   ├── icons/
│   │   │   └── fonts/
│   │   ├── types/                    # TypeScript type definitions
│   │   ├── App.jsx
│   │   └── index.js
│   ├── tests/                        # Jest and Cypress tests
│   │   ├── unit/
│   │   ├── integration/
│   │   └── e2e/
│   ├── .env.example
│   ├── Dockerfile
│   ├── tsconfig.json
│   ├── jest.config.js
│   ├── package.json
│   └── README.md
│
├── docs/                             # Documentation files
│   ├── API_DOCS.md                   # Detailed REST API documentation
│   ├── DATABASE_SCHEMA.md            # Database schema and relationships
│   ├── INSTALLATION.md               # Detailed setup guide
│   ├── DEPLOYMENT.md                 # Deployment to various platforms
│   ├── ARCHITECTURE.md               # System architecture and design
│   ├── CONFIGURATION.md              # Configuration guide
│   ├── CONTRIBUTING.md               # Contribution guidelines
│   ├── SECURITY.md                   # Security best practices
│   ├── TROUBLESHOOTING.md            # Common issues and solutions
│   └── API/
│       ├── authentication.md
│       ├── assessments.md
│       ├── questions.md
│       ├── results.md
│       └── users.md
│
├── docker-compose.yml                # Docker Compose configuration for all services
├── docker-compose.prod.yml           # Production Docker Compose config
├── .gitignore                        # Git ignore rules
├── .dockerignore                     # Docker ignore rules
├── .editorconfig                     # Editor configuration
├── .prettierrc                       # Code formatter configuration
├── .eslintrc                         # Linter configuration
├── LICENSE                           # MIT License
├── README.md                         # This file
└── CHANGELOG.md                      # Version history and changes
```

### Directory Structure Details

**Backend (`src/` directory):**
- `controllers/` - HTTP request handlers that receive requests, call services, and send responses
- `services/` - Business logic, validations, and database operations
- `models/` - Database schemas and ORM entity definitions
- `middleware/` - Custom middleware for authentication, logging, error handling
- `validators/` - Input validation using Joi, Yup, or Zod
- `utils/` - Reusable utility functions and helpers
- `config/` - Configuration management and environment setup

**Frontend (`src/` directory):**
- `components/` - Reusable UI components organized by feature
- `pages/` - Full page components (routes)
- `hooks/` - Custom React hooks for state and side effects
- `services/` - API communication layer (Axios, Fetch)
- `store/` - Global state management (Redux, Zustand)
- `utils/` - Helper functions and formatters
- `assets/` - Images, icons, and static files

## 📚 API Documentation

### Base URL
```
http://localhost:5000/api/v1
```

### API Standards
- **Format**: JSON
- **Authentication**: JWT Bearer Token
- **Rate Limiting**: 100 requests per 15 minutes
- **Versioning**: URL-based (/api/v1, /api/v2, etc.)

### Authentication Endpoints

#### Register User
```http
POST /auth/register
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securePassword123!",
  "firstName": "John",
  "lastName": "Doe",
  "role": "student"
}

Response: 201 Created
{
  "success": true,
  "message": "User registered successfully",
  "data": {
    "id": "user-uuid",
    "email": "user@example.com",
    "firstName": "John",
    "lastName": "Doe",
    "role": "student",
    "createdAt": "2026-01-15T10:30:00Z"
  }
}
```

#### Login
```http
POST /auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securePassword123!"
}

Response: 200 OK
{
  "success": true,
  "data": {
    "accessToken": "eyJhbGciOiJIUzI1NiIs...",
    "refreshToken": "eyJhbGciOiJIUzI1NiIs...",
    "user": {
      "id": "user-uuid",
      "email": "user@example.com",
      "firstName": "John",
      "lastName": "Doe",
      "role": "student",
      "avatar": "https://..."
    }
  }
}
```

#### Get User Profile
```http
GET /auth/profile
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "data": {
    "id": "user-uuid",
    "email": "user@example.com",
    "firstName": "John",
    "lastName": "Doe",
    "role": "student",
    "avatar": "https://...",
    "bio": "Software developer",
    "skills": ["JavaScript", "React", "Node.js"],
    "createdAt": "2026-01-01T08:00:00Z",
    "lastLogin": "2026-01-15T10:30:00Z"
  }
}
```

#### Refresh Access Token
```http
POST /auth/refresh
Content-Type: application/json

{
  "refreshToken": "eyJhbGciOiJIUzI1NiIs..."
}

Response: 200 OK
{
  "success": true,
  "data": {
    "accessToken": "eyJhbGciOiJIUzI1NiIs...",
    "refreshToken": "eyJhbGciOiJIUzI1NiIs..."
  }
}
```

#### Logout
```http
POST /auth/logout
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "message": "Logged out successfully"
}
```

### Assessment Endpoints

#### Get All Assessments
```http
GET /assessments?page=1&limit=10&category=coding&difficulty=intermediate
Authorization: Bearer {accessToken}

Query Parameters:
- page (integer): Page number (default: 1)
- limit (integer): Items per page (default: 10, max: 100)
- category (string): Filter by category
- difficulty (string): beginner | intermediate | advanced
- search (string): Search in title and description
- sortBy (string): title | createdAt | popularity
- sortOrder (string): asc | desc

Response: 200 OK
{
  "success": true,
  "data": {
    "items": [...],
    "pagination": {
      "page": 1,
      "limit": 10,
      "total": 45,
      "pages": 5
    }
  }
}
```

#### Get Assessment Details
```http
GET /assessments/:id
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "data": {
    "id": "assessment-uuid",
    "title": "JavaScript Fundamentals",
    "description": "Test your JavaScript knowledge",
    "category": "programming",
    "difficulty": "intermediate",
    "duration": 60,
    "passingScore": 70,
    "totalPoints": 100,
    "questionCount": 20,
    "createdBy": {...},
    "createdAt": "2026-01-10T09:00:00Z",
    "updatedAt": "2026-01-15T10:30:00Z",
    "questions": [...]
  }
}
```

#### Create Assessment (Admin/Instructor only)
```http
POST /assessments
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "title": "JavaScript Fundamentals",
  "description": "Test your JavaScript knowledge",
  "category": "programming",
  "difficulty": "intermediate",
  "duration": 60,
  "passingScore": 70,
  "totalPoints": 100,
  "instructions": "Answer all questions...",
  "isPublished": false,
  "allowReview": true,
  "showCorrectAnswers": true,
  "randomizeQuestions": true,
  "randomizeOptions": true
}

Response: 201 Created
{
  "success": true,
  "data": {
    "id": "assessment-uuid",
    ...
  }
}
```

#### Update Assessment
```http
PUT /assessments/:id
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "title": "Updated Title",
  "duration": 90,
  ...
}

Response: 200 OK
{
  "success": true,
  "data": {...}
}
```

#### Delete Assessment
```http
DELETE /assessments/:id
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "message": "Assessment deleted successfully"
}
```

#### Publish Assessment
```http
PATCH /assessments/:id/publish
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "targetAudience": ["class-1", "class-2"],
  "startDate": "2026-01-20T00:00:00Z",
  "endDate": "2026-02-20T23:59:59Z",
  "sendNotification": true
}

Response: 200 OK
{
  "success": true,
  "data": {...}
}
```

### Questions Endpoints

#### Add Question to Assessment
```http
POST /assessments/:assessmentId/questions
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "type": "multiple_choice",
  "questionText": "What is JavaScript?",
  "description": "Optional detailed explanation",
  "options": [
    { "text": "A programming language", "isCorrect": true },
    { "text": "A markup language", "isCorrect": false },
    { "text": "A database", "isCorrect": false }
  ],
  "points": 10,
  "difficulty": "easy",
  "tags": ["basics", "fundamentals"],
  "explanation": "JavaScript is a programming language..."
}

Response: 201 Created
{
  "success": true,
  "data": {...}
}
```

#### Get Questions
```http
GET /assessments/:assessmentId/questions
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "data": [...]
}
```

### Results & Submissions Endpoints

#### Submit Assessment
```http
POST /assessments/:assessmentId/submit
Authorization: Bearer {accessToken}
Content-Type: application/json

{
  "answers": {
    "question-uuid-1": "option-0",
    "question-uuid-2": "user-answer-text",
    "question-uuid-3": ["option-0", "option-2"]
  },
  "timeSpent": 2400
}

Response: 201 Created
{
  "success": true,
  "data": {
    "resultId": "result-uuid",
    "score": 85,
    "percentage": 85,
    "passed": true,
    "feedback": "Great job!",
    "details": [...]
  }
}
```

#### Get User Results
```http
GET /results?assessmentId=:id&page=1&limit=10
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "data": {
    "items": [...],
    "pagination": {...}
  }
}
```

#### Get Result Details
```http
GET /results/:resultId
Authorization: Bearer {accessToken}

Response: 200 OK
{
  "success": true,
  "data": {
    "id": "result-uuid",
    "assessmentId": "assessment-uuid",
    "userId": "user-uuid",
    "score": 85,
    "percentage": 85,
    "passed": true,
    "timeSpent": 2400,
    "submittedAt": "2026-01-15T11:00:00Z",
    "answers": [...]
  }
}
```

### Error Response Format
```json
{
  "success": false,
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "Invalid input provided",
    "details": [
      {
        "field": "email",
        "message": "Must be a valid email"
      }
    ]
  }
}
```

### Common HTTP Status Codes
- `200 OK` - Request succeeded
- `201 Created` - Resource created successfully
- `204 No Content` - Request succeeded with no response body
- `400 Bad Request` - Invalid request or validation error
- `401 Unauthorized` - Authentication required
- `403 Forbidden` - Insufficient permissions
- `404 Not Found` - Resource not found
- `409 Conflict` - Resource conflict
- `429 Too Many Requests` - Rate limit exceeded
- `500 Internal Server Error` - Server error

For complete API documentation with more endpoints, examples, and webhooks, see [API_DOCS.md](./docs/API_DOCS.md)

## 🗄️ Database Schema

### Entity Relationship Diagram

The platform uses a relational database structure with the following key entities:

```
Users (1) ──→ (many) Assessments (created_by)
Users (1) ──→ (many) Results (submitted_by)
Assessments (1) ──→ (many) Questions
Assessments (1) ──→ (many) Results (assessment_id)
Questions (1) ──→ (many) Answers (question_id)
Results (1) ──→ (many) Answers (result_id)
Users (many) ──→ (many) Classes (through Enrollments)
Assessments (many) ──→ (many) Classes (through Assignments)
```

### Key Tables

#### Users
- `id` (UUID): Primary key
- `email` (String, Unique): User email
- `password` (String): Hashed password
- `firstName` (String): First name
- `lastName` (String): Last name
- `role` (Enum): admin | instructor | student | evaluator | guest
- `avatar` (String): Avatar URL
- `bio` (String): User biography
- `isActive` (Boolean): Account status
- `emailVerified` (Boolean): Email verification status
- `lastLogin` (DateTime): Last login timestamp
- `createdAt` (DateTime): Creation timestamp
- `updatedAt` (DateTime): Last update timestamp

#### Assessments
- `id` (UUID): Primary key
- `title` (String): Assessment title
- `description` (Text): Detailed description
- `category` (String): Category/subject
- `difficulty` (Enum): beginner | intermediate | advanced
- `duration` (Integer): Duration in minutes
- `passingScore` (Integer): Minimum passing percentage
- `totalPoints` (Integer): Total points for assessment
- `instructions` (Text): Assessment instructions
- `createdBy` (UUID, FK): User who created
- `isPublished` (Boolean): Publication status
- `allowReview` (Boolean): Allow review after submission
- `showCorrectAnswers` (Boolean): Show answers after completion
- `randomizeQuestions` (Boolean): Randomize question order
- `randomizeOptions` (Boolean): Randomize options order
- `createdAt` (DateTime): Creation timestamp
- `updatedAt` (DateTime): Last update timestamp
- `deletedAt` (DateTime, Nullable): Soft delete timestamp

#### Questions
- `id` (UUID): Primary key
- `assessmentId` (UUID, FK): Associated assessment
- `type` (Enum): multiple_choice | short_answer | code | matching | drag_drop | image
- `questionText` (Text): The question
- `description` (Text, Nullable): Additional description
- `points` (Integer): Points for this question
- `difficulty` (Enum): easy | medium | hard
- `explanation` (Text, Nullable): Explanation after submission
- `tags` (Array): Question tags/keywords
- `order` (Integer): Order in assessment
- `createdAt` (DateTime): Creation timestamp
- `updatedAt` (DateTime): Last update timestamp

#### QuestionOptions
- `id` (UUID): Primary key
- `questionId` (UUID, FK): Associated question
- `text` (String): Option text
- `isCorrect` (Boolean): Is this the correct answer
- `explanation` (Text, Nullable): Option explanation
- `order` (Integer): Option order

#### Results
- `id` (UUID): Primary key
- `assessmentId` (UUID, FK): Assessment ID
- `userId` (UUID, FK): Student/taker ID
- `score` (Integer): Total score achieved
- `percentage` (Integer): Percentage score (0-100)
- `passed` (Boolean): Whether passed
- `timeSpent` (Integer): Time spent in seconds
- `startedAt` (DateTime): Start time
- `submittedAt` (DateTime): Submission time
- `isReviewed` (Boolean): Instructor reviewed
- `reviewedBy` (UUID, FK, Nullable): Reviewer ID
- `feedback` (Text, Nullable): Instructor feedback
- `status` (Enum): submitted | grading | graded | reviewed

#### Answers
- `id` (UUID): Primary key
- `resultId` (UUID, FK): Result ID
- `questionId` (UUID, FK): Question ID
- `answerText` (Text, Nullable): Text answer
- `selectedOption` (Integer, Nullable): Selected option index
- `selectedOptions` (Array, Nullable): Multiple selections
- `isCorrect` (Boolean): Is answer correct
- `pointsEarned` (Integer): Points awarded
- `createdAt` (DateTime): Answer timestamp

#### Classes
- `id` (UUID): Primary key
- `name` (String): Class name
- `description` (Text, Nullable): Class description
- `code` (String, Unique): Enrollment code
- `instructorId` (UUID, FK): Instructor ID
- `capacity` (Integer): Max students
- `createdAt` (DateTime): Creation timestamp
- `updatedAt` (DateTime): Last update timestamp

#### Enrollments
- `id` (UUID): Primary key
- `classId` (UUID, FK): Class ID
- `userId` (UUID, FK): User ID
- `role` (Enum): student | TA
- `enrolledAt` (DateTime): Enrollment date
- `unenrolledAt` (DateTime, Nullable): Unenrollment date

#### Assignments
- `id` (UUID): Primary key
- `assessmentId` (UUID, FK): Assessment ID
- `classId` (UUID, FK): Class ID
- `dueDate` (DateTime): Submission deadline
- `visibleFrom` (DateTime): When assignment becomes visible
- `visibleUntil` (DateTime): When assignment becomes hidden
- `assignedBy` (UUID, FK): Instructor ID
- `createdAt` (DateTime): Creation timestamp

### Database Indexes

Key indexes for performance:
```sql
-- Users
CREATE INDEX idx_users_email ON users(email);
CREATE INDEX idx_users_role ON users(role);

-- Assessments
CREATE INDEX idx_assessments_created_by ON assessments(created_by);
CREATE INDEX idx_assessments_category ON assessments(category);
CREATE INDEX idx_assessments_published ON assessments(is_published);

-- Questions
CREATE INDEX idx_questions_assessment_id ON questions(assessment_id);

-- Results
CREATE INDEX idx_results_user_id ON results(user_id);
CREATE INDEX idx_results_assessment_id ON results(assessment_id);
CREATE INDEX idx_results_submitted_at ON results(submitted_at);

-- Enrollments
CREATE INDEX idx_enrollments_user_id ON enrollments(user_id);
CREATE INDEX idx_enrollments_class_id ON enrollments(class_id);
```

For detailed schema diagram and migration scripts, see [DATABASE_SCHEMA.md](./docs/DATABASE_SCHEMA.md)

## 🚀 Deployment

### Deployment Checklist

Before deploying to production:

```
- [ ] All tests passing (npm test)
- [ ] Environment variables configured
- [ ] Database migrations run
- [ ] SSL/TLS certificates obtained
- [ ] Backup strategy in place
- [ ] Monitoring and logging configured
- [ ] Security audit completed
- [ ] Performance tested
- [ ] Load testing completed
- [ ] Documentation updated
```

### Docker Deployment (Recommended)

```bash
# Build production images
docker-compose -f docker-compose.prod.yml build

# Push to registry (optional)
docker tag <image-name> registry.example.com/<image-name>:latest
docker push registry.example.com/<image-name>:latest

# Deploy
docker-compose -f docker-compose.prod.yml up -d

# View logs
docker-compose logs -f

# Update specific service
docker-compose -f docker-compose.prod.yml up -d --no-deps --build backend
```

### Cloud Deployment Options

#### AWS EC2 with PM2
```bash
# Connect to instance
ssh -i key.pem ec2-user@your-instance-ip

# Clone repository
git clone https://github.com/yourusername/Online-Skill-Assessment-Platform.git
cd Online-Skill-Assessment-Platform

# Install dependencies
npm install
cd backend && npm install && cd ../frontend && npm install && cd ..

# Build applications
cd backend && npm run build && cd ../frontend && npm run build && cd ..

# Install PM2 globally
npm install -g pm2

# Create ecosystem.config.js
cat > ecosystem.config.js << 'EOF'
module.exports = {
  apps: [
    {
      name: 'skill-api',
      script: './backend/dist/app.js',
      instances: 'max',
      exec_mode: 'cluster',
      env: { NODE_ENV: 'production' },
      error_file: './logs/api-error.log',
      out_file: './logs/api-out.log'
    },
    {
      name: 'skill-frontend',
      script: 'serve',
      args: '-s ./frontend/build -l 3000',
      error_file: './logs/frontend-error.log',
      out_file: './logs/frontend-out.log'
    }
  ]
};
EOF

# Start with PM2
pm2 start ecosystem.config.js

# Set to restart on reboot
pm2 startup
pm2 save
```

#### AWS Elastic Beanstalk
```bash
# Install EB CLI
pip install awsebcli

# Initialize project
eb init -p "Node.js 18 running on 64bit Amazon Linux 2" skill-assessment

# Create environment
eb create skill-assessment-prod

# Deploy
eb deploy

# View logs
eb logs

# SSH into instance
eb ssh
```

#### Heroku Deployment
```bash
# Install Heroku CLI
# Visit https://devcenter.heroku.com/articles/heroku-cli

# Login to Heroku
heroku login

# Create app
heroku create your-app-name

# Set environment variables
heroku config:set NODE_ENV=production
heroku config:set JWT_SECRET=your_secret_here
heroku config:set DATABASE_URL=postgresql://user:pass@host:port/db

# Deploy
git push heroku main

# View logs
heroku logs --tail

# Open app
heroku open
```

#### Google Cloud Run
```bash
# Build image
docker build -t skill-assessment:latest .

# Configure Docker
gcloud auth configure-docker

# Tag image
docker tag skill-assessment:latest gcr.io/YOUR_PROJECT_ID/skill-assessment:latest

# Push to Container Registry
docker push gcr.io/YOUR_PROJECT_ID/skill-assessment:latest

# Deploy to Cloud Run
gcloud run deploy skill-assessment \
  --image gcr.io/YOUR_PROJECT_ID/skill-assessment:latest \
  --platform managed \
  --region us-central1 \
  --memory 2Gi \
  --cpu 2 \
  --set-env-vars NODE_ENV=production,DATABASE_URL=...
```

#### Azure App Service
```bash
# Create resource group
az group create --name skill-assessment-rg --location eastus

# Create App Service plan
az appservice plan create --name skill-assessment-plan \
  --resource-group skill-assessment-rg --sku B2 --is-linux

# Create web app
az webapp create --resource-group skill-assessment-rg \
  --plan skill-assessment-plan --name skill-assessment-app \
  --runtime "NODE|18-lts"

# Deploy from local Git
az webapp deployment source config-local-git \
  --resource-group skill-assessment-rg \
  --name skill-assessment-app

# Set environment variables
az webapp config appsettings set --resource-group skill-assessment-rg \
  --name skill-assessment-app --settings NODE_ENV=production
```

#### DigitalOcean App Platform
```bash
# Create app.yaml
cat > app.yaml << 'EOF'
name: skill-assessment
services:
- name: api
  github:
    repo: yourusername/Online-Skill-Assessment-Platform
    branch: main
  build_command: cd backend && npm run build
  run_command: cd backend && npm start
  http_port: 5000
- name: web
  github:
    repo: yourusername/Online-Skill-Assessment-Platform
    branch: main
  build_command: cd frontend && npm run build
  run_command: cd frontend && npm start
  http_port: 3000
EOF

# Deploy
doctl apps create --spec app.yaml
```

### Pre-Deployment Tasks

```bash
# Update dependencies
npm update
npm audit fix

# Run security checks
npm audit

# Run tests
npm test -- --coverage

# Build production bundles
npm run build

# Verify build
npm start  # Test locally

# Commit changes
git add .
git commit -m "chore: production build"
git tag v1.0.0
git push origin main --tags
```

For detailed deployment instructions for various platforms, see [DEPLOYMENT.md](./docs/DEPLOYMENT.md)

## 🔒 Security

### Security Features Implemented

- ✅ **JWT-based Authentication** - Secure token-based authentication with refresh tokens
- ✅ **Password Hashing** - bcrypt with 12 salt rounds for secure password storage
- ✅ **HTTPS/TLS** - All data in transit encrypted with SSL/TLS certificates
- ✅ **Input Validation** - Comprehensive XSS and SQL injection prevention
- ✅ **Rate Limiting** - DDoS protection with request rate limiting
- ✅ **CORS Configuration** - Controlled cross-origin request handling
- ✅ **Environment Variables** - No hardcoded secrets in source code
- ✅ **Database Encryption** - Sensitive data encrypted at rest
- ✅ **CSRF Protection** - Cross-site request forgery prevention
- ✅ **Security Headers** - HSTS, X-Frame-Options, Content-Security-Policy
- ✅ **Helmet.js** - HTTP header security middleware
- ✅ **Two-Factor Authentication** - Optional 2FA/MFA support
- ✅ **Audit Logging** - Log sensitive actions and access

### Authentication & Authorization

```typescript
// JWT Token Structure
{
  "iss": "skill-assessment-platform",
  "sub": "user-uuid",
  "aud": "skill-assessment-web-app",
  "exp": 1642262400,
  "iat": 1642176000,
  "nbf": 1642176000,
  "role": "student",
  "permissions": ["assessments:read", "results:read"]
}
```

### Role-Based Access Control (RBAC)

```
Admin
├── Manage users
├── Create/manage assessments
├── View all reports
├── System configuration
└── Security management

Instructor
├── Create assessments
├── Manage own classes
├── Grade assignments
├── View class analytics
└── Communicate with students

Student
├── Take assessments
├── View own results
├── Access learning materials
└── Download certificates

Evaluator
├── Grade assignments
├── Provide feedback
└── View assigned results

Guest
└── View public assessments (read-only)
```

### Security Checklist for Production

```
Authentication & Authorization:
- [ ] Change default JWT secrets
- [ ] Enable 2FA for admin accounts
- [ ] Set strong password policies
- [ ] Implement session timeouts
- [ ] Configure SSO if needed
- [ ] Set up API keys with rotation

Data Protection:
- [ ] Enable database encryption
- [ ] Configure encrypted connections (SSL/TLS)
- [ ] Set up regular backups
- [ ] Implement backup encryption
- [ ] Test disaster recovery procedures
- [ ] Set up database activity monitoring

Infrastructure:
- [ ] Enable HTTPS/TLS in production
- [ ] Configure secure headers (Helmet.js)
- [ ] Set up WAF (Web Application Firewall)
- [ ] Configure security groups/firewalls
- [ ] Enable VPC for database
- [ ] Set up DDoS protection

Monitoring & Logging:
- [ ] Enable access logging
- [ ] Set up security event logging
- [ ] Configure log retention policies
- [ ] Set up real-time alerts
- [ ] Enable vulnerability scanning
- [ ] Configure intrusion detection

Dependencies:
- [ ] Update all dependencies
- [ ] Run npm audit and fix issues
- [ ] Set up dependency scanning
- [ ] Configure automated updates
- [ ] Review license compliance

Operations:
- [ ] Implement disaster recovery plan
- [ ] Set up automated backups
- [ ] Configure incident response procedure
- [ ] Train team on security practices
- [ ] Regular security audits
- [ ] Penetration testing (quarterly)
```

### Secure Configuration Examples

**Helmet.js Headers:**
```typescript
import helmet from 'helmet';

app.use(helmet());
app.use(helmet.contentSecurityPolicy({
  directives: {
    defaultSrc: ["'self'"],
    scriptSrc: ["'self'", "'unsafe-inline'"],
    styleSrc: ["'self'", "'unsafe-inline'"],
    imgSrc: ["'self'", "data:", "https:"],
  },
}));
app.use(helmet.hsts({ maxAge: 31536000, includeSubDomains: true }));
```

**Password Security:**
```typescript
import bcrypt from 'bcrypt';

// Hashing password
const salt = await bcrypt.genSalt(12);
const hashedPassword = await bcrypt.hash(plainPassword, salt);

// Validating password
const isValid = await bcrypt.compare(plainPassword, hashedPassword);
```

**Input Validation:**
```typescript
import { body, validationResult } from 'express-validator';

router.post('/login', [
  body('email').isEmail().normalizeEmail(),
  body('password').isLength({ min: 8 }).trim().escape(),
], (req, res) => {
  const errors = validationResult(req);
  if (!errors.isEmpty()) {
    return res.status(400).json({ errors: errors.array() });
  }
  // Process login
});
```

**Rate Limiting:**
```typescript
import rateLimit from 'express-rate-limit';

const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100, // 100 requests per window
  message: 'Too many requests, please try again later',
  standardHeaders: true,
  legacyHeaders: false,
});

app.use('/api/', limiter);
```

### Reporting Security Issues

If you discover a security vulnerability, please **DO NOT** create a public GitHub issue. Instead:

1. Email: security@skillassessment.com
2. Include detailed description of the vulnerability
3. Provide steps to reproduce
4. Allow 30 days for fix before public disclosure

For detailed security guidelines, see [SECURITY.md](./docs/SECURITY.md)

## 📊 Performance

### Performance Optimization Strategies

**Frontend:**
- **Code Splitting** - Dynamic imports and lazy loading of routes
- **Bundle Optimization** - Minification and tree-shaking
- **Image Optimization** - WebP format, responsive images, lazy loading
- **Caching** - Service workers and HTTP caching headers
- **CDN** - Static assets served via CloudFront or Cloudflare
- **Compression** - Gzip and Brotli compression for assets

**Backend:**
- **Database Caching** - Redis for session and query caching
- **Database Optimization** - Proper indexing on frequently queried columns
- **Query Optimization** - Pagination, select specific columns
- **Connection Pooling** - Reuse database connections
- **Compression** - Gzip for API responses
- **Load Balancing** - Distribute traffic across multiple instances
- **Horizontal Scaling** - Add more server instances

**Infrastructure:**
- **CDN** - Distribute content globally
- **Caching Layer** - Redis/Memcached for hot data
- **Database Replication** - Read replicas for scaling
- **Message Queues** - Async job processing
- **Monitoring** - Real-time performance metrics

### Performance Benchmarks

**Target Metrics:**
```
Frontend Performance:
- First Contentful Paint (FCP): < 1.5s
- Largest Contentful Paint (LCP): < 2.5s
- Cumulative Layout Shift (CLS): < 0.1
- Time to Interactive (TTI): < 3.5s
- Page Size: < 3MB (initial load)

Backend Performance:
- API Response Time: < 200ms (p95)
- Database Query Time: < 100ms (p95)
- Throughput: > 1000 requests/second
- Availability: 99.9% uptime

Real User Monitoring:
- Bounce Rate: < 5%
- Time on Site: > 5 minutes
- Conversion Rate: > 5%
```

### Monitoring Tools

**Application Performance Monitoring (APM):**
- New Relic
- DataDog
- Dynatrace
- Elastic APM
- AWS X-Ray

**Frontend Monitoring:**
```typescript
import WebVitals from 'web-vitals';

const handleMetric = (metric) => {
  console.log(`${metric.name}: ${metric.value}ms`);
  // Send to analytics service
};

WebVitals.getCLS(handleMetric);
WebVitals.getFID(handleMetric);
WebVitals.getFCP(handleMetric);
WebVitals.getLCP(handleMetric);
```

**Database Query Profiling:**
```javascript
// Enable query logging
const queryConfig = {
  logging: (sql, timing) => {
    if (timing > 100) { // Log slow queries
      console.warn(`Slow query (${timing}ms): ${sql}`);
    }
  }
};
```

**Load Testing:**
```bash
# Using Apache Bench
ab -n 10000 -c 100 http://localhost:3000/

# Using Artillery
artillery quick --count 300 --num 10000 http://localhost:3000/

# Using k6
k6 run load-test.js
```

**Monitoring Dashboard:**
```bash
# Start Prometheus
docker run -p 9090:9090 \
  -v $(pwd)/prometheus.yml:/etc/prometheus/prometheus.yml \
  prom/prometheus

# Start Grafana
docker run -p 3000:3000 \
  -e GF_SECURITY_ADMIN_PASSWORD=admin \
  grafana/grafana
```

For detailed performance optimization guide, see [PERFORMANCE.md](./docs/PERFORMANCE.md)

## 🐛 Troubleshooting

### Backend Issues

#### 1. Database Connection Failed

**Error:**
```
Error: ECONNREFUSED 127.0.0.1:5432
```

**Solutions:**
```bash
# Check PostgreSQL is running
sudo service postgresql status

# Or with Docker
docker-compose ps

# Verify connection string in .env
echo $DATABASE_URL

# Test connection
psql -U postgres -h localhost -d skill_assessment_db -c "SELECT 1"

# Reset database
npm run db:reset
```

#### 2. Port Already in Use

**Error:**
```
Error: listen EADDRINUSE: address already in use :::5000
```

**Solutions:**
```bash
# Find process using port
lsof -i :5000

# Kill process
kill -9 <PID>

# Or change PORT in .env
echo "PORT=5001" >> .env

# Or use different port with npm
PORT=5001 npm run dev
```

#### 3. Module Not Found / Dependencies Issue

**Error:**
```
Error: Cannot find module 'express'
```

**Solutions:**
```bash
# Clear node_modules and reinstall
rm -rf node_modules package-lock.json
npm install

# Or with yarn
rm -rf node_modules yarn.lock
yarn install

# Verify installation
npm list express
```

#### 4. Migration Errors

**Error:**
```
Error: Migration file not found
```

**Solutions:**
```bash
# Check migration status
npm run db:migrate:status

# Rollback last migration
npm run db:migrate:undo

# Rollback all migrations
npm run db:migrate:undo:all

# Run migrations again
npm run db:migrate
```

#### 5. JWT Token Invalid

**Error:**
```
JsonWebTokenError: invalid token
```

**Solutions:**
```bash
# Regenerate JWT_SECRET in .env
# Make sure it's at least 32 characters
JWT_SECRET=$(openssl rand -base64 32)

# Restart server
npm run dev

# Clear any stored tokens in browser DevTools
```

### Frontend Issues

#### 1. CORS Errors

**Error:**
```
Access to XMLHttpRequest has been blocked by CORS policy
```

**Solutions:**
```bash
# Check backend CORS configuration
# In backend .env:
CORS_ORIGIN=http://localhost:3000

# Verify frontend URL
REACT_APP_API_URL=http://localhost:5000/api/v1

# Restart both services
```

#### 2. Build Errors

**Error:**
```
Error: ENOSPC: System limit reached
```

**Solutions:**
```bash
# Increase file watches limit (Linux/Mac)
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf
sudo sysctl -p

# Or clear build cache
rm -rf build dist .next

# Rebuild
npm run build
```

#### 3. Blank Page / White Screen

**Solutions:**
```bash
# Check browser console for errors
# Open DevTools: F12 or Cmd+Option+I

# Clear browser cache
# Chrome: Cmd+Shift+Delete (Mac) or Ctrl+Shift+Delete (Windows)

# Try different port
PORT=3001 npm start

# Check if backend is running
curl http://localhost:5000/api/health

# Rebuild frontend
npm run build
npm start
```

### Docker Issues

#### 1. Container Won't Start

**Solutions:**
```bash
# Check logs
docker-compose logs backend

# Rebuild image
docker-compose build --no-cache backend

# Reset volumes
docker-compose down -v
docker-compose up -d
```

#### 2. Database Volume Permission Issues

**Solutions:**
```bash
# Fix permissions (Linux)
sudo chown -R $USER:$USER ./data

# Or use Docker volumes properly
docker volume ls
docker volume rm skill-assessment-db-data
docker-compose up -d
```

#### 3. Out of Memory

**Solutions:**
```bash
# Increase Docker memory limit
# Docker Desktop → Preferences → Resources → Memory

# Or check current usage
docker stats

# Reduce number of containers
docker-compose down
docker-compose up -d backend db
```

### Common Quick Fixes

```bash
# Clear everything and start fresh
docker-compose down -v
rm -rf node_modules backend/node_modules frontend/node_modules
npm install
cd backend && npm install && cd ../frontend && npm install && cd ..
docker-compose up -d

# Check all services
docker-compose ps

# View combined logs
docker-compose logs -f

# Test backend health
curl http://localhost:5000/api/health

# Test frontend
curl http://localhost:3000

# Database backup before troubleshooting
docker-compose exec db pg_dump -U postgres skill_assessment_db > backup.sql

# Restore database
docker-compose exec -T db psql -U postgres skill_assessment_db < backup.sql
```

### Getting Help

1. **Check Documentation**: [docs/](./docs/)
2. **Search Issues**: [GitHub Issues](https://github.com/yourusername/Online-Skill-Assessment-Platform/issues)
3. **Ask Questions**: [GitHub Discussions](https://github.com/yourusername/Online-Skill-Assessment-Platform/discussions)
4. **Email Support**: support@skillassessment.com

For more troubleshooting tips, see [TROUBLESHOOTING.md](./docs/TROUBLESHOOTING.md)

## 🗺️ Roadmap

### Phase 1 (Current - Q1 2026)
Core platform foundation with essential assessment features.

**Completed:**
- [x] Core assessment platform architecture
- [x] User authentication and RBAC
- [x] Basic assessment creation and taking
- [x] Real-time scoring and feedback
- [x] Student analytics dashboard

**In Progress:**
- [ ] Mobile app development (React Native)
- [ ] Advanced plagiarism detection (Turnitin integration)
- [ ] AI-powered question suggestions
- [ ] Enhanced reporting features

**Planned:**
- [ ] Proctored exam support
- [ ] Eye-tracking and behavior monitoring
- [ ] Advanced learning path recommendations

### Phase 2 (Q2-Q3 2026)
Advanced features and integrations.

**Features:**
- [ ] AI-powered essay grading with NLP
- [ ] Real-time collaboration tools
- [ ] Coding environment (IDE integration)
- [ ] Video recording and presentation assessments
- [ ] Peer review system with rubrics
- [ ] LMS integrations (Canvas, Blackboard, Moodle)
- [ ] SCORM 1.2 / xAPI support
- [ ] Advanced branching logic for adaptive assessments

### Phase 3 (Q4 2026+)
Enterprise features and market expansion.

**Enterprise Features:**
- [ ] White-label solution
- [ ] Advanced SSO (SAML, OAuth2)
- [ ] Custom branding and themes
- [ ] Advanced analytics and business intelligence
- [ ] Compliance certifications (HIPAA, FERPA, GDPR)
- [ ] International language support (20+ languages)
- [ ] Advanced API for third-party integrations

**Market Expansion:**
- [ ] Certification programs marketplace
- [ ] Skill-based job matching
- [ ] Corporate training platform
- [ ] University partnerships
- [ ] Certification revenue model

### Technology Roadmap

**Infrastructure:**
- [ ] Kubernetes deployment support
- [ ] GraphQL API alongside REST
- [ ] Microservices architecture
- [ ] Edge computing support
- [ ] Serverless function support (AWS Lambda)

**Performance:**
- [ ] Offline mode support
- [ ] Progressive Web App (PWA) features
- [ ] Real-time sync with Service Workers
- [ ] Advanced caching strategies
- [ ] Performance monitoring dashboard

**Developer Experience:**
- [ ] Webhook system
- [ ] Plugin architecture
- [ ] SDK for multiple languages
- [ ] API client libraries
- [ ] Enhanced documentation and tutorials

### Community Contributions Welcome

We're always looking for community contributions! See areas where you can help:

- 🐛 **Bug Fixes**: Report and fix issues
- ✨ **Features**: Implement new functionality
- 📚 **Documentation**: Improve guides and examples
- 🌍 **Translations**: Support new languages
- 🧪 **Testing**: Improve test coverage
- 💡 **Ideas**: Suggest new features

Check [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for guidelines.

## 🤝 Contributing

We welcome contributions from developers, designers, and documentation writers! This project thrives on community involvement.

### Getting Started

1. **Fork the Repository**
   ```bash
   # Click "Fork" button on GitHub
   ```

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Online-Skill-Assessment-Platform.git
   cd Online-Skill-Assessment-Platform
   ```

3. **Add Upstream Remote**
   ```bash
   git remote add upstream https://github.com/ORIGINAL_OWNER/Online-Skill-Assessment-Platform.git
   ```

4. **Create Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

### Development Workflow

#### Before Starting

1. **Sync with upstream** to get latest changes
   ```bash
   git fetch upstream
   git merge upstream/main
   ```

2. **Create feature branch** following naming convention:
   - Feature: `feature/short-description`
   - Bug fix: `bugfix/issue-number`
   - Documentation: `docs/topic`
   - Chore: `chore/description`

#### While Developing

1. **Follow code style**: We use ESLint and Prettier
   ```bash
   npm run lint
   npm run format
   ```

2. **Write tests** for new functionality
   ```bash
   npm test
   npm run test:watch
   ```

3. **Update documentation** if needed
   - Code comments for complex logic
   - JSDoc for functions
   - Update relevant docs/*.md files

4. **Commit with descriptive messages**
   ```bash
   git commit -m "feat: add amazing feature"
   git commit -m "fix: resolve issue #123"
   git commit -m "docs: update installation guide"
   ```

   Follow [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` New feature
   - `fix:` Bug fix
   - `docs:` Documentation
   - `style:` Code style (formatting, etc.)
   - `refactor:` Code refactoring
   - `test:` Test additions or changes
   - `chore:` Build process, dependencies

### Code Standards

#### TypeScript/JavaScript
- Use **TypeScript** for type safety
- Follow **ESLint** configuration
- Use **Prettier** for formatting
- Min 80% test coverage

```typescript
// Good
function getUserById(id: string): Promise<User> {
  // Implementation
}

// Bad
function getUserById(id) {
  // No type annotations
}
```

#### Component Structure (React)
```typescript
import React from 'react';
import styles from './Component.module.css';
import { useCustomHook } from '@/hooks';

/**
 * ComponentName - Brief description
 * @param {Object} props - Component props
 * @param {string} props.title - Title text
 * @returns {JSX.Element}
 */
export const ComponentName: React.FC<ComponentProps> = ({
  title,
  ...props
}) => {
  const [state, setState] = React.useState('');

  return <div className={styles.container}>{title}</div>;
};

export default ComponentName;
```

#### API Endpoints
```typescript
/**
 * Create new assessment
 * @method POST
 * @route /assessments
 * @access Instructor, Admin
 * @param {AssessmentInput} body - Assessment data
 * @returns {Assessment} Created assessment
 * @throws {ValidationError} Invalid input
 * @throws {UnauthorizedError} Insufficient permissions
 */
router.post('/assessments', authenticateUser, authorizeRole('instructor'), 
  validateInput(assessmentSchema), async (req, res) => {
  // Implementation
});
```

### Testing Requirements

```bash
# Run unit tests
npm test

# Run tests in watch mode
npm test -- --watch

# Generate coverage report
npm test -- --coverage

# Run end-to-end tests
npm run test:e2e
```

**Test Coverage Thresholds:**
- Statements: 80%
- Branches: 75%
- Functions: 80%
- Lines: 80%

### Pull Request Process

1. **Update your branch** with latest main
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Push to your fork**
   ```bash
   git push origin feature/AmazingFeature
   ```

3. **Create Pull Request**
   - Go to GitHub and click "Create Pull Request"
   - Fill out the PR template completely
   - Link related issues (#123)
   - Request reviewers

4. **PR Checklist**
   - [ ] Code follows style guidelines
   - [ ] Tests added and passing
   - [ ] Documentation updated
   - [ ] No breaking changes (or documented)
   - [ ] Commit messages follow convention
   - [ ] Changes reviewed locally
   - [ ] No merge conflicts
   - [ ] CI/CD checks pass

### PR Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Related Issues
Closes #123

## Testing
- [ ] Unit tests added
- [ ] Manual testing done

## Screenshots (if applicable)
[Screenshots here]

## Checklist
- [ ] Follows code style
- [ ] Tests pass
- [ ] Documentation updated
```

### Documentation Guidelines

1. **README Updates**: Explain "why" not just "how"
2. **Code Comments**: Document complex logic
3. **API Docs**: Include request/response examples
4. **Tutorials**: Step-by-step guides with screenshots
5. **FAQs**: Common questions and solutions

### Commit Message Examples

```bash
# Feature
git commit -m "feat(assessments): add AI-powered grading"

# Bug fix with issue reference
git commit -m "fix(auth): resolve token refresh issue #456"

# Documentation
git commit -m "docs: update installation guide for Windows"

# Multiple lines
git commit -m "feat(api): add pagination to assessments endpoint

- Add limit and offset parameters
- Default limit set to 10
- Return total count in response
- Add tests for pagination"
```

### Resources for Contributors

- [Setup Guide](./docs/INSTALLATION.md)
- [Architecture Guide](./docs/ARCHITECTURE.md)
- [API Documentation](./docs/API_DOCS.md)
- [Coding Standards](./docs/CODING_STANDARDS.md)
- [Git Workflow](./docs/GIT_WORKFLOW.md)

### Community

- **GitHub Issues**: Report bugs and request features
- **GitHub Discussions**: Ask questions and share ideas
- **Discord**: [Join our community](https://discord.gg/example)
- **Email**: dev@skillassessment.com
- **Twitter**: [@skillassessment](https://twitter.com/skillassessment)

### Recognition

Contributors will be recognized in:
- README contributors section
- Release notes
- Monthly community spotlight
- Special Discord role

Thank you for contributing! 🎉

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for complete details.

### What You Can Do
- ✅ Use commercially
- ✅ Modify the code
- ✅ Distribute copies
- ✅ Use privately

### Requirements
- ⚠️ Include license and copyright notice
- ⚠️ State significant changes

### Limitations
- ❌ No warranty or liability
- ❌ No trademark rights

For more details, see [MIT License](https://opensource.org/licenses/MIT)

---

## 📞 Contact

### Getting Help

**For General Questions:**
- 📧 **Email**: support@skillassessment.com
- 💬 **Discord**: [Join our community](https://discord.gg/skillassessment)
- 💭 **GitHub Discussions**: [Ask questions](https://github.com/yourusername/Online-Skill-Assessment-Platform/discussions)
- 🐦 **Twitter**: [@SkillAssess](https://twitter.com/skillassessment)

**For Bug Reports:**
- 🐛 **GitHub Issues**: [Report a bug](https://github.com/yourusername/Online-Skill-Assessment-Platform/issues)
- 📧 **Email**: bugs@skillassessment.com

**For Security Issues:**
- 🔒 **Security Team**: security@skillassessment.com
- **Do NOT create public issues for security vulnerabilities**

**For Business Inquiries:**
- 💼 **Email**: business@skillassessment.com
- 📞 **Phone**: +1 (555) 123-4567
- 🌐 **Website**: [skillassessment.com](https://skillassessment.com)

### Project Information

**Author:** [Your Name/Organization]  
**Maintainer:** [@yourusername](https://github.com/yourusername)  
**Contributors:** [See all contributors](https://github.com/yourusername/Online-Skill-Assessment-Platform/graphs/contributors)  

**Repository:** [GitHub](https://github.com/yourusername/Online-Skill-Assessment-Platform)  
**Documentation:** [Online Docs](./docs)  
**Issues:** [GitHub Issues](https://github.com/yourusername/Online-Skill-Assessment-Platform/issues)  

---

## ⭐ Quick Links

### Documentation
- [Installation Guide](./docs/INSTALLATION.md) - Detailed setup instructions
- [API Documentation](./docs/API_DOCS.md) - Complete API reference
- [Database Schema](./docs/DATABASE_SCHEMA.md) - Database structure
- [Architecture Guide](./docs/ARCHITECTURE.md) - System design
- [Deployment Guide](./docs/DEPLOYMENT.md) - Production deployment
- [Security Guide](./docs/SECURITY.md) - Security best practices

### Resources
- [Contributing Guide](./docs/CONTRIBUTING.md) - How to contribute
- [Troubleshooting](./docs/TROUBLESHOOTING.md) - Common issues
- [Changelog](./CHANGELOG.md) - Version history
- [Code of Conduct](./CODE_OF_CONDUCT.md) - Community guidelines

### Community
- [GitHub Discussions](https://github.com/yourusername/Online-Skill-Assessment-Platform/discussions)
- [Discord Server](https://discord.gg/skillassessment)
- [Twitter](https://twitter.com/skillassessment)
- [LinkedIn](https://linkedin.com/company/skillassessment)

### Development
- [Frontend Repository](./frontend) - React/Vue frontend code
- [Backend Repository](./backend) - Node.js backend code
- [Project Board](https://github.com/yourusername/Online-Skill-Assessment-Platform/projects) - Development tracking
- [CI/CD Pipeline](https://github.com/yourusername/Online-Skill-Assessment-Platform/actions)

### Tools & Services
- [Docker Hub](https://hub.docker.com/r/yourusername/skill-assessment) - Docker images
- [npm Package](https://www.npmjs.com/package/skill-assessment-sdk) - SDK package
- [API Documentation](https://docs.skillassessment.com/api) - Interactive API docs
- [Status Page](https://status.skillassessment.com) - Service status

---

## 🎯 Project Statistics

- **Stars**: ⭐⭐⭐⭐⭐ Please star us!
- **Forks**: Friendly forks welcome
- **Contributors**: Active community
- **Last Update**: January 15, 2026
- **Version**: 1.0.0
- **License**: MIT

---

<div align="center">

### Made with ❤️ by the Skill Assessment Team

If you found this project helpful, please consider:
- ⭐ **Starring** the repository
- 🔗 **Sharing** with your network
- 💬 **Providing feedback** on GitHub
- 🤝 **Contributing** to the project

### Support Us

- [Sponsor on GitHub](https://github.com/sponsors/yourusername)
- [Buy Me a Coffee](https://buymeacoffee.com/skillassessment)
- [Patreon](https://patreon.com/skillassessment)

---

**[⬆ Back to Top](#-online-skill-assessment-platform)**

Last Updated: January 15, 2026  
Version: 1.0.0  
Status: ✅ Active Development

</div>
