# Use an official Python runtime as a base image
FROM python:3.6-slim

MAINTAINER @sparky_005

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt
RUN python -m nltk.downloader stopwords
RUN python -m nltk.downloader twitter_samples

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World 
ENTRYPOINT []
CMD ["/bin/bash"]
