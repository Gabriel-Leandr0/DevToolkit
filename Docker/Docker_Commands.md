# Docker

### Building image:
docker build -f src/main/docker/Dockerfile.jvm -t gabrielmgr/helpgr:1.0 .

---

### Running image:

**Only image:**
docker run --name db-helpgr -p 27017:27017 mongo

**Creating network and running image:**
docker run --name helpgr --network rede-gr -p 8080:8080 gabrielmgr/helpgr:1.0

---

### Running my Quarkus application :

docker run --name db-helpgr --network rede-gr -p 27017:27017 mongo

docker run --name helpgr --network rede-gr -p 8080:8080 gabrielmgr/helpgr:1.0


