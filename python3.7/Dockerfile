FROM python:3.7-alpine3.11

RUN apk add --no-cache bash curl make gcc openssl-dev libffi-dev musl-dev
RUN pip install --upgrade pip setuptools
RUN pip install --upgrade pipenv

# setup poetry
ENV POETRY_VERSION "1.1.4"
RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
ENV PATH "$PATH:/root/.poetry/bin"

CMD ["/bin/bash"]
