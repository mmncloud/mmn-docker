FROM hypriot/rpi-node
MAINTAINER tkrplus 

RUN git clone https://github.com/mmncloud/mmn-bot.git
WORKDIR /mmn-bot

EXPOSE 8080
ENTRYPOINT ["./bin/hubot","--adapter","slack"]
