# Spring Boot with React Frontend

This repository contains a Spring Boot backend with a Java 17 runtime and a React frontend.

## Backend Setup

1. **Java 17**: Ensure you have Java 17 installed on your system. You can download it from [AdoptOpenJDK](https://adoptopenjdk.net/).

2. **Spring Boot**: Clone this repository and navigate to the backend directory:
3. **Run Spring Boot**: Use your preferred IDE or build tool to run the Spring Boot application.

## PostgreSQL 16.1 Docker Setup

This guide walks you through setting up PostgreSQL 16.1 using Docker on port 5435.

## Prerequisites

1. **Docker**: Install Docker on your system. You can download Docker Desktop from the [official Docker website](https://www.docker.com/products/docker-desktop).

## Setup Steps

1. **Pull PostgreSQL Image**: Open a terminal or command prompt and pull the PostgreSQL 16.1 image from Docker Hub:
   ```docker pull postgres:16.1```
2. **Create Docker Container**: Run the following command to create a Docker container named `postgres-16.1` using the pulled PostgreSQL image:
   ```docker run --name postgres-16.1 -p 5435:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres:16.1```
3. **Verify**: Check if the container is running by executing:```docker ps```
#### Explanation of the command:
- `--name postgres-16.1`: Sets the name of the container to `postgres-16.1`.
- `-p 5435:5432`: Maps port 5435 on the host to port 5432 inside the container.
- `-e POSTGRES_PASSWORD=mysecretpassword`: Sets the password for the PostgreSQL `postgres` user to `mysecretpassword`. You can change this password as needed.
- `-d`: Runs the container in detached mode (in the background).
- `postgres:16.1`: Specifies the PostgreSQL image and its version.

## Frontend Setup

1. **Node.js 22.1.0**: Ensure you have Node.js version 22.1.0 installed on your system. You can manage Node.js versions using tools like [nvm](https://github.com/nvm-sh/nvm) or [n](https://github.com/tj/n).

2. **React App**: Navigate to the frontend directory:
3. **Install Dependencies**: Run the following command to install dependencies:

4. **Run the React App**: Start the React development server:

This will start the development server at `http://localhost:3000/` by default.

## Contributing

Contributions are welcome! Please feel free to open issues or pull requests for any improvements or fixes.

## License

This project is licensed under the [MIT License](LICENSE).
