# jenkins
jenkins+docker 自动化构建部署搭建过程

# download jenkins image

```
docker pull jenkins/jenkins:lts
```

```
docker run --name myjenkins -d -v /your/jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts
```
NOTE:   确保当前jenkins 用户有权限操作文件目录```/your/jenkins_home``` ，更多命令选项关注[官方文档](https://github.com/jenkinsci/docker/blob/master/README.md)