# docker-forward-proxy

Simple forward proxy.

## Install

```
$ docker pull u1aryz/forward-proxy:latest
```

## Quickstart

- Simple
```
$ docker run -d --name goproxy --restart=always -p 64444:8080 u1aryz/forward-proxy
```

- If use basic auth

```
$ docker -d --name goproxy --restart=always -p 64444:8080 u1aryz/forward-proxy -user=u1aryz -pass=hogefuga
```

- If change container port

```
$ docker run -p 3128:9090 u1aryz/forward-proxy -port=9090
```
