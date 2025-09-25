# Use Node.js base image
FROM node:14-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the frontend files
COPY . .

# Start the React app
CMD ["npm", "start"]
