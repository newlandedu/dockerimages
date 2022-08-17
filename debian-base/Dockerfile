FROM registry.k8s.io/build-image/debian-base:bullseye-v1.2.0

ARG ARCH
ARG binary=./bin/${ARCH}/nfsplugin
COPY ${binary} /nfsplugin
