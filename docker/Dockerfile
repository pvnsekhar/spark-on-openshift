FROM openjdk:8-jre

# Download and install Apache Spark
RUN wget https://downloads.apache.org/spark/spark-3.5.1/spark-3.5.1.tgz && \
    tar -xvzf spark-3.5.1.tgz  && \
    mv spark-3.5.1 /opt/spark && \
    rm spark-3.5.1.tgz

# Set Spark environment variables
ENV SPARK_HOME /opt/spark
ENV PATH $SPARK_HOME/bin:$PATH
