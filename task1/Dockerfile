# Use the latest Ubuntu base image
FROM ubuntu:latest

# Update package list and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove externally managed file to avoid installation issues
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy the Flask application file
COPY ./api.py /app/api.py

# Expose port 5252
EXPOSE 5252

# Command to run the Flask application
CMD ["python3", "api.py"]
