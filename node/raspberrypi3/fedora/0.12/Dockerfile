# AUTOGENERATED FILE
FROM resin/raspberrypi3-fedora-buildpack-deps:latest

ENV NODE_VERSION 0.12.15

RUN curl -SLO "http://resin-packages.s3.amazonaws.com/node/v$NODE_VERSION/node-v$NODE_VERSION-linux-armv7hf.tar.gz" \
	&& echo "93646a95f3810dea773d9a7846b12337afa84722adea9be93dbe5f4c9b06efc9  node-v0.12.15-linux-armv7hf.tar.gz" | sha256sum -c - \
	&& tar -xzf "node-v$NODE_VERSION-linux-armv7hf.tar.gz" -C /usr/local --strip-components=1 \
	&& rm "node-v$NODE_VERSION-linux-armv7hf.tar.gz" \
	&& npm config set unsafe-perm true -g --unsafe-perm \
	&& rm -rf /tmp/*

CMD ["echo","'No CMD command was set in Dockerfile! Details about CMD command could be found in Dockerfile Guide section in our Docs. Here's the link: http://docs.resin.io/deployment/dockerfile"]
