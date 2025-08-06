# Use Node 16 Alpine (lightweight image)
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

# Create a non-root user and group
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

# Give ownership of the app folder to the new user
RUN chown -R appuser:appgroup /app

# Switch to the non-root user
USER appuser

# Expose Angular dev port
EXPOSE 4200

# Start Angular development server
CMD ["ng", "serve", "--host", "0.0.0.0"]
