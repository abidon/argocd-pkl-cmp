FROM debian:stable-slim

ARG TARGETARCH
ARG TARGETOS

RUN apt-get update && \
    apt-get install -y curl && \
    curl -L -o /usr/bin/pkl "https://github.com/apple/pkl/releases/download/0.28.2/pkl-$TARGETOS-$(echo $TARGETARCH | sed s/arm64/aarch64/)" && \
    chmod +x /usr/bin/pkl && \
    apt-get purge -y curl && \
    apt-get clean && apt-get autoremove -y
