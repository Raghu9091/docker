## Docker Commands 

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
```
docker build -t onbuild:v1 --no-cache --progress=plain ONBUILD/
```


