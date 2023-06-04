FROM node:14-alpine

WORKDIR /app

# COPY package.json .
COPY package*.json ./
# RUN npm config set registry http://registry.npmjs.org/ && npm install
RUN npm install

COPY . .
# RUN cp -a /web/node_modules /usr/src/app/

# RUN webpack

# ENV NODE_ENV=production
# ENV PORT=4000
EXPOSE 8080
CMD [ "npm", "run" ,"start" ]

# EXPOSE 4000

# # Use an official Node.js runtime as a parent image
# FROM node:14-alpine

# # Set the working directory to /app
# WORKDIR /app

# # Copy the package.json and package-lock.json files to the container
# COPY package*.json ./

# # Install dependencies
# RUN npm install

# # Copy the rest of the application code to the container
# COPY . .

# # Set the environment variable for hot reloading
# ENV NODE_ENV development

# # Expose port 8080 for the application
# EXPOSE 8080

# # Start the application using webpack-dev-server with hot reloading
# CMD ["npm", "run", "dev"]