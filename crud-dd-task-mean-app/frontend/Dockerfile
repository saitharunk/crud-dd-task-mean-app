FROM node:18

WORKDIR /usr/src/app

# Copy only package files first for caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the backend code
COPY . .

# Expose backend port
EXPOSE 3000

# Start backend using your main file
CMD ["node", "server.js"]
