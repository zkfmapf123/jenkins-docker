# Dockerfile in Jenkins

## 설치방법

- 1. jenkins 폴더안에서 작업 실행

```
    docker build -t jenkins-docker .

    ddocker run -p 8080:8080 -p 50000:50000 \
    -v /var/jenkins_home:/var/jenkins_home \
    -v /var/run/docker.sock:/var/run/docker.sock \
    --name jenkins -d jenkins-docker
```
