# Use the official Node.js image from the Docker Hub
FROM node:14

# Create and change to the app directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the app dependencies
RUN npm install

# Copy the app source code to the working directory
COPY . .

# Expose port 3000 to the outside world
EXPOSE 3000

# Run the app
CMD ["npm", "start"]