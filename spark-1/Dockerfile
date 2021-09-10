FROM datamechanics/spark:2.4.7-hadoop-3.1.0-java-8-scala-2.12-python-3.7-latest

RUN pip3 install numpy
RUN /opt/entrypoint.sh

WORKDIR /app

COPY src /app

CMD ["/opt/spark/bin/pyspark", "/app/src/build_model.py"]