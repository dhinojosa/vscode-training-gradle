# Specifies the docker base image you want to use
FROM mcr.microsoft.com/vscode/devcontainers/java:17

# Install Gradle inside the Docker container
RUN apt-get update && apt-get -y install gradle

# Sets the Docker container working directory
WORKDIR /workspace

# Copies your existing source code from your local system into the Docker container
COPY . ./

# Run Maven test
CMD ["gradle", "test"]
