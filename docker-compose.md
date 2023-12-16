# Docker Compose Cheatsheet

## 1. Basics

- **Define Services in `docker-compose.yml`:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
  ```

- **Run Docker Compose:**
  `docker-compose up`

- **Run Docker Compose in Detached Mode:**
  `docker-compose up -d`

- **Stop Docker Compose:**
  `docker-compose down`

## 2. Services

- **Scale Services:**
  `docker-compose up --scale service_name=3`

- **Build and Run Services:**
  `docker-compose up --build`

- **Run a Single Service:**
  `docker-compose up service_name`

## 3. Environment Variables

- **Set Environment Variables in `docker-compose.yml`:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      environment:
        - KEY=value
  ```

## 4. Networking

- **Expose Ports:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      ports:
        - "80:8080"
  ```

- **Use External Networks:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      networks:
        - external_network
  networks:
    external_network:
      external: true
  ```

## 5. Volumes

- **Mount Volumes:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      volumes:
        - /path/on/host:/path/in/container
  ```

- **Use Named Volumes:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      volumes:
        - volume_name:/path/in/container
  volumes:
    volume_name:
  ```

## 6. Dependencies

- **Wait for Dependencies:**
  ```yaml
  version: '3'
  services:
    service_name:
      image: image_name
      depends_on:
        - dependency_service
  ```
