# Task 0: Docker Hello World

## Description
This project creates a Docker image based on Ubuntu that updates packages, upgrades software, and outputs "Hello, World!" when run.

## Dockerfile
```dockerfile
# Use the latest Ubuntu as base image
FROM ubuntu:latest

# Update APT package list
RUN apt-get update

# Upgrade installed packages (with -y to auto-confirm)
RUN apt-get upgrade -y

# Set the default command to echo "Hello, World!"
CMD ["echo", "Hello, World!"]
