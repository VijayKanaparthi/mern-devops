# Use Node.js as base image
FROM node:18

# Set working directory
WORKDIR /App

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire backend code
COPY . .

# Expose port 5000
EXPOSE 5000

# Start the application
CMD ["npm", "run", "dev"]
