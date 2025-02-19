# Use Node.js base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy rest of the app
COPY . .

# Expose the port
EXPOSE 5001

# Start the app
CMD ["node", "index.js"]
