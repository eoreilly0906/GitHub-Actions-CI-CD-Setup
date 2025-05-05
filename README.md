# Coding Quiz Application

A full-stack coding quiz application that tests users' knowledge of programming concepts. The application features a React frontend and a Node.js/TypeScript backend.

## CI/CD Pipeline

This project implements a robust Continuous Integration and Continuous Deployment (CI/CD) pipeline using:

- **GitHub Actions**: For automated testing and deployment workflows
- **Render**: For cloud deployment and hosting

### Pipeline Features

- Automated testing on every push and pull request
- Automatic deployment to Render when tests pass
- TypeScript compilation and build verification
- End-to-end testing with Cypress

### Workflow Structure

The CI/CD pipeline consists of two main workflows:

1. **Test Workflow**: Runs on every push and pull request
   - Installs dependencies
   - Builds both client and server
   - Runs TypeScript compilation
   - Executes Cypress tests

2. **Deploy Workflow**: Triggers after successful test workflow
   - Deploys the application to Render
   - Ensures zero-downtime deployments
   - Maintains production environment stability

## Getting Started

1. Clone the repository
2. Install dependencies: `npm install`
3. Start development server: `npm run develop`
4. Run tests: `npm test`

## Project Structure

- `client/`: React frontend application
- `server/`: Node.js/TypeScript backend
- `.github/workflows/`: GitHub Actions workflow configurations
- `render.yaml`: Render deployment configuration
