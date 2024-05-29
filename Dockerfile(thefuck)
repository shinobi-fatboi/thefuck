# Use the official Python image from the Docker Hub
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /usr/src/thefuck

# Clone the repository from GitHub
RUN apt-get update && apt-get install -y git \
    && git clone https://github.com/nvbn/thefuck.git .

# Install the application
RUN python setup.py install

# Set the entrypoint for the application
ENTRYPOINT ["thefuck"]
