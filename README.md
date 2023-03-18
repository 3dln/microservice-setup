# My Platform

This setup is using Next.js for the frontend, Node.js with Express.js for the backend, and TypeScript with Yarn for package management. The project utilizes Docker for containerization and includes services like Redis, RabbitMQ, and NGINX.

## Table of Contents

- [My Platform](#my-platform)
  - [Table of Contents](#table-of-contents)
  - [Requirements](#requirements)
  - [Setup](#setup)
    - [Project Structure](#project-structure)
    - [Frontend and Backend with TypeScript and Yarn](#frontend-and-backend-with-typescript-and-yarn)
    - [Dockerfiles for Frontend and Backend](#dockerfiles-for-frontend-and-backend)
    - [Docker Compose for Services](#docker-compose-for-services)
  - [Running the Platform](#running-the-platform)

## Requirements

- Node.js
- Yarn
- Docker
- Docker Compose v2

## Setup

### Project Structure

Create a root directory for the entire project and separate subdirectories for the frontend and backend projects.

```console
mkdir my-platform
cd my-platform
mkdir frontend backend
```

### Frontend and Backend with TypeScript and Yarn

Set up the frontend project using Next.js and TypeScript, and the backend project using Node.js, Express.js, and TypeScript. Use Yarn as the package manager.

Detailed instructions can be found [here](#frontend-and-backend-with-typescript-and-yarn).

### Dockerfiles for Frontend and Backend

Create `Dockerfile`s for both the frontend and backend projects.

Detailed instructions can be found [here](#dockerfiles-for-frontend-and-backend).

### Docker Compose for Services

Create a `docker-compose.yml` file to manage all the services, including Redis, RabbitMQ, and NGINX. Create an `nginx.conf` file for the NGINX configuration.

Detailed instructions can be found [here](#docker-compose-for-services).

## Running the Platform

To start all services using Docker Compose v2, run the following command in the root directory of your project:

```console
docker compose up
```

The platform will be accessible at:

- Frontend: `http://localhost`
- Backend: `http://localhost/api`
