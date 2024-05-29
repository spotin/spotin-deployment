# Traefik

> Traefik is the leading open-source reverse proxy and load balancer for HTTP
> and TCP-based applications that is easy, dynamic and full-featured.
>
> <https://traefik.io/traefik/>

## Prerequisites

The following prerequisites must be filled to run this service:

- [Docker](https://docs.docker.com/get-docker/) must be installed.
- [Docker Compose](https://docs.docker.com/compose/install/) must be installed
  (it should be installed by default with Docker in most cases).

## Set the environment variables

Edit the `*.env` files to your needs.

You can now start the application with Docker.

## Run the application with Docker

Do not forget to set the environment variables as described in the previous
section.

In a terminal, run the following commands:

```bash
# Pull the latest images
docker compose pull

# Start the application with Docker
docker compose up --detach
```
