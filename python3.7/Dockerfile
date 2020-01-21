FROM python:3.7-alpine3.11

RUN apk add --no-cache bash make openssl-dev libffi-dev
RUN pip install --upgrade pip setuptools
RUN pip install --upgrade pipenv

CMD ["/bin/bash"]
