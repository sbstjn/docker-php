# sbstjn/php [![Docker Stars](https://img.shields.io/docker/stars/sbstjn/php.svg?maxAge=600)](https://hub.docker.com/r/sbstjn/php/) [![Docker Pulls](https://img.shields.io/docker/pulls/sbstjn/php.svg?maxAge=600)](https://hub.docker.com/r/sbstjn/php/)

> Docker image with useful tools for `PHP` projects. Works fine in CircleCI and GitLab CI.

## Components

- `aws-cli/1.16.70 Python/2.7.15 Linux/4.9.125-linuxkit botocore/1.12.60`
- `awscurl`
- `cfn-lint 0.18.1`
- `Docker version 18.06.1-ce, build e68fc7a`
- `PHP 7.2.20`
- `Composer version 1.8.6 2019-06-11 15:03:05`
- `PHPUnit 7.5.13`

## Usage

### General

```Dockerfile
# Dockerfile

FROM sbstjn/php
```

### CircleCI

```yaml
jobs:
  checkout:
    docker:
      - image: sbstjn/php
```

## Development

```bash
# Clone repository

$ > git clone git@github.com:sbstjn/docker-php.git
$ > cd docker-php

# Build container

$ > docker build .

# Start bash and test your environment

$ > docker run -it --entrypoint /bin/bash <container-id>
```

## License

Feel free to use the code, it's released using the [MIT license](LICENSE.md).

## Contribution

You are welcome to contribute to this project! 😘

To make sure you have a pleasant experience, please read the [code of conduct](CODE_OF_CONDUCT.md). It outlines core values and beliefs and will make working together a happier experience.