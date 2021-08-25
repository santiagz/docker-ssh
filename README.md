# docker-ssh
![Supported Python versions](https://img.shields.io/badge/python-3.9-green.svg?style=for-the-badge&logo=appveyor) ![GitHub last commit](https://img.shields.io/github/last-commit/santiagz/docker-ssh?style=for-the-badge)
==========

A simple docker container that runs ssh

To build the image do:

```
docker build -t kartoza/ssh git://github.com/timlinux/docker-ssh
```

To run a container do:

```
docker run --name "ssh" -p 2222:22 -d -t kartoza/ssh
```

To log into your container do:

```
ssh root@localhost -p 2222
```

Default password will appear in docker logs:

```
docker logs <container name> | grep 'root login password'
```

-----------

Tim Sutton (tim@linfiniti.com)
May 2014
