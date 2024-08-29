# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files
COPY email-sender-app/package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application files
COPY email-sender-app/. .

# Start the application
CMD ["npm", "start"]
