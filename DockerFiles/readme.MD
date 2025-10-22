## Docker Installation

```
dnf -y install dnf-plugins-core
dnf config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo
dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
systemctl enable docker
systemctl start docker
```

sudo usermod -aG docker ec2-user --> are you using AWS Account


## Docker Commands 
ref :- ``` https://docs.docker.com/reference/dockerfile/ ```

* using override can't ENTRYPOINT
```
docker ps -a --no-trunc 
```

# Work Directory Cache Time (deatailed showing )
```
docker build -t workdir:v1 --no-cache --progress=plain WORKDIR/
```

# ARG build time we can overwrite Arg 
```
docker build -t workdir:v1 --no-cache --progress=plain --build-arg trainer=raghu ARG/
docker build -t arg:v1 --no-cache --progress=plain --build-arg version=8 ARG/
```

# onbild
* While Doveloping image you can put some conditions while other are using  your Images..

```
docker build -t onbuild:v1 --no-cache --progress=plain ONBUILD/
```


STOPSIGNAL signal # bydefault it is stop 