# nginx-echo-headers

A simple tool for debugging HTTP requests, nginx will return all request headers and body to the client.

## Build for EKS, arm architecture
```shell
docker build --platform linux/arm64/v8 -t veretie/nginx-echo-headers .
docker push veretie/nginx-echo-headers:latest
```

## Run
```shell
docker pull veretie/nginx-echo-headers
docker run -p 8080:8080 veretie/nginx-echo-headers
```