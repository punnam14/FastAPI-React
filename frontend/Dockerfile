# Use an official Node.js image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy the rest of the application
COPY . .

# Expose React development server port
EXPOSE 3000

# Start React
CMD ["npm", "start"]
