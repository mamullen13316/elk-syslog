# Docker Compose for ELK Stack

## Usage
```bash
docker compose up
```
Once all containers are up, run setup on the `filebeat` container:
```bash
docker exec $(docker ps -q -f 'name=filebeat') filebeat setup
```
This will take a few minutes.  