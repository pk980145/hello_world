#Tells Docker to use this Node version
FROM node:latest

#Tells Docker to create folder called code inside Docker image
WORKDIR /code

#Copies the package.json file into code folder
COPY package*.json ./ 

#Runs node package manager and install dependencies
RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]




# First step
# npm init -y


# To build the docker file
# docker build -t my-node-app .

# To build the docker file
# docker run -p 3000:3000 my-node-app



# # Use an official Node.js image as a base
# FROM node:v20.11.1

# # Set the working directory in the container
# WORKDIR /usr/src/app

# # Copy package.json and package-lock.json (if available) to the working directory
# COPY package*.json ./

# # Install npm dependencies
# RUN npm install

# # Copy the current directory contents into the container at /usr/src/app
# COPY . .

# # Expose the port the app runs on
# EXPOSE 3000

# # Command to run the application
# CMD ["node", "app.js"]
