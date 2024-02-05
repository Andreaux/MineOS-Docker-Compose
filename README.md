Version: 1.0

# MineOS-Docker-Compose
A Simple Docker Compose File to run MineOS (the Minecraft server manager). It contains Traefik labels that go with my Traefik installation to provide wildcard SSL certificates to internal Homelab services through Cloudflare at https://github.com/Andreaux/Traefik-Docker-Compose
This file is set up the way it works for my Home Lab. Feel free to modify it to fit your purpose.

# How to use this package?
1. Set up Traefik and Cloudflare (not part of this package. See: https://github.com/Andreaux/Traefik-Docker-Compose)
2. Modify the .env file (or set up the same environment variables if you're using a package manager like Portainer for example).
3. Create a folder for the persistent data somewhere and share it with NFS (optional).
4. Edit the docker-compose.yml file to mount the NFS share you created into the container (top of the file) or, if it's a local folder, you can remove the share info at the top of the docker-compose.yml file and modify the volume definition.
5. Create and launch MineOS with docker-compose up -d

Everything should "just work".

# Support this project
If you find this useful, a coffee through Ko-Fi is all it takes to make me happy <3 (I love coffee :D) Click the Sponsor button on the top of this page or visit https://ko-fi.com/andreaux to buy me a coffee.
