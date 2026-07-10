# 🐳 Day 18 – Docker Images & Containers

## 📖 Overview

Today, I learned about Docker Images and Containers in detail. I understood Docker Architecture, Container Lifecycle, and how Docker creates and manages containers from images.

---

# 📚 Topics Covered

## 🏗️ Docker Architecture

```text
Developer
      │
Docker CLI
      │
Docker Daemon
      │
Local Image Check
      │
Docker Hub (If Image Not Available)
      │
Image Download
      │
Container Creation
      │
Application Output
```

---

## 🖼️ Docker Images

A Docker Image is a lightweight, read-only template containing:

- Application Code
- Runtime
- Libraries
- Dependencies
- Configuration Files

### Commands Practiced

```bash
docker images
docker image ls
docker pull ubuntu
```

---

## 📦 Docker Containers

A Container is a running instance of a Docker Image.

### Workflow

```text
Docker Image
      │
docker run
      │
Docker Container
      │
Running Application
```

One Docker Image can create multiple Containers.

---

# 🔄 Container Lifecycle

```text
Image
   │
docker run
   │
Running
   │
docker stop
   │
Stopped
   │
docker start
   │
Running
   │
docker rm
   │
Deleted
```

### Commands Practiced

```bash
docker ps
docker ps -a
docker stop
docker start
docker restart
docker rm
```

---

# 📌 Important Concepts Learned

## docker ps vs docker ps -a

### docker ps

Displays only Running Containers.

### docker ps -a

Displays all Containers (Running + Stopped).

---

## Exited (0)

```text
STATUS: Exited (0)
```

Meaning:

- Container executed successfully.
- Program completed normally.
- Exit Code `0` = Success.

---

## Image vs Container

| Docker Image | Docker Container |
|--------------|------------------|
| Blueprint | Running Instance |
| Static | Dynamic |
| Read-only | Executable |
| Can create multiple containers | Runs the application |

---

# 🧪 Ubuntu Container Lab

### Commands

```bash
docker pull ubuntu

docker run -it ubuntu bash
```

### Commands Practiced Inside Container

```bash
pwd
ls
whoami
mkdir devops
cd devops
touch test.txt
cat /etc/os-release
exit
```

---

# 🎯 Key Learning

Docker first checks whether an Image exists locally.

If the Image is not available:

Docker → Docker Hub → Download Image → Create Container → Run

If the Image already exists:

Docker directly creates a new Container without downloading the Image again.

---

# 💻 Commands Practiced Today

```bash
docker images
docker image ls
docker pull ubuntu
docker run
docker ps
docker ps -a
docker stop
docker start
docker restart
docker rm
docker run -it ubuntu bash
```

---

# 🚀 Outcome

Today I learned:

✅ Docker Architecture  
✅ Docker Images  
✅ Docker Containers  
✅ Container Lifecycle  
✅ docker ps vs docker ps -a  
✅ Exited (0) Meaning  
✅ Ubuntu Container Basics  
✅ One Image → Multiple Containers Concept

This knowledge forms the foundation of Containerization and DevOps workflows.

---

## 🔥 Next Step

➡️ Day 19 – Dockerfile & Custom Images

Topics:

- Dockerfile
- docker build
- docker exec
- docker logs
- docker inspect
- Build Your Own Docker Image

#Docker #DevOps #Containers #Linux #DockerHub #Cloud #LearningInPublic
