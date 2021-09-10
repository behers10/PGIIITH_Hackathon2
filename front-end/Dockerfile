FROM python:3.6-slim

RUN pip3 install flask
RUN pip3 install kafka

WORKDIR /app

COPY content /app/
COPY templates /app/
COPY app.py /app/

EXPOSE 4000

CMD ["python3", "app.py"]
