# 📦 bane-nor Base Images  
This repository hosts and maintains a collection of standardized base container images to streamline and unify the development and deployment processes at **Bane NOR**. These images are built and published to **GitHub Container Registry (GHCR)** and are optimized for various languages and runtimes.

Each base image includes essential tools, security patches, and configurations that align with Bane NOR's internal requirements for production-grade applications. Below is a list of the available images and their descriptions.

---

## 🚀 Available Base Images

### 1. **Base**  
**Image**: [`ghcr.io/bane-nor/base`](https://github.com/bane-nor/base)  
![Base](https://github.com/bane-nor/base/actions/workflows/docker-image.yml/badge.svg)  
A minimal base image used as a foundation for other container images. This image contains only essential packages and tools. Based on Alpine Linux to provide low CVE footprint. 

---

### 2. **Dotnet**  
**Image**: [`ghcr.io/bane-nor/dotnet`](https://github.com/bane-nor/dotnet)  
![Dotnet](https://github.com/bane-nor/dotnet/actions/workflows/docker-image.yml/badge.svg)  
A base image for .NET applications, preconfigured with commonly used dependencies and optimized for faster builds and deployments. 3 latest supported versions of the .NET runtime and sdk maintained as tags. 

---

### 3. **Node**  
**Image**: [`ghcr.io/bane-nor/node`](https://github.com/bane-nor/node)  
![Node](https://github.com/bane-nor/node/actions/workflows/docker-image.yml/badge.svg)  
A Node.js base image for building and running JavaScript/TypeScript applications. It includes common packages and tools for web development.

---

### 4. **Python**  
**Image**: [`ghcr.io/bane-nor/python`](https://github.com/bane-nor/python)  
![Python](https://github.com/bane-nor/python/actions/workflows/docker-image.yml/badge.svg)  
A Python base image for data processing, scripting, and backend services. Includes pip and common Python libraries. Includes the 3 latest minor versions of Python 3

---

### 5. **Nutils (Network Tools)**  
**Image**: [`ghcr.io/bane-nor/nutils`](https://github.com/bane-nor/nutils)  
![Network Tools](https://github.com/Bane-NOR/nutils/actions/workflows/docker-image.yml/badge.svg)  
A utility image for network operations and diagnostics. Contains tools like `curl`, `wget`, `netcat`, and more for debugging and network analysis.

---

### 6. **Bun**  
**Image**: [`ghcr.io/bane-nor/bun`](https://github.com/bane-nor/bun)  
![Container Build](https://github.com/Bane-NOR/bun/actions/workflows/docker-image.yml/badge.svg)  
A base image for running and building apps using [Bun](https://bun.sh/), a fast JavaScript runtime. Ideal for rapid development of modern web applications. 

!!!note "Bun has some issues on HTTP2, we advise using node until further stability is ensured" 

---

### 7. **Nginx**  
**Image**: [`ghcr.io/bane-nor/nginx`](https://github.com/bane-nor/nginx)  
![Image Build](https://github.com/bane-nor/node/actions/workflows/docker-image.yml/badge.svg)  
An optimized Nginx image for serving static content and reverse proxying. Includes security enhancements and preconfigured settings for common use cases.

---

### 8. **Go**  
**Image**: [`ghcr.io/bane-nor/golang`](https://github.com/bane-nor/golang)  
[![Container Build](https://github.com/Bane-NOR/golang/actions/workflows/docker-image.yml/badge.svg?branch=main)](https://github.com/Bane-NOR/golang/actions/workflows/docker-image.yml)
A base image for running build apps using [Go](https://go.dev/), Go (golang) is a general purpose, higher-level, imperative programming language.


---

## 📘 How to Use  
To pull an image, use the following command:  
```bash
docker pull ghcr.io/bane-nor/<image-name>:<tag>
```

### Example: Pull the Python image  
```bash
docker pull ghcr.io/bane-nor/python:3.12
```

---

## 🛠️ CI/CD Status  
All images are continuously built and tested using GitHub Actions to ensure stability and security. Check individual badges for the current build status.

---

## 📄 License  
These images are provided under the **MIT License**. Please check individual repositories for specific details.

---

