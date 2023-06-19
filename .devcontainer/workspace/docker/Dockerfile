FROM mcr.microsoft.com/devcontainers/php:0-8.2

RUN apt-get update -y \
  && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
    postgresql-client \
  && apt-get autoremove -y \
  && apt-get clean \
  && rm -rf /var/cache/apt/* /var/lib/apt/lists/
