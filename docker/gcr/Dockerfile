# docker build --rm -f docker/gcr/Dockerfile -t plugins/gcr .

FROM plugins/docker:latest

ARG OS="linux"
ARG ARCH="amd64"

ADD release/${OS}/${ARCH}/drone-docker-gcr /bin/
ENTRYPOINT ["/usr/local/bin/dockerd-entrypoint.sh", "/bin/drone-docker-gcr"]
