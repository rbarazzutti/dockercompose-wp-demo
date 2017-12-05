WordPress Instances in Docker Compose
=====================================

This repo just contains an example `docker-compose setup` that shows some features of Docker, s.t.
* Networks
* Volumes

This setup contains a pair of full-fledged Wordpress installation (MySQL and WordPress containers) and an Nginx instance that routes HTTP requests to the appropriate Wordpress installation.

Requirements:
* [Docker](https://store.docker.com/search?type=edition&offering=community)
* [Docker-Compose](https://docs.docker.com/compose/install/)

Usage:

    git clone http://www.github.com/rbarazzutti/dockercompose-wp-demo
    cd dockercompose-wp-demo
    docker-compose up -d

Then `docker-compose` will start two MySQL instances, two WordPress instances and an Nginx instance to handle the requests.

This setup is working with two differents hostnames that are actually supposed to point to your lovely home (127.0.0.1).

Once `docker-compose` finished its job, you'd be able to access it with the following URLs:
* http://wp-alpha.fever.ch:8080
* http://wp-beta.fever.ch:8080

December, 5th 2017 RBarazzutti