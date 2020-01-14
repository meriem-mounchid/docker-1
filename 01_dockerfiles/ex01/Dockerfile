FROM debian

EXPOSE 30033 10011 9987

RUN apt update && apt install curl bzip2 -y

RUN curl https://files.teamspeak-services.com/releases/server/3.9.1/teamspeak3-server_linux_amd64-3.9.1.tar.bz2 -o ts.tar.bz2

RUN tar xvf ts.tar.bz2

WORKDIR teamspeak3-server_linux_amd64

RUN touch .ts3server_license_accepted

RUN  ./ts3server_startscript.sh start

#To run it :
#docker run -p 30033:30033 -p 10011:10011 -p 9987:9987/UDP -it ID
