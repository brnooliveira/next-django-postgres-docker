FROM python:3.10-alpine

WORKDIR /usr/src/app

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY app/ .

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

