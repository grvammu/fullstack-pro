# Use a Node.js base image
FROM node:14

# Set the working directory inside the container
WORKDIR /var/www

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the application port
EXPOSE 1004

# Start the application
CMD ["node", "index.js"]
