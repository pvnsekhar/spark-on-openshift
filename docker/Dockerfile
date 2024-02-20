FROM spark:python3

EXPOSE 8080/tcp
EXPOSE 7077/tcp


ENTRYPOINT [ "/opt/spark/sbin/start-master.sh --port 7077 --webui-port 8080" ]

USER spark