Here are the **MOST IMPORTANT Docker basic commands** you must know as a beginner 👍
I’ll give **command + meaning + example**, very simple.

---

# 🐳 Docker Basic Commands (Beginner Friendly)

---

## 1️⃣ Check Docker installation

```bash
docker --version
```

👉 Confirms Docker is installed

---

## 2️⃣ Download an image (pull)

```bash
docker pull ubuntu
```

👉 Downloads the **ubuntu image**
👉 Image is **not running**

---

## 3️⃣ List Docker images

```bash
docker images
```

👉 Shows all downloaded images

---

## 4️⃣ Run a container

```bash
docker run ubuntu
```

👉 Creates + starts a container
👉 Runs default command and exits

---

## 5️⃣ Run container with interactive shell (MOST USED)

```bash
docker run -it ubuntu bash
```

👉 `-i` = interactive
👉 `-t` = terminal
👉 You enter the container shell

---

## 6️⃣ Exit container

```bash
exit
```

👉 Container stops

---

## 7️⃣ List running containers

```bash
docker ps
```

---

## 8️⃣ List all containers (running + stopped)

```bash
docker ps -a
```

---

## 9️⃣ Stop a running container

```bash
docker stop <container_id>
```

Example:

```bash
docker stop a1b2c3d4
```

---

## 🔟 Start a stopped container

```bash
docker start <container_id>
```

---

## 1️⃣1️⃣ Restart a container

```bash
docker restart <container_id>
```

---

## 1️⃣2️⃣ Remove a container

```bash
docker rm <container_id>
```

👉 Container must be stopped

Force remove:

```bash
docker rm -f <container_id>
```

---

## 1️⃣3️⃣ Remove an image

```bash
docker rmi ubuntu
```

👉 Image must not be used by containers

---

## 1️⃣4️⃣ Run container in background (detached)

```bash
docker run -d nginx
```

👉 Runs in background

---

## 1️⃣5️⃣ View container logs

```bash
docker logs <container_id>
```

---

## 1️⃣6️⃣ Enter running container

```bash
docker exec -it <container_id> bash
```

👉 Like `ssh` into container

---

## 1️⃣7️⃣ Remove ALL stopped containers

```bash
docker container prune
```

---

## 🧠 Most Important Commands (Remember these first)

```bash
docker images
docker ps
docker ps -a
docker run -it ubuntu bash
docker stop
docker rm
docker rmi
docker exec -it
```

---

## 🧪 Simple Practice Task (DO THIS)

```bash
docker pull ubuntu
docker run -it ubuntu bash
ls
exit
docker ps -a
docker rm <container_id>
```

---

## 🧠 Easy Memory Trick

* **Image** → `docker images`
* **Run** → `docker run`
* **See containers** → `docker ps`
* **Delete** → `docker rm / rmi`

---

If you want next, I can:

* Explain **docker run command options**
* Teach **Dockerfile**
* Explain **ports & volumes**
* Give **daily Docker practice**

Just tell me 👍
