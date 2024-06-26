# Use the official Node.js 18 image as a base
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy the package.json and yarn.lock files
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port on which the Express.js server will run
EXPOSE 5000

# Start the Express.js server
CMD ["yarn", "start"]
