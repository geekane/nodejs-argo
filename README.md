# Minimalist Node.js Blog

A minimalist, high-performance personal blog landing page built with Node.js native `http` module and vanilla CSS. Supports responsive design and light/dark theme preference syncing.

## Features

- **No external dependencies**: Pure Node.js native `http` server.
- **Minimalist aesthetics**: Curated typography, clean layout, and smooth scaling.
- **Dark Mode support**: Responsive theme shifting built-in.
- **Dockerized deployment**: Lightweight Alpine-based Docker deployment configuration.

## Getting Started

### Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm run dev
   ```

3. Open `http://localhost:3000` in your web browser.

### Docker Deployment

To build and run the docker image:

```bash
docker build -t node-blog .
docker run -p 3000:3000 node-blog
```
