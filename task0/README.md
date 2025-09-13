# Docker Task 0

## Dockerfile Content
FROM ubuntu:latest
RUN apt-get update
RUN apt-get upgrade -y
CMD ["echo", "Hello, World!"]

text

## Purpose
- Uses Ubuntu latest as base image
- Updates APT package list
- Upgrades installed packages
- Outputs "Hello, World!" when run

## Build Command
`docker build -t softy-pinko:task0 .`

## Run Command  
`docker run --rm softy-pinko:task0`

## Expected Output
`Hello, World!`
EOF
