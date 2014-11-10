Dependencies
============

* Docker - docker.com
* Fig - fig.sh
* Flocker - clusterhq.com


Demo 1 - Docker
===============

Building and pushing a Docker image::

    docker-osx shell
    docker build -t lmarsden/flask:v0.16 .; docker push lmarsden/flask:v0.16

Running Docker::

    docker run -p 80:80 lmarsden/flask:v0.16

Check your web browser: http://localdocker/


Demo 2 - Fig
============

Running fig::

    fig up

Check your web browser: http://localdocker/


Demo 3 - Flocker
================

Running flocker::

    flocker-deploy deployment-node1.yml fig.yml

Check your web browser: http://172.16.255.250/

Move Redis to second node::

    flocker-deploy deployment-node2.yml fig.yml

Check your web browser: http://172.16.255.250/
