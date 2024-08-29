# Stage 1: Build the application
FROM node:18-alpine AS build

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY email-sender-app/package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application files
COPY email-sender-app/. .

# Start the application
CMD ["npm", "start"]
