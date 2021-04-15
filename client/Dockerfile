# Dockerfile for client

# Create image based on the official Node image from dockerhub
FROM node:14.15.3-alpine3.12

# Change directory so that our commands run inside this new directory
WORKDIR /usr/app

# Copy dependency definitions
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy local files to app folder
COPY . .

# Expose the port the app runs in
EXPOSE 3000

# Serve the app
CMD ["npm","start"]