```shell
docker build -t prabhatiitbhu/myjenkins .

docker run --name=myjenkins -d -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):/usr/bin/docker -p 8080:8080 prabhatiitbhu/myjenkins

docker exec -it myjenkins /bin/bash

cat /var/jenkins_home/secrets/initialAdminPassword
```
