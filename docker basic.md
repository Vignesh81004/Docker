
This will show you how Docker runs a **web server inside a container**.

---

# Step 1 — Pull the Nginx Image

Run this command:

```bash
docker pull nginx
```

What happens:

1. Docker downloads the **nginx image** from
   Docker Hub
2. The image is stored on your system.

Check it:

```bash
docker images
```

You should see:

```
REPOSITORY   TAG       IMAGE ID
nginx        latest
```

---

# Step 2 — Run the Nginx Container

Now start the container.

```bash
docker run -d -p 8080:80 nginx
```

Explanation:

```
-d       → run in background
-p       → port mapping
8080     → your computer port
80       → nginx container port
```

---

# Step 3 — Check Running Containers

```bash
docker ps
```

You should see something like:

```
CONTAINER ID   IMAGE   STATUS
8ab12c         nginx   Up
```

This means your **container is running**.

---

# Step 4 — Test in Browser

Open browser and go to:

```
http://localhost:8080
```

You should see the **Nginx welcome page**.

This means:

```
Your Laptop
     ↓
Docker
     ↓
Nginx Container
     ↓
Website Running
```

---

# Step 5 — View Logs

Check container logs:

```bash
docker logs <container-id>
```

Example:

```bash
docker logs 8ab12c
```

This shows web server logs.

---

# Step 6 — Enter the Container

```bash
docker exec -it <container-id> bash
```

Now you are **inside the nginx container**.

Try:

```bash
ls
cd /usr/share/nginx/html
ls
```

You will see the **default website files**.

Exit container:

```
exit
```

---

# Step 7 — Stop the Container

```bash
docker stop <container-id>
```

---

# Step 8 — Remove Container

```bash
docker rm <container-id>
```

---

# What You Just Learned

With this one example you practiced:

```
docker pull
docker run
docker ps
docker logs
docker exec
docker stop
docker rm
```

These are the **most used Docker commands**.

