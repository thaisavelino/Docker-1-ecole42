FROM debian:9.3

MAINTAINER tavelino <tavelino@student.42.fr>

RUN apt-get update && apt-get -y upgrade && apt -y install wget && apt-get -y install bzip2

RUN wget https://files.teamspeak-services.com/releases/server/3.6.1/teamspeak3-server_linux_amd64-3.6.1.tar.bz2 \
   && tar -xf teamspeak3-server_linux_amd64-3.6.1.tar.bz2

ENV TS3SERVER_LICENSE=accept

EXPOSE 9987/udp 10011 30033 41144

CMD /teamspeak3-server_linux_amd64/ts3server_minimal_runscript.sh starerver query
