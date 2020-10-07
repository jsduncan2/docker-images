FROM alpine:latest

WORKDIR /app

ARG VERSION=v1.19.2
ADD https://storage.googleapis.com/kubernetes-release/release/${VERSION}/bin/linux/amd64/kubectl kubectl

RUN chmod +x kubectl && \
  /app/kubectl version --client

ENTRYPOINT [ "/app/kubectl" ]
