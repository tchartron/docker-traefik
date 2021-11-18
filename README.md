# traefik-2

Main traefik proxy routing to all docker stacks on a machine using docker and file providers.  
Handles letsencrypt TLS certificates.  
Includes a portainer container for a nice optionnal GUI  

## Setup
```bash
git clone git@github.com:tchartron/docker-traefik.git
cd docker-traefik && touch letsencrypt/acme.json
chmod 600 letsencrypt/acme.json
cp .env.example .env #and change values
docker-compose up -d
