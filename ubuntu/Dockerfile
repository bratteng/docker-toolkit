FROM ubuntu:jammy-20240405

RUN apt-get update \
  && apt-get install --no-install-recommends --no-install-suggests -y \
    ca-certificates \
    curl \
    dnsutils \
    iputils-ping \
    iproute2 \
    wget \
    btop \
    redis-tools

COPY --from=smallstep/step-cli:0.25.2 /usr/local/bin/step /usr/local/bin/step
