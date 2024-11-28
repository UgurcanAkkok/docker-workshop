# Docker Workshop

## Dockerhub

We can find and pull images using [docker hub](https://hub.docker.com/). It is the default image registry managed by the Docker.

## Dockerfile and Docker build

We will use a simple python app to build a docker container.
- Change directory into `step1/`
- Build a docker container image.
    ```bash
    docker build -t workshop:step1 .
    ```
- Run the container image.
    ```bash
    docker run -p 5000:5000 workshop:step1
    ```
- Open the web page in browser: http://127.0.0.1:5000

## Docker Compose

What if we need more containers?
- Change directory into `step2/`
- Build and run the containers using docker compose
    ```bash
    docker compose up --build
    ```
- Open the web page in browser: http://127.0.0.1:5000
