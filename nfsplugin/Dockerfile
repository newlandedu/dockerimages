FROM registry.k8s.io/build-image/debian-base:bullseye-v1.2.0

ARG ARCH
ARG binary=./bin/${ARCH}/nfsplugin
COPY ${binary} /nfsplugin

RUN apt update && apt upgrade -y && apt-mark unhold libcap2 && clean-install ca-certificates mount nfs-common netbase

ENTRYPOINT ["/nfsplugin"]
