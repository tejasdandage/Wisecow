FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive
ENV PATH="/usr/games:$PATH"

RUN apt update && \
    apt install -y cowsay fortune-mod netcat-openbsd && \
    apt clean

COPY wisecow.sh /usr/local/bin/wisecow.sh
RUN chmod +x /usr/local/bin/wisecow.sh

CMD ["/usr/local/bin/wisecow.sh"]




