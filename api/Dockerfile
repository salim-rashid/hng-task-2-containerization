FROM python:3.9.15-buster

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code
COPY requirements.txt /code/

RUN pip3 install -r requirements.txt
COPY . /code/

EXPOSE 8000

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
