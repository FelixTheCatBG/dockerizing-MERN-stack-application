#  Dockerfile for Node Express Backend api (development)

# Create image based on the official Node image from dockerhub
FROM node:14.15.3-alpine3.12

# Create App Directory where our app will be places
RUN mkdir -p /usr/src/app

# Change directory so that our commands run inside this new directory
WORKDIR /usr/src/app

# Copy dependency definitions
COPY package*.json ./

# Install Dependencies
RUN npm install

# Get all the code needed to run the app and copy it to app folder
COPY . /usr/src/app

# Expose the port the app runs in
EXPOSE 8080

# Serve the app
CMD ["npm","start"]
