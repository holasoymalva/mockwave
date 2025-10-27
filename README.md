# Apiwave - Backend Generation Platform

> Generate complete backend projects and APIs instantly using AI-powered automation

Apiwave is a modern SaaS platform that transforms API specifications into production-ready backend projects in seconds. Whether you're prototyping a new idea or building a production API, Apiwave handles the heavy lifting so you can focus on what matters.

## 🏗️ Development Setup

This repository contains the complete Apiwave platform built as a monorepo with React frontend and Node.js backend.

### Project Structure

```
apiwave-platform/
├── frontend/          # React frontend application
├── backend/           # Node.js backend services  
├── docker-compose.yml # Local development environment
└── package.json       # Monorepo configuration
```

### Prerequisites

- Node.js 18+ and npm 9+
- Docker and Docker Compose (for local development)

### Quick Start

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Set up environment variables:**
   ```bash
   cp .env.example .env
   cp frontend/.env.example frontend/.env
   # Edit the .env files with your configuration
   ```

3. **Start with Docker (recommended):**
   ```bash
   npm run docker:up
   ```

4. **Or start manually:**
   ```bash
   # Start database services
   docker-compose up postgres redis -d
   
   # Start both frontend and backend
   npm run dev
   ```

### Available Scripts

- `npm run dev` - Start both frontend and backend in development mode
- `npm run build` - Build both applications for production
- `npm run test` - Run tests for both applications
- `npm run lint` - Lint all code
- `npm run format` - Format code with Prettier
- `npm run docker:up` - Start all services with Docker
- `npm run docker:down` - Stop all Docker services

### Services

- **Frontend**: http://localhost:3000
- **Backend**: http://localhost:3001
- **PostgreSQL**: localhost:5432
- **Redis**: localhost:6379

### Technology Stack

**Frontend:**
- React 18 with TypeScript
- Vite for build tooling
- Tailwind CSS for styling
- React Query for state management
- Monaco Editor for code viewing

**Backend:**
- Node.js with Express.js
- TypeScript
- PostgreSQL database
- Redis for caching
- Socket.io for real-time features

**Development Tools:**
- ESLint + Prettier for code quality
- Vitest for testing
- Docker for containerization

## 🚀 Features

### Multiple Input Formats
- **Natural Language**: Describe your API in plain English
- **YAML Specifications**: Upload OpenAPI/Swagger files
- **JSON Schemas**: Import structured API definitions
- **Visual Wizard**: Build your API through an intuitive interface

### Complete Backend Generation
Powered by DeepSeek Coder V2, APIwave generates:
- ✅ RESTful API endpoints
- ✅ Authentication & authorization mechanisms
- ✅ Mock data generators
- ✅ Comprehensive testing frameworks
- ✅ Environment configuration files
- ✅ Documentation

### Interactive Preview
- Live API endpoint testing
- Real-time mock responses
- Syntax-highlighted code browser
- Instant specification updates

### One-Click Cloud Deployment
Deploy your generated backends directly to:
- AWS
- Google Cloud Platform
- Microsoft Azure
- And more...

### Secure Project Management
- OAuth authentication (Google, GitHub, GitLab)
- Version control for all projects
- Secure project sharing
- Team collaboration tools

## 🎯 Quick Start

### 1. Sign Up
```bash
Visit https://apiwave.io and sign in with your preferred OAuth provider
```

### 2. Create Your First Project
Choose your preferred input method:

**Natural Language:**
```
Create a REST API for a task management system with users, projects, and tasks. 
Include authentication and CRUD operations for all resources.
```

**YAML Upload:**
```yaml
openapi: 3.0.0
info:
  title: Task Manager API
  version: 1.0.0
paths:
  /tasks:
    get:
      summary: List all tasks
      ...
```

### 3. Preview & Test
- Explore generated endpoints in the interactive preview
- Test API calls with sample data
- Review the complete codebase
- Make adjustments as needed

### 4. Deploy or Download
- **Deploy**: One-click deployment to your preferred cloud provider (< 5 minutes)
- **Download**: Get the complete project as a ZIP file

## 💡 Use Cases

- **Rapid Prototyping**: Generate mock APIs for frontend development
- **API Design**: Validate API specifications before implementation
- **Backend Scaffolding**: Generate boilerplate code for new projects
- **Learning**: Explore best practices in API design and implementation
- **MVP Development**: Launch backend services quickly

## 📊 Subscription Tiers

### Free Tier
- Up to 5 projects per month
- Basic authentication options
- Community support
- 7-day project retention

### Pro Tier
- Unlimited projects
- Advanced authentication (OAuth2, JWT, API Keys)
- Priority support
- Unlimited project retention
- Usage analytics
- Custom domain support

### Enterprise Tier
- Everything in Pro
- Team collaboration features
- Private cloud deployment
- SLA guarantees
- Dedicated account manager
- Third-party integrations
- Advanced monitoring & analytics

## 🛠️ Supported Technologies

**Backend Frameworks:**
- Node.js (Express, Fastify, NestJS)
- Python (Flask, FastAPI, Django)
- Go (Gin, Echo)
- Java (Spring Boot)
- Ruby (Rails, Sinatra)

**Databases:**
- PostgreSQL
- MySQL
- MongoDB
- Redis

**Authentication:**
- JWT
- OAuth 2.0
- API Keys
- Session-based

## 📖 Documentation

Visit our [comprehensive documentation](https://docs.apiwave.io) for:
- Detailed tutorials
- API reference
- Best practices
- Example projects
- Integration guides

## 🔒 Security

APIwave takes security seriously:
- OAuth 2.0 authentication
- Encrypted data storage
- Secure project sharing with access controls
- Regular security audits
- GDPR compliant

## 🤝 Support

- **Documentation**: [docs.apiwave.io](https://docs.apiwave.io)
- **Email**: support@apiwave.io
- **Community Forum**: [community.apiwave.io](https://community.apiwave.io)
- **Twitter**: [@apiwave](https://twitter.com/apiwave)

## 🗺️ Roadmap

- [ ] GraphQL API generation
- [ ] WebSocket support
- [ ] Microservices architecture templates
- [ ] CI/CD pipeline integration
- [ ] API versioning management
- [ ] Load testing tools
- [ ] API monetization features

## 📜 License

Copyright © 2025 APIwave. All rights reserved.

## 🌟 Getting Started

Ready to revolutionize your API development workflow?

[Start Building Now](https://apiwave.io/signup) | [View Demo](https://apiwave.io/demo) | [Pricing](https://apiwave.io/pricing)

---

**Built with ❤️ for developers who want to move fast without breaking things.**