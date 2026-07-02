# First Dockerfile Example

This repository contains a simple Docker example that demonstrates how to containerize a basic Python application using Docker.

## Project Structure

```
.
├── app.py
└── first-docker-file
    ├── app.py
    └── Dockerfile
```

## Prerequisites

* Docker installed on your system

## Build the Docker Image

Navigate to the project directory containing the `Dockerfile` and run:

```bash
docker build -t first-docker-example .
```

## Run the Docker Container

```bash
docker run first-docker-example
```

## Expected Output

```text
Hello-world
```

## Dockerfile Overview

* Uses the latest Ubuntu image as the base image.
* Sets `/app` as the working directory.
* Copies the project files into the container.
* Installs Python 3 and pip.
* Sets an environment variable:

  * `NAME=World`
* Runs the Python application using:

```bash
python3 app.py
```

## Learning Objectives

This project helped me understand:

* Creating a Dockerfile
* Using a base image
* Setting the working directory with `WORKDIR`
* Copying files using `COPY`
* Installing packages with `RUN`
* Defining environment variables with `ENV`
* Running an application using `CMD`
