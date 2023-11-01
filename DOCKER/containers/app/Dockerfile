FROM node:latest

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY . .

# Install application dependencies
RUN npm install

# Copy the rest of the application code to the contain

# Expose the port your Node.js app listens on (e.g., 3000)
EXPOSE 3000

# Define the command to start your Node.js application
CMD ["node", "app.js"]



