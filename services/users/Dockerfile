FROM python:3.7.4-alpine3.10

COPY . /usr/src/app
WORKDIR /usr/src/app
RUN pip install -r requirements.txt

CMD python manage.py run -h 0.0.0.0
