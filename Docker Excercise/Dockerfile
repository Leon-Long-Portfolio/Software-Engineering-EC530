FROM python:3.11-slim-buster

WORKDIR /app

COPY . .

RUN pip install --upgrade pip && \
    pip install flake8 pytest

RUN if [ -f requirements.txt ]; then pip install -r requirements.txt; fi


CMD ["pytest", "./tests"]

