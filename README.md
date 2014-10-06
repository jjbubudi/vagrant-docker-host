Prerequisite
--------------
1. Vagrant 1.6+
2. Docker client (via homebrew if you are using OSX)

Booting the VM
--------------

```sh
export DOCKER_HOST=tcp://localhost:2375
vagrant up
```

Test it out
--------------
```sh
docker run -it --rm ubuntu:latest bash
```

License
----

MIT
