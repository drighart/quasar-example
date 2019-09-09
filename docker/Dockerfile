FROM drighart/workbench-python-base:latest

RUN pip install \
    python-language-server \
    flake8 \
    autopep8 \
    pylint \
    pytest

ARG version=latest

WORKDIR /home/theia
ADD $version.package.json ./package.json
ARG GITHUB_TOKEN
RUN yarn --cache-folder ./ycache && rm -rf ./ycache
RUN yarn theia build

EXPOSE 3000 8080

RUN npm install -g @quasar/cli

ENV SHELL /bin/bash
ENTRYPOINT [ "yarn", "theia", "start", "/home/project", "--hostname=0.0.0.0" ]