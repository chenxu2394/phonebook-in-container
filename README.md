# How to run

## Build the backend image and start the backend container
```
cd backend
docker build -t phonebook-backend-dev -f dev.Dockerfile .  
docker run -d -p 3001:3001 phonebook-backend-dev
```
## Build the frontend image and start the frontend container
```
cd frontend
docker build -t phonebook-frontend-dev -f dev.Dockerfile .  
docker run -d -p 3000:3000 --env REACT_APP_API_URL=http://localhost:3001/api phonebook-frontend-dev
```