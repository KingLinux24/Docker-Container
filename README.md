````markdown
````
---
# Docker Assignment - Cloud Computing

This repository contains my solutions for **Assignment 3: Docker-Container**  
for the course *Cloud Computing* (Semester V, B.Tech CSE Cyber-Security).  

---
## Task 1: Pull the Alpine image from Docker Hub
````bash
docker pull alpine
docker images
````

---

## Task 2: Build an image from a Dockerfile

Create a `Dockerfile`:

```dockerfile
FROM alpine
CMD ["echo", "Hello from my custom Dockerfile!"]
```

Build the image:

```bash
docker build -t custom-alpine .
docker images
```

---

## Task 3: Create an image with my name and push to Docker Hub

```bash
docker tag custom-alpine israeldavid/custom-alpine:v1
docker login
docker push israeldavid/custom-alpine:v1
```

---

## Task 4: List all Docker containers

```bash
docker ps -a
```

---

## Task 5: Get Docker system information

```bash
docker info
```

---

## Task 6: List all Docker images

```bash
docker images
```

---

## Task 7: Write a simple Python program to print N numbers

File: `numbers.py`

```python
N = int(input("Enter a number: "))
for i in range(1, N+1):
    print(i)
```

Run it:

```bash
python3 numbers.py
```

---

## Task 8: Search for a Docker image with my name

```bash
docker search israeldavid
```

---

## Task 9: Create and run an Nginx container

```bash
docker pull nginx
docker run -d -p 8080:80 nginx
```

Open browser: `http://localhost:8080`

---

## Task 10: Automated Pentesting Docker Image

Pull and run the image (example):

```bash
docker pull <github-image-link>
docker run -it <image-name>
```

Generated report is saved as `PentestReport.pdf`.

---

## Technologies Used

* Docker
* Python
* Nginx
* Kali Linux

## Author

**Israel Mbiyavanga David**
B.Tech CSE (Cyber-Security) | Semester V

```

👉 Do you want me to **write this full README.md file ready for upload** to your GitHub repo, or would you like me to also **add the Dockerfiles and Python scripts** so you can upload them along with it?
```
