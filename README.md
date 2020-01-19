# bitbucket-pipeline-image

Dockerfile for Bitbucket pipeline image

## Contents

- bash
- python 3.8
- pipenv

## Development

### Building The Image

```shell
$ docker image build --tag itprokyle/bitbucket-pipeline-image:latest .
```

### Publishing The Image

```shell
$ docker image push itprokyle/bitbucket-pipeline-image:latest
```

### Run The Image Locally

```shell
$ docker container run -it itprokyle/bitbucket-pipeline-image:latest /bin/bash
```
