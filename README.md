This is a simple web-based task manager application built using HTML, CSS, and JavaScript, packaged within a Docker container for easy deployment and accessibility.

Running Locally:
To run the application on your local machine, you have two options: clone the repository or directly open the "index.html" file in your web browser.

Building the Docker Image and Running a Container:
Before proceeding, ensure you have Docker Desktop installed on your machine.
Navigate to the directory containing the Dockerfile and the web application's code.
In your terminal, open your preferred editor and execute the command: `docker build -t your-docker-image-name`. Remember to replace "your-docker-image-name" with your chosen image name.
After the image is successfully built, initiate a container using the following command: `docker run -d -p 8080:80 your-docker-image-name`. This command creates a container named "your-docker-image-name" and maps port 8080 of your host machine to port 80 of the container.
Access the running application by opening your web browser and navigating to 'http://localhost:8080'.

Assumptions and Development Considerations:
During the development process, certain decisions were made to ensure the application's efficiency and simplicity:
- The application was designed to be lightweight, incorporating only HTML, CSS, and JavaScript, all consolidated into a single "index.html" file. This approach streamlines deployment and enhances accessibility.
- Nginx was selected as the web server to host the application due to its efficient handling of static files. Furthermore, the usage of the Alpine Linux distribution for the Docker image underscores our commitment to minimizing resource usage and maximizing efficiency.
