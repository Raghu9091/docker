## Docker Learning understandig the Containers 

```
https://joindevops.medium.com/why-containerization-is-popular-how-to-understand-the-advantages-55261a17517c
```


#  Docker is containerasation platform

![alt txt](containers.svg)


# docker port working
![alt txt](docker.svg)


## Docker Installation

```
dnf -y install dnf-plugins-core
dnf config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo
dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
systemctl enable docker
systemctl start docker
```