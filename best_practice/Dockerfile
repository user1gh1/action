# Use an official Node.js runtime as the base image
FROM node:latest

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy all files from the current directory to the working directory in the container
COPY . .

# Expose the port on which your application runs
EXPOSE 80

# Define the command to start your application
CMD ["node", "server.mjs"]
