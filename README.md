# Docker Environment for PHP Studies

This repository contains a Docker-based development environment designed to facilitate learning and practicing PHP. It leverages Docker Compose to orchestrate multiple services, including PHP, Nginx, Composer, and MariaDB, offering an integrated and ready-to-use development experience.

## Repository Structure

- `docker-compose.yml`: Defines Docker services, including PHP, Nginx, Composer, and MariaDB.
- `nginx/`: Contains Nginx server configuration.
  - `default.conf`: Nginx configuration file.
- `src/`: Directory for storing your PHP scripts and projects.

## How to Use

1. **Clone the Repository**: Clone this repository to your local machine.
2. **Build and Start Containers**: At the root of the project, run `docker-compose up -d` to build and start the containers.
3. **Access and Modify**: Place your PHP files in the `src/` folder. They will be accessible via the Nginx server.
4. **Access the Application**: Once the containers are running, access your application by visiting `http://localhost` in your web browser.
5. **Interact with the Database**: 
    - The MariaDB service is set up and can be accessed by your PHP application. 
    - To directly access the MariaDB database, use the command: `docker exec -it php_container mysql -h db -u user -p`. You will be prompted to enter the password.

## Prerequisites

To use this environment, you will need Docker and Docker Compose installed on your machine. See the [official Docker documentation](https://docs.docker.com/get-docker/) for installation instructions.
