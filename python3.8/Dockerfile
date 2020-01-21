FROM python:3.8-alpine3.11

RUN apk add --no-cache bash make gcc openssl-dev libffi-dev musl-dev
RUN pip install --upgrade pip setuptools
RUN pip install --upgrade pipenv

CMD ["/bin/bash"]
