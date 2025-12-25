# CTF Challenge - 4 Flags

A multi-stage Capture The Flag challenge focusing on web exploitation, privilege escalation, and binary exploitation.

## Prerequisites

You need Docker and Docker Compose installed on your system.

### Install Docker

**Windows/Mac:**
- Download Docker Desktop from https://www.docker.com/products/docker-desktop
- Install and start Docker Desktop

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install docker.io docker-compose
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
```

After installation, log out and back in (or run `newgrp docker`).

## Setup

1. **Extract the files:**
```bash
unzip files.zip
cd files
```

2. **Build and start the challenge:**
```
docker compose up -d --build
```

Wait a few minutes for the build to complete.

3. **Verify it's running:**
```
docker ps
```

You should see a container named `ctf_challenge` running.


## Your Mission

Find and capture all 4 flags in this format:
- `flag{format}`



## Stopping the Challenge

```
docker compose down
```

## Troubleshooting

**Container won't start:**
```
docker compose down
docker compose up -d --build
```


**Reset everything:**
```
docker compose down -v
docker compose up -d --build
```



This is a self-contained CTF challenge. Use your penetration testing skills and tools to find the flags!

Good luck! 🚀
