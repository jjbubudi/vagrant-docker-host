Introduction
--------------
Setting up NFS share folder using the official boot2docker VM is a lot of work. Thanks to yungsang we have a vagrant box that allows us to do this easily.
This Vagrantfile configures a VM that shares your $HOME folder so that you can link your volumes as if your OSX machine was your actual Docker host.

Prerequisite
--------------
1. Only Mac OSX is supported
2. Vagrant 1.6+
3. Docker client (via homebrew)

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
