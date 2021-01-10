## Grant permission

```
cd ./docker-image
chmod +x entry.sh
```

## Build

```
cd ./docker-image
docker build -t lambda/python:3.9-alpine3.12 .
```

## Run in local

```
cd ./docker-image
docker run -p 9000:8080 lambda/python:3.9-alpine3.12
```

```
% curl -XPOST "http://localhost:9000/2015-03-31/functions/function/invocations" -d '{}'
"Hello from AWS Lambda using Python3.9.1 (default, Dec 17 2020, 01:59:58) \n[GCC 9.3.0]!"
```
