# docker build --rm -f docker/heroku/Dockerfile -t plugins/heroku .

ARG BASE=docker:18.03.1-ce-dind
FROM $BASE

ARG OS="linux"
ARG ARCH="amd64"

ADD release/${OS}/${ARCH}/drone-docker /bin/
ADD release/${OS}/${ARCH}/drone-docker-heroku /bin/
ENTRYPOINT ["/usr/local/bin/dockerd-entrypoint.sh", "/bin/drone-docker-heroku"]
