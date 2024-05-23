FROM ubuntu:latest

# Update apt and install necessary packages
RUN apt-get update && \
    apt-get install -y \
    python3 \
    ssh \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Expose SSH port
EXPOSE 22
