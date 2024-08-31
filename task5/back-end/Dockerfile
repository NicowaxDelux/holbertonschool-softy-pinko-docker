FROM ubuntu:latest

RUN apt-get update &&\
    apt-get upgrade -y &&\
    apt-get install -y python3 python3-pip

RUN pip3 install --break-system-packages flask flask-cors

WORKDIR /app

COPY . .

EXPOSE 5252


CMD [ "python3", "api.py" ]