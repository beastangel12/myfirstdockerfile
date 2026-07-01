FROM ubuntu:latest

# Set the working directory in the image
# working directory is nth but on the docker container you are using the CD command and you are moving to slash app folder and Used the work directory for basically telling my Docker image that every action that I perfrom shouldbe on this specific folder.

WORKDIR /app

# Copy the files from the host file system to the image file system.
# Copying the whole in the current diretory in /app 
COPY . /app

# Install the necessary packages
RUN apt update && apt install -y python3 python3-pip

# Set environment variables
ENV NAME=World

# Run a command to start the application
CMD ["python3", "app.py"]
