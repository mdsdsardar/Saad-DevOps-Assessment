# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the port (if your application requires one)
# EXPOSE 3000  # Uncomment if your application listens to a port

# Start the application
CMD ["npm", "start"]
