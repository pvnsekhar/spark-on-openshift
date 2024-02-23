FROM openjdk:8-jre

RUN apt-get update && apt-get install -y procps

# Download and install Apache Spark
RUN wget https://downloads.apache.org/spark/spark-3.5.1/spark-3.5.1-bin-hadoop3-scala2.13.tgz && \
    tar -xvzf spark-3.5.1-bin-hadoop3-scala2.13.tgz  && \
    mv spark-3.5.1-bin-hadoop3-scala2.13 /opt/spark && \
    rm spark-3.5.1-bin-hadoop3-scala2.13.tgz

# Set Spark environment variables
ENV SPARK_HOME /opt/spark
ENV PATH $SPARK_HOME/bin:$PATH

ENTRYPOINT [ "/opt/spark/sbin/start-master.sh" ]