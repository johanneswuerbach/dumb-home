FROM arm32v6/python:3.6-alpine3.7

RUN apk add --no-cache git build-base

RUN git clone https://github.com/bejonwe/PrometheusSmartHome.git /usr/src/app

WORKDIR /usr/src/app

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000
CMD [ "python", "./main.py" ]
