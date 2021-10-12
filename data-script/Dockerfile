FROM alpine
RUN apk update && \
    apk add mysql-client

WORKDIR /opt

COPY import.sh /opt
COPY mydatabase.sql /opt

RUN chmod +x /opt/import.sh

CMD /opt/import.sh
