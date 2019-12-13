FROM ubuntu:18.04

RUN apt update && \
  apt -y install curl jq && \
  rm -rf /var/lib/apt/lists/* && \
  curl -o /usr/local/bin/kubectl -L https://storage.googleapis.com/kubernetes-release/release/v1.17.0/bin/linux/amd64/kubectl && \
  chmod +x /usr/local/bin/kubectl

ENTRYPOINT ["/usr/local/bin/kubectl"]
