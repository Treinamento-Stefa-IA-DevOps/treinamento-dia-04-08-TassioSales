#FROM python:3.8-slim
FROM centos/python-36-centos7

COPY . /codigo

WORKDIR /codigo

RUN pip install uvicorn panda fastapi sklearn

CMD ["uvicorn", "main:app","--host", "0.0.0.0", "--port", "5000", "--reload"]
