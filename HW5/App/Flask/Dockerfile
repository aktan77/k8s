FROM python:3.6-alpine

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
RUN apk upgrade && apk update && apk add curl

COPY . .

CMD [ "python3", "-u", "flask_app.py" ]
