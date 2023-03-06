FROM node:latest


WORKDIR /home/app

COPY chatbot-server/build/ ./

COPY ["chatbot-server/package.json","chatbot-server/package-lock.json", "./"]

RUN npm install --production

RUN npm install -g serve

CMD serve -s .