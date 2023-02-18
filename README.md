# Deploying Laravel Application with Docker
This repository contains the files required to deploy a Laravel application using Docker. The deployment consists of a Dockerfile and a docker-compose.yml file.
## Prerequisites
Before deploying the Laravel application using Docker, you need to have the following prerequisites installed on your machine:

- Docker
- Docker Compose

## Deployment Steps
Follow the below steps to deploy the Laravel application using Docker:

1. Clone the repository to your local machine.
2. Navigate to the root directory of the cloned repository.
3. Build the Docker image by running the following command:
   \
   `docker build -t <your_image_name> `
4. Start the containers using Docker Compose by running the following command:
   \
   `docker-compose up -d`
5. Visit http://<your_instance_public_ip>:8080 in your web browser to see the Laravel application running.



## Dockerfile

The Dockerfile contains the instructions required to build the Docker image. It includes:

1. A base image of PHP with Apache installed.
2. Installation of necessary packages.
3. Copying the Laravel application files to the container.
4. Setting up the working directory.
5. Setting up the Apache virtual host.


## docker-compose.yml
The docker-compose.yml file defines the Docker services required to run the Laravel application. It includes:

- A service for the PHP application container.
- A service for the MySQL database container.
- Configuration for the volumes to be mounted.

## Configuration

You can configure the Laravel application by modifying the .env file. Make sure to update the database credentials and other settings as necessary.

## Conclusion

That's it! You have now successfully deployed a Laravel application using Docker. If you have any issues, please refer to the Docker documentation or the Laravel documentation for further guidance.

