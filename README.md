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

# jenkins starten

```bash
 docker run --name jenkins-blueocean --rm --detach   --network jenkins --env DOCKER_HOST=tcp://docker:2376   --env DOCKER_CERT_PATH=/certs/client --env DOCKER_TLS_VERIFY=1   --publish 8080:8080 --publish 50000:50000   --volume jenkins-data:/var/jenkins_home   --volume jenkins-docker-certs:/certs/client:ro --volume /home/dian/workspace/jenkins:/home  myjenkins-blueocean:1.1

```

