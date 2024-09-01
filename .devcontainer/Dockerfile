# Use the official Ubuntu image as a base
FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && \
    apt-get install -y curl gnupg && \
    curl -fsSL https://code-server.dev/install.sh | sh

# Set environment variables
ENV PASSWORD=yourpassword

# Expose the port code-server will run on
EXPOSE 8080

# Start code-server
CMD ["code-server", "--host", "0.0.0.0", "--port", "8080"]
