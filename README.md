# fuzzy-octo-broccoli

An Express application with Vercel Speed Insights integration.

## Features

- Express.js web server
- Vercel Speed Insights for performance monitoring
- Static file serving
- Health check endpoint

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

```bash
npm install
```

### Running the Application

```bash
# Development
npm run dev

# Production
npm start
```

The application will be available at `http://localhost:3000`

## Vercel Speed Insights

This project is configured with Vercel Speed Insights to monitor and analyze application performance.

### How it Works

Speed Insights automatically tracks:
- First Contentful Paint (FCP)
- Largest Contentful Paint (LCP)
- Cumulative Layout Shift (CLS)
- First Input Delay (FID)
- Time to First Byte (TTFB)

### Viewing Metrics

After deploying to Vercel:
1. Navigate to your Vercel dashboard
2. Select your project
3. Go to the "Speed Insights" tab
4. View real-time performance metrics

### Configuration

The Speed Insights script is included in `public/index.html` and will automatically collect performance data when the application is deployed to Vercel.

## API Endpoints

- `GET /` - Main application page
- `GET /api/health` - Health check endpoint

## Deployment

This application is configured for deployment on Vercel:

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## License

See [LICENSE](LICENSE) file for details.
