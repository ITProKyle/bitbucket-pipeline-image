FROM python:3.8-alpine3.11

RUN apk add --no-cache bash curl make gcc git openssh-client openssl-dev libffi-dev musl-dev npm
RUN pip install --upgrade pip setuptools
RUN pip install --upgrade pipenv

# setup poetry
ENV POETRY_VERSION "1.1.4"
RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
ENV PATH "$PATH:/root/.poetry/bin"

# setup pyright
ENV PYRIGHT_VERSION "1.1.85"
RUN npm i -g "pyright@${PYRIGHT_VERSION}"

CMD ["/bin/bash"]
