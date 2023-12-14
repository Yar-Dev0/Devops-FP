# Use an official Node.js runtime as a base image
FROM node:14

# Set the working directory in the container
WORKDIR /frontend

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the current directory contents into the container at /app
COPY . .

# Expose port 3000 to the outside world
EXPOSE 3000

# Define environment variable for doctors service URL
ENV DOCTORS_SERVICE_URL doctors-service:9090

# Define environment variable for appointments service URL
ENV APPOINTMENTS_SERVICE_URL appointments-service:7070

# Command to run the application
CMD ["node", "app.js"]
