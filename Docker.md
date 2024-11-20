# Docker Commands Cheat Sheet

This document serves as a cheat sheet for common Docker commands.

| **Action**                                          | **Command**                                           |
| --------------------------------------------------- | ----------------------------------------------------- |
| **Install Docker (Ubuntu)**                         | `sudo apt update && sudo apt install docker.io`       |
| **Install Docker (CentOS)**                         | `sudo yum install docker`                             |
| **Start Docker**                                    | `sudo systemctl start docker`                         |
| **Stop Docker**                                     | `sudo systemctl stop docker`                          |
| **Restart Docker**                                  | `sudo systemctl restart docker`                       |
| **Check Docker status**                             | `sudo systemctl status docker`                        |
| **List running containers**                         | `docker ps`                                           |
| **List all containers**                             | `docker ps -a`                                        |
| **Run a new container**                             | `docker run <image_name>`                              |
| **Run a container in detached mode**                | `docker run -d <image_name>`                           |
| **Stop a running container**                        | `docker stop <container_id>`                           |
| **Remove a container**                              | `docker rm <container_id>`                             |
| **Remove all stopped containers**                   | `docker container prune`                              |
| **Execute a command inside a running container**    | `docker exec -it <container_id> <command>`             |
| **List images**                                     | `docker images`                                       |
| **Pull an image from Docker Hub**                   | `docker pull <image_name>`                             |
| **Build an image from a Dockerfile**                | `docker build -t <image_name>:<tag> <path>`            |
| **Remove an image**                                 | `docker rmi <image_name>`                              |
| **Remove unused images**                            | `docker image prune`                                   |
| **List volumes**                                    | `docker volume ls`                                     |
| **Create a volume**                                 | `docker volume create <volume_name>`                   |
| **Remove a volume**                                 | `docker volume rm <volume_name>`                       |
| **Remove unused volumes**                           | `docker volume prune`                                  |
| **List networks**                                   | `docker network ls`                                    |
| **Create a network**                                | `docker network create <network_name>`                 |
| **Remove a network**                                | `docker network rm <network_name>`                     |
| **Start services with Docker Compose**              | `docker-compose up`                                    |
| **Start services in detached mode**                 | `docker-compose up -d`                                |
| **Stop services**                                   | `docker-compose down`                                  |
| **View logs**                                       | `docker-compose logs`                                  |

### Useful Flags:
- `-it` (Interactive terminal)
- `--rm` (Remove container after exit)
- `-p <host_port>:<container_port>` (Map ports)

For more detailed information, please refer to the official [Docker Documentation](https://docs.docker.com/).
