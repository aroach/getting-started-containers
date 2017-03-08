https://pwd.mantl.io

```
docker search hello-world
docker run hello-world
```

https://hub.docker.com


# workshop 1

```
docker search ubuntu
docker run -ti ubuntu
touch /HELLO
```

# workshop 2

```
git clone -b dist https://github.com/tianon/docker-brew-ubuntu-core.git
cd docker-brew-ubuntu-core/xenial
docker build .
docker images
docker run –ti <image id>
```

```
#!/usr/bin/env python

print("Hello from DevNet CL ANZ!")
```

```
# Dockerfile
RUN apt-get update
RUN apt-get -y install python
ADD hellodevnet.py /hellodevnet.py
RUN chmod +x /hellodevnet.py

CMD["/hellowdevnet.py"]
```

```
docker run <image ID>
```

# workshop 3

```
FROM ubuntu
RUN apt-get update
RUN apt-get –y install python
ADD hellodevnet.py /hellodevnet.py

CMD [“/hellodevnet.py”]
```

```
git clone https://github.com/matjohn2/container-intro-devnet.git

cd container-intro-devnet

cat Dockerfile

docker build .
```

# workshop 4


```
# Dockerfile
FROM ubuntu
RUN apt-get update
RUN apt-get -y install python
EXPOSE 8000
ENTRYPOINT [“python”, “-m”, “SimpleHTTPServer”, “8000”]
```

```
docker run <new image id>
docker ps
docker inspect <Container ID> 
curl http://<CONTAINERIP>:8000/
```



