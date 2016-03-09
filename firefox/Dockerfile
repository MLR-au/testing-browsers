from ubuntu:xenial

RUN apt-get update && apt-get install -y firefox xvfb
COPY start /usr/local/bin/ 
RUN chmod +x /usr/local/bin/start
ENTRYPOINT /usr/local/bin/start