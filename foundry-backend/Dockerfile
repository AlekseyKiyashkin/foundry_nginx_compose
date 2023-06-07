FROM node:20.2

WORKDIR /home/foundryvtt
COPY Foundry*.zip .
RUN apt install unzip
RUN unzip Foundry*.zip -d foundry && rm Foundry*.zip
WORKDIR /home/foundryvtt/foundry

VOLUME /home/foundryvtt/foundryuserdata

EXPOSE 30000
CMD [ "node", "resources/app/main.js", "--headless", "--dataPath=/home/foundryvtt/foundryuserdata" ]

