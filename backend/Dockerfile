FROM ubuntu:22.04

RUN sed -i 's|http://archive.ubuntu.com|http://in.archive.ubuntu.com|g' /etc/apt/sources.list \
 && apt-get update \
 && apt-get install -y --no-install-recommends g++ ca-certificates \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /app
COPY . .
CMD ["bash"]
