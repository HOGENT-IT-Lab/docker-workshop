---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

![bg left:40% 80%](./img/logo.png)

# **Docker**

Slides voor Docker workshop van het IT-lab


---

![bg left:100% 80%](./img/docker-logo-blue.svg)

---


# Meevolgen op:

https://hogent-it-lab.github.io/docker-workshop/slides

![QR bg right contain](./img/link_qr.png)

---

# Wat is Docker?


- Virtualisatie op een ander niveau: containerisatie
- Gebruikt Linux kernel
- Opzetten (geïsoleerde) applicaties

---

# Docker versus virtuele machine

- Wat is nu eigenlijk het verschil met een virtuele machine (VM)?

  - Virtuele machine: emuleert volledige computer (virtuele hardware!)
  - Docker container: spreekt Linux-kernel aan die draait op een hostsysteem
---

# Bouwstenen van Docker

- Dockerfile
- Docker Image
- Docker Container


---

# Dockerfile

- Wat is een Dockerfile?

---

# Docker Image

- Wat is een Docker Image?
- Dockerhub!

---

# Docker Container

- Wat is een Docker container?

---

# Port bindings

- Elke container heeft een IP-adres (zelf ingesteld of automatisch toegewezen)
- Elke container zit in een (of meerdere) Docker netwerk (zelf ingesteld of automatisch toegewezen)
- Concept van port binding: een poort van een container koppelen aan een poort van het hostsysteem
---


# Port bindings - visueel


INSERT IMAGE THAT VISUALISES THIS!

---

# Docker installeren

- Algemene stappen (voor Linux)
- Voor deze demo: werken in een virtuele machine!
- Andere mogelijkheden: Docker Desktop en WSL (Opgelet!!)

---

# Docker gebruiken - commando's

- Beheren van containers!
- docker ps
- docker run
- docker stop
- docker rm
- docker rmi

---

# Docker gebruiken - commando's

- Extra's en handige zaken:
- docker exec -ti 
- docker system prune -a
- 

---

# Docker gebruiken - Docker Compose


- Docker run commando's: handig maar omslachtig...
- Wat met meerdere containers tegelijk opstarten?
- Oplossing: Docker Compose!


---

# Volume binding

- Mappen/bestanden van jouw Docker container binden aan het hostsysteem
- Nuttig voor data-persistentie
- Biedt mogelijkheden voor het maken van backups

---

# Docker demo - Minecraft server


- Eigen Minecraft server opstarten in een container
- Volume binding voor de data van de server
- Speel Minecraft op een server die je zelf in beheer hebt!

---

# Docker networking

- Standaard: Docker regelt vanalles zelf under the hood
- Je kan zelf (interne) Docker netwerken declareren
- Nut? Isolatie van netwerken, overzicht, veiligheid,...

---

# Nuttige links - Docker

- [Docker documentatie](https://docs.docker.com/)
- [Docker installatie](https://docs.docker.com/engine/install/)
- [Docker Compose documentatie](https://docs.docker.com/compose/)
- [Docker Networking documentatie](https://docs.docker.com/network/)

---

# Nuttige links - Docker

- [Composerize](https://composerize.com/) - `docker run` commando naar docker-compose
  
- [DockerHub](https://hub.docker.com/)
  
- [Docker cheat sheet](https://docs.docker.com/get-started/docker_cheatsheet.pdf)