FROM registry.access.redhat.com/ubi8/ubi-minimal:latest

# Install util-linux for commands like mountpoint
RUN microdnf install -y procps-ng curl util-linux findutils python3 python3-pip \
  && microdnf clean all \
  && pip3 --disable-pip-version-check install -U --compile --no-cache-dir awscli s3cmd