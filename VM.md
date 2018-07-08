# 가상머신 사용법

## Docker
### installation(centos7)
- `sudo yum install yum-utils deviece-mapper-persistent-data lvm2`
- `sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
- `sudo yum install docker-ce`
- `sudo systemctl start docker`
- `docker -v`

- 도커 포트 4243 개방
`sudo firewall-cmd --zone=public --add-port=4243/tcp`
### installation(ubuntu 16.10)


### 



