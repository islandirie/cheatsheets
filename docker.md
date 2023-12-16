# Docker Cheatsheet

## 1. **Images**

### Pull an Image
```bash
docker pull image_name
```

### List Images
```bash
docker images
```

### Remove an Image
```bash
docker rmi image_name
```

## 2. **Containers**

### Run a Container
```bash
docker run image_name
```

### List Running Containers
```bash
docker ps
```

### List All Containers (including stopped ones)
```bash
docker ps -a
```

### Stop a Running Container
```bash
docker stop container_id
```

### Remove a Container
```bash
docker rm container_id
```

## 3. **Build and Customize Images**

### Build an Image from Dockerfile
```bash
docker build -t image_name .
```

### Build an Image with a Tag
```bash
docker build -t image_name:tag .
```

### Build with Build Args
```bash
docker build --build-arg key=value -t image_name .
```

## 4. **Volumes**

### Create a Volume
```bash
docker volume create volume_name
```

### List Volumes
```bash
docker volume ls
```

### Remove a Volume
```bash
docker volume rm volume_name
```

## 5. **Networks**

### Create a Network
```bash
docker network create network_name
```

### List Networks
```bash
docker network ls
```

### Remove a Network
```bash
docker network rm network_name
```

## 6. **Docker Compose**

### Run Docker Compose
```bash
docker-compose up
```

### Run Docker Compose in Detached Mode
```bash
docker-compose up -d
```

### Stop Docker Compose
```bash
docker-compose down
```

## 7. **Logs and Exec**

### View Container Logs
```bash
docker logs container_id
```

### Execute a Command in a Running Container
```bash
docker exec -it container_id command
```

## 8. **Miscellaneous**

### Docker Version
```bash
docker version
```

### Docker Info
```bash
docker info
```

### Cleanup (Remove All Containers and Images)
```bash
docker system prune -a
```

### PART 2

# Docker Cheatsheet

## 1. Images

- **Pull an Image:**
  `docker pull image_name`

- **List Images:**
  `docker images`

- **Remove an Image:**
  `docker rmi image_name`

## 2. Containers

- **Run a Container:**
  `docker run image_name`

- **List Running Containers:**
  `docker ps`

- **List All Containers (including stopped ones):**
  `docker ps -a`

- **Stop a Running Container:**
  `docker stop container_id`

- **Remove a Container:**
  `docker rm container_id`

## 3. Build and Customize Images

- **Build an Image from Dockerfile:**
  `docker build -t image_name .`

- **Build an Image with a Tag:**
  `docker build -t image_name:tag .`

## 4. Volumes

- **Create a Volume:**
  `docker volume create volume_name`

- **List Volumes:**
  `docker volume ls`

- **Remove a Volume:**
  `docker volume rm volume_name`

## 5. Networks

- **Create a Network:**
  `docker network create network_name`

- **List Networks:**
  `docker network ls`

- **Remove a Network:**
  `docker network rm network_name`

## 6. Docker Compose

- **Run Docker Compose:**
  `docker-compose up`

- **Run Docker Compose in Detached Mode:**
  `docker-compose up -d`

- **Stop Docker Compose:**
  `docker-compose down`

## 7. Logs and Exec

- **View Container Logs:**
  `docker logs container_id`

- **Execute a Command in a Running Container:**
  `docker exec -it container_id command`

## 8. Miscellaneous

- **Docker Version:**
  `docker version`

- **Docker Info:**
  `docker info`

- **Cleanup (Remove All Containers and Images):**
  `docker system prune -a`

