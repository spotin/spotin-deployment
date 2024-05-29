# Spot in deployment

## Start the application for production mode

### Prerequisites

The following prerequisites must be filled to run this service:

- [Docker](https://docs.docker.com/get-docker/) must be installed.
- [Docker Compose](https://docs.docker.com/compose/install/) must be installed
  (it should be installed by default with Docker in most cases).

### Set the environment variables

Edit the `*.env` files to your needs.

You can now start the application in staging or production modes:

- [Staging mode](#run-the-application-in-staging-mode-with-docker)
- [Production mode](#run-the-application-in-production-mode-with-docker)

### Run the application in staging mode with Docker

Do not forget to set the environment variables as described in the previous
section.

In a terminal, run the following commands:

```bash
# Copy the override file for the staging environment
cp docker-compose.override.staging.yaml docker-compose.override.yaml

# Pull the latest images
docker compose pull

# Start the application with Docker
docker compose up --detach

# Optional: seed the database with some data
docker compose exec spotin npm run prisma:seed
```

### Run the application in production mode with Docker

Do not forget to set the environment variables as described in the previous
section.

In a terminal, run the following commands:

```bash
# Pull the latest images
docker compose pull

# Start the application with Docker
docker compose up --detach

# Optional: seed the database with some data
docker compose exec spotin npm run prisma:seed
```
