# Docker version of PocketBase - backend for your next SasS and Mobile App

![GitHub release (latest by date)](https://img.shields.io/github/v/release/pocketbase/pocketbase?logo=github&logoColor=%23ffffff&style=for-the-badge)
![Docker Image Version (latest by date)](https://img.shields.io/docker/v/spectado/pocketbase?logo=docker&logoColor=%23ffffff&style=for-the-badge)
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/spectado/pocketbase/latest?logo=docker&logoColor=%23ffffff&style=for-the-badge)

## Supported Architectures

![Docker AMD64](https://img.shields.io/badge/amd64-grey?logo=&logoColor=%23ffffff&style=for-the-badge)
![Docker ARM64](https://img.shields.io/badge/arm64-grey?logo=&logoColor=%23ffffff&style=for-the-badge)
![Docker arm v7](https://img.shields.io/badge/arm%20v7-grey?logo=&logoColor=%23ffffff&style=for-the-badge)

Pulling `spectado/pocketbase:latest` will retrieve the correct image for your arch.

## Application Setup

Access the webui at `<your-ip>:80`, for more information check out [PocketBase](https://pocketbase.io/docs/).

## PocketBase

This docker image is a build of [pocketbase.io - Open Source backend for your next SaaS and Mobile app in 1 file](https://pocketbase.io)

- Realtime database
- Authentication
- File storage
- Admin dashboard

## Links

[![PocketBase GIT](https://img.shields.io/badge/github-grey?logo=github&logoColor=%23ffffff&style=for-the-badge)](https://github.com/pocketbase/pocketbase)
[![PocketBase WEB](https://img.shields.io/badge/web-grey?logo=&logoColor=%23ffffff&style=for-the-badge)](https://pocketbase.io)
[![PocketBase DOCS](https://img.shields.io/badge/documentation-blue?logo=markdown&logoColor=%23ffffff&style=for-the-badge)](https://pocketbase.io/docs/)

## Usage

**docker-compose**

```yml
version: "3.7"
services:
  pocketbase:
    image: spectado/pocketbase:latest
    container_name: pocketbase
    restart: unless-stopped
    ports:
      - "80:80"
    volumes:
      - /path/to/data:/pb_data
```
