# WordPress Docker Compose Setup

This script sets up a WordPress environment using Docker Compose. It includes a MySQL database, WordPress container, and phpMyAdmin for easy database management.

## Prerequisites
- Docker: Install Docker on your system before running the script.

## Usage

1. Run the script:
   - Open a terminal.
   - Navigate to the directory where the script is located.
   - Run the following command:
     
     chmod +x wordpress_docker_setup.sh
     ./wordpress_docker_setup.sh
     

   The script performs the following actions:
   - Updates the package repositories and installs the `nano` text editor (optional).
   - Creates a `wordpress` directory and navigates into it.
   - Generates a `docker-compose.yml` file with the necessary configurations for MySQL, WordPress, and phpMyAdmin.
   - Starts the containers using Docker Compose.

2. Access WordPress:
   - Open a web browser and visit `http://localhost:8081` to access the WordPress site.
   - Follow the on-screen instructions to set up and configure your WordPress installation.

3. Access phpMyAdmin:
   - Open a web browser and visit `http://localhost:8080` to access phpMyAdmin.
   - Use the following credentials to log in:
     - Username: root
     - Password: 123
     - Host: db

4. Customize the Setup:
   - Modify the `docker-compose.yml` file in the `wordpress` directory to customize the configuration, such as ports or database credentials.

5. Clean up:
   - To stop and remove the containers, run the following command from within the `wordpress` directory:
     
     docker-compose down
     

Notes:
just clone this repo to your pwd and there you go
