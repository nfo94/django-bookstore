FROM python:3.10.6-slim-bullseye

# disables automatic check for pip updates each time
ENV PIP_DISABLE_PIP_VERSION_CHECK 1
# python will not try to write .pyc files
ENV PYTHONDONTWRITEBYTECODE 1
# ensures our console output is not buffered by Docker
ENV PYTHONBUFFERED 1

WORKDIR /code

COPY ./requirements.txt .
RUN pip install -r requirements.txt

COPY . .
