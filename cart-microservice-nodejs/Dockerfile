# Use a Node.js base image
FROM node:14

# Set the working directory
WORKDIR /var/www

# Copy the package.json and package-lock.json first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the application port
EXPOSE 1004

# Start the application
CMD ["node", "index.js"]
