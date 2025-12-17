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


Perfect 👍
Below are **MORE BASIC & IMPORTANT Docker commands** that beginners usually miss, but **real DevOps engineers use daily**.
I’ll keep it **simple + practical**, no overload.

---

# 🐳 More Important Docker Commands (Beginner → Intermediate)

---

## 🔍 1️⃣ Search images on Docker Hub

```bash
docker search nginx
```

👉 Find images from Docker Hub

---

## ℹ️ 2️⃣ Inspect image or container (VERY IMPORTANT)

```bash
docker inspect ubuntu
docker inspect <container_id>
```

👉 Shows full details (JSON): IP, mounts, config

---

## 📊 3️⃣ See container resource usage

```bash
docker stats
```

👉 CPU, memory, network usage (like `top`)

---

## 🧹 4️⃣ Remove unused data (CLEANUP)

```bash
docker system prune
```

👉 Removes:

* stopped containers
* unused images
* unused networks

⚠️ Careful in production

---

## 📁 5️⃣ Copy files between host ↔ container

```bash
docker cp file.txt <container_id>:/tmp/
docker cp <container_id>:/tmp/file.txt .
```

---

## 🧾 6️⃣ Show container logs (follow mode)

```bash
docker logs -f <container_id>
```

👉 Like `tail -f`

---

## 🧠 7️⃣ Show image build history

```bash
docker history ubuntu
```

👉 See how image was built

---

## 🧪 8️⃣ Test image without running shell

```bash
docker run ubuntu echo "Hello Docker"
```

---

## 🔄 9️⃣ Rename a container

```bash
docker rename old_name new_name
```

---

## 🏷️ 🔟 Name a container while running (BEST PRACTICE)

```bash
docker run --name myubuntu -it ubuntu bash
```

👉 Easier than container ID

---

## 🌐 1️⃣1️⃣ List Docker networks

```bash
docker network ls
```

---

## 🔌 1️⃣2️⃣ Inspect Docker network

```bash
docker network inspect bridge
```

---

## 📦 1️⃣3️⃣ List Docker volumes

```bash
docker volume ls
```

---

## 📂 1️⃣4️⃣ Inspect volume

```bash
docker volume inspect <volume_name>
```

---

## 🧠 1️⃣5️⃣ Show Docker disk usage

```bash
docker system df
```

👉 How much space Docker uses

---

## 🛑 1️⃣6️⃣ Kill a container (force stop)

```bash
docker kill <container_id>
```

👉 Like `kill -9`

---

## 🔁 1️⃣7️⃣ Pause & unpause container

```bash
docker pause <container_id>
docker unpause <container_id>
```

---

## 🔐 1️⃣8️⃣ Login to Docker Hub

```bash
docker login
```

---

## 📤 1️⃣9️⃣ Push image to Docker Hub

```bash
docker push username/image_name
```

👉 After tagging

---

## 🏷️ 2️⃣0️⃣ Tag an image

```bash
docker tag ubuntu myubuntu:v1
```

---

## 🧠 Most Used in Real Life (Focus on these)

```bash
docker exec -it
docker logs -f
docker inspect
docker stats
docker system prune
docker network ls
docker volume ls
```

---

## 🧪 Practice Task (Recommended)

```bash
docker run --name test -d nginx
docker ps
docker logs test
docker inspect test
docker stats
docker stop test
docker rm test
```

---

## 🧠 Easy Remember Rule

* **Debug** → `logs`, `inspect`, `stats`
* **Cleanup** → `prune`
* **Data** → `volume`
* **Network** → `network`

---

If you want next, I can:

* Explain **docker run flags deeply**
* Teach **volumes with example**
* Explain **port mapping**
* Start **Dockerfile**

Just tell me 👍

