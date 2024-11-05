FROM python:3.11.9-slim

RUN pip install pipenv

WORKDIR /app                                                                

COPY ["Pipfile", "Pipfile.lock", "./"]

RUN pipenv install --system --deploy

COPY ["predict.py", "model_C=1.0.bin", "./"]
