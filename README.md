# assignment2-yoshi

## Report (Approach Overview)

Actions's deploy.yml file defines what runner it will use. "ubuntu-latest" runner comes with "npm" and Node by default. This is CI/CD pipeline to deploy code on the Internet right after pushing it to the remote GitHub repository.
Docker container could be run and it runs locally. The Vite command is configured on package.json and we can use it to build this app as dist directory.

## CI/CD Deployment

[![Deploy to GitHub Pages](https://github.com/flatbase1012/assignment2-yoshi/actions/workflows/deploy.yml/badge.svg)](https://github.com/flatbase1012/assignment2-yoshi/actions/workflows/deploy.yml)

## Project Description
A brief description of your project - what it does, why it was created, and any other relevant information.

## Live Demo
[View the live demo](https://flatbase1012.github.io/assignment2-yoshi)

## Technology Stack
- React
- Vite
- Docker
- GitHub Actions
- GitHub Pages

## Local Development

### Prerequisites
- Docker and Docker Compose
- Git

### Setup and Run

1. Clone the repository
```bash
git clone https://github.com/flatbase1012/assignment2-yoshi
cd assignment2-yoshi
```

2. Start the Docker development environment
```bash
docker-compose up
```

3. Access the development server at [http://localhost:5173](http://localhost:5173)

## Environment Variables
The application uses the following environment variables:
- `NODE_ENV` - Set to "development" for local development

## Deployment

This project is automatically deployed to GitHub Pages using GitHub Actions when changes are pushed to the main branch.

### Manual Deployment
If you want to deploy manually:

1. Build the application
```bash
npm run build
```

2. Deploy to GitHub Pages
```bash
npm run deploy
```

## GitHub Actions Workflow

The CI/CD pipeline includes the following steps:
1. Checkout code
2. Setup Node.js environment
3. Install dependencies
4. Build the application
5. Deploy to GitHub Pages

## Configuration Details

### GitHub Pages Configuration
- Base path: `/assignment2-yoshi/` (configured in vite.config.js)
- Homepage URL: `https://flatbase1012.github.io/assignment2-yoshi`

### Docker Development Configuration
- Development server with hot reload
- Volume mounting for real-time code changes
- Port mapping from container to host 
