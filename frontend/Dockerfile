# Dockerfile for frontend service

# Use a base Node.js image
FROM node:14

# Install git (if not already installed)
RUN apt-get update && apt-get install -y git

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose port 3000
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]