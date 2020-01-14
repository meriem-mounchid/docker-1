FROM debian:latest

RUN apt-get update && apt-get upgrade -y && \
		apt-get install vim git curl python3 python3-pip python3-dev -y && \
		mkdir /root/apps

WORKDIR /root/apps

ENTRYPOINT ["bash"]
