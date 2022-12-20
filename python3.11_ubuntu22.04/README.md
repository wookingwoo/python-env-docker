# python3.11_ubuntu22.04

## Make Docker Images

### Pull Container Images

<https://hub.docker.com/r/wookingwoo/python3.11-on-ubuntu22.04>

```bash
docker pull wookingwoo/python3.11-on-ubuntu22.04:1.0
```

### Building Docker Images with Dockerfiles

```bash
docker build --tag python3.11-on-ubuntu22.04:1.0 .
```

## Run Container

```bash
docker run -it --name python3.11-on-ubuntu22.04 python3.11-on-ubuntu22.04:1.0
```
