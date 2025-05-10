# Use Node.js LTS base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json ./
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the port Gateway Service runs on
EXPOSE 3004

# Start the service
CMD ["node", "app.js"]
