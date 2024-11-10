# PHP Project: exercise5php

This project is a simple web application built using PHP and containerized with Docker for deployment.

## Project Structure

- `index.php`: The main entry point of the web application.
- `Dockerfile`: Defines how the Docker image is built for the PHP project.
- `README.md`: Project documentation and instructions for execution.

Before running this project, you must have the following programs:

- **Docker**: To build and run the container. You can download Docker from [Docker Desktop](https://www.docker.com/products/docker-desktop).
- **Docker Hub Account**: To pull the project image directly from Docker Hub. Make sure you have an account and are logged in.

## Manual Execution from Code

1. **Download the Project from GitHub**:

   - Go to the repository on GitHub and click **"Code"**. Then select **"Download ZIP"** to download the project to your computer.
   - Unzip the ZIP file into a folder of your choice.

2. **Open a Terminal in the Project Folder**:

   - Navigate to the folder where you unzipped the project and go into the `exercise4go` project folder.
   - Open a terminal or command prompt (CMD) inside this folder. On Windows, you can right-click the folder and select **"Open PowerShell window here"**.

3. **Build the Docker image**:

     Run the following command in the terminal to build the Docker image:
        ```bash
           docker build -t meybili/exercise5php .
        ```

4. **Run the Application**:

    Once the image has been built successfully, run the following command to start the container:
        ```bash
        docker run --name exercise5php -p 80:80 meybili/exercise5php
        ```

## Running from Docker Hub

1. **Pull the image from Docker Hub**:

    ```bash
    docker pull meybili/exercise5php:latest
    ```

2. **Run the container for the project**:

        ```bash
        docker run --name exercise5php -p 80:80 meybili/exercise5php
        ```

3. Open your browser and navigate to http://localhost:80 to see the app.

### Output Example

![alt text](image.png)

### Notes

- Make sure Docker is running.
- If you have problems accessing http://localhost:80, check that the port is not in use or check your firewall.

## Credits

This project was developed by Meybili Olivares (https://github.com/meybili19).