FROM arm32v6/python:3.6-alpine3.7

RUN apk add --no-cache git

RUN git clone https://github.com/johanneswuerbach/PrometheusSmartHome.git /usr/src/app

WORKDIR /usr/src/app

RUN git checkout invalid-auth

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000
CMD [ "python", "./main.py" ]
