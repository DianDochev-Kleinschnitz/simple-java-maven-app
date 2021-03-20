# simple-java-maven-app

# demo

Build Anstossen:
```bash
curl -s http://localhost:8080/git/notifyCommit?url=file:///home/simple-java-maven-app


curl -s http://localhost:8080/git/notifyCommit?url=https://github.com/DianDochev-Kleinschnitz/demo.git

```

# dind starten

```bash
docker run   --name jenkins-docker   --rm   --detach   --privileged   --network jenkins   --network-alias docker   --env DOCKER_TLS_CERTDIR=/certs   --volume jenkins-docker-certs:/certs/client   --volume jenkins-data:/var/jenkins_home   --publish 2376:2376   docker:dind
```