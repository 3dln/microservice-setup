# Use the official Node.js image as a base
FROM node:alpine

# Set the working directory
WORKDIR /app

# Copy package.json and yarn.lock into the working directory
COPY package.json yarn.lock ./

# Install dependencies
RUN yarn install --production

# Copy the remaining application files
COPY . .

# Build the Next.js application
RUN yarn build

# Expose the port the app will run on
EXPOSE 3000

# Start the application
CMD ["yarn", "start"]
