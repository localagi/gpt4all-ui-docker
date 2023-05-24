# gpt4all-ui-docker

Sophisticated docker builds for parent project [nomic-ai/gpt4all-ui](https://github.com/nomic-ai/gpt4all-ui). 

![example workflow](https://github.com/localagi/gpt4all-ui-docker/actions/workflows/publish-docker.yml/badge.svg?branch=main)

Easy setup. Compatible. Tweakable. Scaleable.

#### Supported platforms
`amd64`, `arm64`

#### Supported versions
 
Containers follow the version scheme of the parent project

`main` (default), `v0.0.9`,  etc.

See [Releases](../../releases)

## Prerequisites

* `docker` and `docker compose` are available on your system

## Run
make sure you have a config
  * `wget -P configs/ https://raw.githubusercontent.com/nomic-ai/gpt4all-ui/main/configs/default.yaml`

### via compose (recommended)

* get `docker-compose.yml` (clone repo, copy or else) 
* Run `docker compose up`
* wait for everything to finish
* open/refresh `http://localhost:9600` 

### via cli

* `docker run -p 9600:9600 -v ./configs:/srv/configs localagi/gpt4all-ui:main`

### Runtime options
Environment variables to set for the specific service

#### version selection `GPT4ALL_UI_VERSION`
Prepend, e.g. `GPT4ALL_UI_VERSION=v0.0.9`


### Get the latest builds / update
`docker compose pull`

### Cleanup
`docker compose rm`

## Contributing

When there is a new version and there is need of builds or you require the latest main build, feel free to open an issue

## Problems?

Open an issue on the [Issue Tracker](../../issues)

## Limitations
We cannot support issues regarding the base software. Please refer to the main project page mentioned in the second line of this card.

