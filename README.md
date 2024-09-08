# Containerization of a Two-Tier Application using Docker

This project demonstrates the containerization of a two-tier application (front-end and back-end) using Docker. It includes a static website built with HTML, CSS, and JavaScript, and the application is served using an Nginx web server inside a Docker container.

## Project Structure
/my-project ├── Dockerfile ├── index.html ├── styles.css ├── app.js ├── pictures/ │ ├── image1.jpg │ └── image2.png └── README.md


- `index.html`: The main HTML file for the static website.
- `styles.css`: Contains the CSS styles for the website.
- `app.js`: JavaScript file for dynamic content on the site.
- `pictures/`: Contains images used in the website.
- `Dockerfile`: The configuration file to create a Docker image of the static site.
- `README.md`: Documentation of the project.

## Prerequisites

Before running this project, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)

## Docker Setup

### 1. Build the Docker Image

To build the Docker image for the static website, navigate to the project directory and run:

docker build -t static-website .

### 2. Run the Docker Container
Once the image is built, run the Docker container by exposing it on port 8080:

docker run -p 8080:80 static-website

You can now access the website at http://localhost:8080 in your web browser.

## Technologies Used

#### HTML5: Markup for creating the structure of the website.
#### CSS3: Styling for the website.
#### JavaScript: Adds dynamic behavior to the website.
#### Docker: Used to containerize the application for portability and ease of deployment.
#### Nginx: A web server used to serve static files inside the Docker container.

## Features
#### Responsive and clean static website.
#### Easy deployment using Docker.
#### Containerized two-tier architecture using Docker and Nginx.

