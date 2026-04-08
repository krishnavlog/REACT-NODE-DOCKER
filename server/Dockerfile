# Use Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy the entire app
COPY . .

# Expose port 5000
EXPOSE 5000

# Start the Node.js server
CMD ["node", "server.js"]
