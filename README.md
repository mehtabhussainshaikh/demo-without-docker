# Express.js Starter App

A basic Node.js Express server ready for deployment.

## Quick Start

1. Install dependencies:
```bash
npm install
```

2. Create environment file:
```bash
cp .env.example .env
```

3. Start the server:
```bash
# Production
npm start

# Development (requires nodemon)
npm run dev
```

## API Endpoints

- `GET /` - Welcome message
- `GET /api/health` - Health check endpoint

## Environment Variables

- `PORT` - Server port (default: 3000)
- `NODE_ENV` - Environment mode (development/production)

## Deployment

### Heroku
1. Set environment variables in Heroku dashboard
2. Deploy using Git:
```bash
git add .
git commit -m "Initial deploy"
git push heroku main
```

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Deploy: `vercel`

### DigitalOcean App Platform
1. Connect your GitHub repository
2. Set build command: `npm install`
3. Set run command: `npm start`
4. Set environment variables

### Docker
1. Build image:
```bash
docker build -t express-app .
```

2. Run container:
```bash
docker run -p 3000:3000 express-app
```

## Project Structure

```
├── server.js          # Main server file
├── package.json       # Dependencies and scripts
├── .env.example       # Environment variables template
├── .gitignore         # Git ignore file
└── README.md          # This file
```
