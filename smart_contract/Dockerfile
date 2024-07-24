# Use a Node.js base image
FROM node:14

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the smart contract files
COPY . .

# Expose port (if necessary, for example, if you run a local blockchain)
EXPOSE 8545

# Command to run the development server
CMD ["npx", "hardhat", "node"]
