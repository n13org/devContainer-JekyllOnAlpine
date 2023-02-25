## Jekyll on Alpine Docker Image

Dockerfile Arguments

|name|default|
|---|---|
| ALPINE_VERSION | 3.16     |
| RUBY_VERSION   | 3.1.3-r0 |
| JEKYLL_VERSION | 4.3.1-r0 |

Build the image

```shell
docker build --build-arg ALPINE_VERSION=3.17 --tag jekyllbuilder:latest .
```

Run the container from image

```shell
docker run -it --rm jekyllbuilder:latest
```
