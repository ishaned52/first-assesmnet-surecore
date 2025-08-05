# Use Node 16 (best match for Angular 14)
FROM node:16-alpine

# Create app directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --legacy-peer-deps

# Copy rest of the project
COPY . .

# Install Angular CLI
RUN npm install -g @angular/cli@14

# Expose the port the app runs on
EXPOSE 4200

# Run the dev server
CMD ["ng", "serve", "--host", "0.0.0.0"]