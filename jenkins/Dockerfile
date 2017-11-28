FROM hypriot/rpi-java
MAINTAINER tkrplus 

RUN apt-get update; \
		apt-get upgrade; \
		apt-get install jenkins; \

EXPOSE 8080
EXPOSE 50000

USER jenkins

ENTRYPOINT ["service","jenkins","restart"]
