# docker build --rm -f docker/heroku/Dockerfile -t plugins/heroku .

FROM plugins/docker:latest

ARG OS="linux"
ARG ARCH="amd64"

ADD release/${OS}/${ARCH}/drone-docker-heroku /bin/
ENTRYPOINT ["/usr/local/bin/dockerd-entrypoint.sh", "/bin/drone-docker-heroku"]
