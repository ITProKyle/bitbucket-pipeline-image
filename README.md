# bitbucket-pipeline-image

Bitbucket pipeline image containing the components most used for testing and building projects. The tabs revolve around the primary language required but will include all listed languages. If the tag is not specific to a language, the latest version of the language is used.


## Contains

- bash
- python
  - pipenv


## Development

Docker images are built automatically when merged into master so there is no need to manually publish new versions.

### Building The Image

```shell
$ docker image build --tag bitbucket-pipeline-image:tag .
```

### Publishing The Image

```shell
$ docker image push bitbucket-pipeline-image:tag
```

### Run The Image Locally

```shell
$ docker container run -it bitbucket-pipeline-image:tag /bin/bash
```
