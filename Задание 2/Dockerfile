FROM python:3.9-alpine

COPY ./stocks_products/requirements.txt /src/requirements.txt

WORKDIR src

RUN pip3 install --no-cache-dir -r requirements.txt

COPY ./stocks_products /src

EXPOSE 8000

LABEL description="Luzanov_homework_add"

ENV MY_ENV=netology

RUN [ "python", "manage.py", "makemigrations"] \
&& [ "python", "manage.py", "migrate"]

CMD [ "python", "manage.py", "runserver", "0.0.0.0:8000"]
