# Spot in Deployment

## Clone the repository

In order to clone the repository, run the following command:

```bash
# Clone the repository
git clone https://github.com/spotin/spotin-deployment.git
```

## Start the applications

Check the following README for instructions on how to start the applications:

- [Spot in](spotin/README.md)
- [Traefik](traefik/README.md)

## Free up space

To free up space, you can delete the unused Docker containers and volumes with
the following command:

```bash
# Delete all the stopped containers and volumes
docker system prune --all
```

You can check the remaining disk space with the following command:

```bash
# Check the remaining disk space
df --human-readable
```
