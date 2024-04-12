# Use an official Python runtime as a parent image
FROM python:3.8-slim

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the Python script into the container
COPY hello_world.py .

# Install any necessary packages
# RUN pip install some-package  # Uncomment and replace if you need to install packages

# Create a non-root user with no password (username here is 'appuser')
RUN adduser --disabled-password --gecos '' appuser

# Switch to the non-root user
USER appuser

# Command to run the script
CMD ["python", "./hello_world.py"]

