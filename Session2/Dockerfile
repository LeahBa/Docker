FROM alpine:latest
LABEL maintainer="chagitlb@gmail.com"

RUN apk update
RUN apk add --update python3 py3-pip

COPY . /src
WORKDIR /src

RUN pip3 install click==7.0 Flask==1.0.2 itsdangerous==1.1.0 Jinja2==2.10 MarkupSafe==1.1.1 Werkzeug==0.14.1

EXPOSE 5000

ENTRYPOINT ["python3", "./app.py"]
