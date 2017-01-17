FROM alpine

COPY . /web

VOLUME /web

COPY ./keepcontaineralive.sh /tmp
RUN chmod 755 /tmp/keepcontaineralive.sh

CMD /tmp/keepcontaineralive.sh 
