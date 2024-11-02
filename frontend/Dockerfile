# Frontend Dockerfile
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json (if exists) to install dependencies
COPY ./frontend/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend code
COPY ./frontend/ ./

# Expose the frontend port
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]