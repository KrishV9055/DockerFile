# DockerFile

# Frontend Dockerfile
1. `FROM node:latest`: This line tells Docker to use an existing Docker image called "node" with the latest version. Docker images are like pre-packaged environments that contain everything needed to run an application.

2. `WORKDIR /app`: This sets the working directory inside the Docker container to `/app`. It's like navigating to a specific folder on your computer before doing anything else.

3. `COPY package*.json ./`: This copies the package.json file (and any other file that starts with "package") from your local machine into the `/app` directory in the Docker container. The package.json file typically lists all the dependencies needed for your Node.js application.

4. `RUN npm install`: This command runs inside the Docker container and installs all the dependencies listed in the package.json file. It's like running `npm install` on your local machine to install all the required libraries for your Node.js application.

5. `COPY . .`: This copies all the files and folders from your local machine into the `/app` directory in the Docker container. This includes your application code.

6. `EXPOSE 3000`: This command tells Docker to expose port 5000 from the container to the outside world. It's like opening a specific door on the container so that other programs can communicate with your Node.js application running inside.

7. `CMD ["npm", "start"]`: This sets the default command to run when the Docker container starts. In this case, it runs `npm start`, which typically starts your Node.js application. It's like setting the initial action when you turn on your computer.


# Backend Dockerfile
1. `FROM node:latest`: This line tells Docker to use an existing Docker image called "node" with the latest version. Docker images are like pre-packaged environments that contain everything needed to run an application.

2. `WORKDIR /app`: This sets the working directory inside the Docker container to `/app`. It's like navigating to a specific folder on your computer before doing anything else.

3. `COPY package*.json ./`: This copies the package.json file (and any other file that starts with "package") from your local machine into the `/app` directory in the Docker container. The package.json file typically lists all the dependencies needed for your Node.js application.

4. `RUN npm install`: This command runs inside the Docker container and installs all the dependencies listed in the package.json file. It's like running `npm install` on your local machine to install all the required libraries for your Node.js application.

5. `COPY . .`: This copies all the files and folders from your local machine into the `/app` directory in the Docker container. This includes your application code.

6. `EXPOSE 5000`: This command tells Docker to expose port 5000 from the container to the outside world. It's like opening a specific door on the container so that other programs can communicate with your Node.js application running inside.

7. `CMD ["npm", "start"]`: This sets the default command to run when the Docker container starts. In this case, it runs `npm start`, which typically starts your Node.js application. It's like setting the initial action when you turn on your computer.


# Compose File

