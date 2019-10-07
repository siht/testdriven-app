FROM python:3.7.4-alpine3.10

RUN apk update && \
    apk add --virtual build-deps gcc python-dev musl-dev && \
    apk add postgresql-dev && \
    apk add netcat-openbsd

COPY . /usr/src/app
WORKDIR /usr/src/app
RUN chmod +x ./entrypoint.sh && pip install -r requirements.txt

CMD ["/usr/src/app/entrypoint.sh"]
