FROM hypriot/rpi-java
MAINTAINER tkrplus 

# jenkins 2.0 系を使用するように変更
RUN wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -

RUN apt-get update && \
	apt-get upgrade && \
	apt-get install -y wget


# jenkins 2.0 系を使用するように変更
RUN wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add - && \
	apt-get update && \
	apt-get install jenkins 

EXPOSE 8080
EXPOSE 50000

USER jenkins

ENTRYPOINT ["service","jenkins","restart"]
