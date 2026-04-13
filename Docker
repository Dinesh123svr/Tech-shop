# Use Node.js 18 alpine image as the base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the port the app runs on
EXPOSE 8080

# Environment variable for port
ENV PORT=8080

# Command to run the application
CMD ["npm", "start"]
