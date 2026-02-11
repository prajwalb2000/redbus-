FROM node:16-alpine
 
# Create app directory
WORKDIR /app
 
# Copy dependency files
COPY package.json package-lock.json ./
 
# Install dependencies
RUN npm install
 
# Copy application source
COPY . .
 
# Expose backend port (change if your app uses a different one)
EXPOSE 5000
 
# Start the backend
CMD ["node", "app.js"]
 
