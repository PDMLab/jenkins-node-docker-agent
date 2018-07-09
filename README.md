# Jenkins Docker / Docker-Compose / Nodejs agent

This repository contains Docker image definitions to be used as Docker `agents` in Jenkins Pipelines.
The images contain the specified Node.js versions, `docker` and `docker-compose`.

## Usage

```groovy
agent {
    docker {
      image 'pdmlab/jenkins-node-docker-agent:6.11.1'
    }
  }
```

`wrapdocker` is based on https://github.com/jpetazzo/dind/blob/master/wrapdocker.
