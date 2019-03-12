FROM	ft-rails:on-build

RUN 	apt-get update && gem install rails -v 4.2.7 && mkdir -p /opt/app
COPY 


EXPOSE	3000
CMD		["rails", "s", "-b", "0.0.0.0", "-p", "3000"]
