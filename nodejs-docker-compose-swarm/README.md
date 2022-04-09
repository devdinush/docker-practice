## Scaling Docker using Docker + Docker-compose + Docker Swarm

### Build Image
    
```bash
docker-compose build
```

### Initialize the Swarm

```bash
docker swarm init
```

### Create Service

```bash
docker stack deploy -c docker-compose.yml nodejs-docker-compose-swarm
```

### Check Service list

    
```bash
docker service ls\
```

### Scaling the Service

```bash
docker service scale nodejs-docker-compose-swarm=20
```
### Delete the Service

```bash
docker service rm <service_id>
```