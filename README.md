# php-docker
PHP 8.5.12 FPM on Alpine Linux

[Docker Hub](https://hub.docker.com/r/kairyou/php-docker)

```sh
docker pull kairyou/php-docker:8.5.12
```

The image includes Imagick, Redis, Memcached, GD, MySQL and PostgreSQL extensions,
and OPcache.

Pushes to `main` and manual runs of the Docker Image CI workflow build and publish
`linux/amd64` and `linux/arm64` images with the `8.5.12`, `latest`, and build date
tags. The workflow summary records the published image digest. Use the version
tag or the verified digest for deployments, and test the published image before
upgrading an existing application.

When upgrading PHP, update both the Dockerfile base version and the workflow's
`VERSION` value.
