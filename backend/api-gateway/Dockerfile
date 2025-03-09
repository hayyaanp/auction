# Use Node.js LTS
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files first for layer caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy source code
COPY . .

# Expose the port your gateway runs on
EXPOSE 8080

# Start the gateway
CMD ["npm", "start"]