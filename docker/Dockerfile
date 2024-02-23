FROM openjdk:8-jre

# Download and install Apache Spark
RUN wget https://downloads.apache.org/spark/spark-3.2.0/spark-3.2.0-bin-hadoop3.2.tgz && \
    tar -xvzf spark-3.2.0-bin-hadoop3.2.tgz && \
    mv spark-3.2.0-bin-hadoop3.2 /opt/spark && \
    rm spark-3.2.0-bin-hadoop3.2.tgz

# Set Spark environment variables
ENV SPARK_HOME /opt/spark
ENV PATH $SPARK_HOME/bin:$PATH
