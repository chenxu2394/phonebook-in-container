# How to run

## Build the backend image
```
cd backend
docker build -t phonebook-backend-dev -f dev.Dockerfile .  
```
## Build the frontend image
```
cd frontend
docker build -t phonebook-frontend-dev -f dev.Dockerfile .  
```

## To set up the development environment using Docker Compose, at the root, run
```
docker compose -f docker-compose.dev.yml up -d
```

### For frontend development, visit `http://localhost:8080`
### For backend development, visit `http://localhost:8080/api/info` and `http://localhost:8080/api`
### Visit database at `http://localhost:8080/api/persons`