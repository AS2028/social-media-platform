# Base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy dependencies
COPY package*.json ./

# Install dependencies (safe mode)
RUN npm install --legacy-peer-deps

# Copy rest of the code
COPY . .

# Start app
CMD ["npm", "start"]

