# Use official Node.js runtime as a parent image
FROM node:18

# Set working directory in the container
WORKDIR /app

# Copy package.json & package-lock.json first (의존성 설치를 위해)
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy all project files
COPY . .

# Expose the application port
EXPOSE 5000

# Start the NestJS server
CMD ["npm", "run", "start"]