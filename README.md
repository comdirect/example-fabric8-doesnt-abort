This repo is for reproducing the [issue #1512 Plugin doesn't abort the build in case the Dockerfile can't be processed when building remote](https://github.com/fabric8io/docker-maven-plugin/issues/1512).
It can be deleted as soon as the issue is closed.

Commands, see also the issue:

Running podman as a service:

    $ podman system service tcp:localhost:8880 --log-level=debug --time=0

Building with the fabric8 docker-maven-plugin:

    $ mvn clean install -Pfabric8

Building with the spotify docker-maven-plugin:

    $ mvn clean install -Pspotify
