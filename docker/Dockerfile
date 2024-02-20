FROM spark:python3

EXPOSE 8080/tcp
EXPOSE 7077/tcp

RUN mkdir /opt/spark/logs

ENTRYPOINT [ "/opt/spark/sbin/start-master.sh" ]

USER spark