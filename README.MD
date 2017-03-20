# Clair CoreOS with local-image-analyzer ready

A Dockerfile and docker-compose for running Vulnerability Static Analysis for Containers using [Clair](https://github.com/coreos/clair).

The Dockerfile also contains the local-image-analyzer for analyzing local docker images.

# How to run

Run ``docker-compose up`` to get clair and postgresql up.

Please restart clair in case it stops due to postgres startup order.

To analyze your image, run: ``docker exec clair_clair analyzer <imageID>

Refer to [Clair docker-compose](https://github.com/coreos/clair#docker-compose) for more information.


