# docker build --rm -f docker/ecr/Dockerfile -t plugins/ecr .

FROM plugins/docker:latest

ARG OS="linux"
ARG ARCH="amd64"

ADD release/${OS}/${ARCH}/drone-docker-ecr /bin/
ENTRYPOINT ["/usr/local/bin/dockerd-entrypoint.sh", "/bin/drone-docker-ecr"]
