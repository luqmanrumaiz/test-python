# Flask Server

A simple Flask server with Docker setup.

## Requirements

- Docker and Docker Compose

## Running the Server

### Using Docker Compose (recommended)

```bash
cd server
docker-compose up
```

The server will be available at http://localhost:8080

### Building and Running with Docker Directly

```bash
cd server
docker build -t flask-server .
docker run -p 8080:8080 flask-server
```

## API Endpoints

- `GET /api/health` - Health check endpoint
- `GET /api/hello` - Returns a greeting message
