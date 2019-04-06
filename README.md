# Dockerized Hugo

## What Is This

This is a [Docker](https://www.docker.com) image of [Hugo](https://github.com/gohugoio/hugo), the Hugo is a powerful static site generator in [Golang](https://golang.org/). The purpose is to more easy to use Hugo, Golang will not be required in the host system and easy to switch Hugo version.

## How To Use This Image

### Create A New Site

```sh
docker run --rm -v $(pwd)/blog:/site shawnoy/hugo new site blog.0x427567.com
```

### Run Localhost Server

```sh
docker run --rm --volume $(pwd):/site -p 1313:1313 shawnoy/hugo server -D --bind 0.0.0.0
```
