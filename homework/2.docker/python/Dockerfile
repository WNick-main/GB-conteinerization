from python:3.9

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

ADD . /app

EXPOSE 8080

RUN chmod +x /app/app.py

ENTRYPOINT /app/app.py runserver 0.0.0.0:8080 