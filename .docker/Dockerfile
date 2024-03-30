FROM node:latest

RUN mkdir -p /site/app
WORKDIR /aws

COPY package.json /aws
COPY app /site/app

RUN npm install --omit=dev

EXPOSE 3000/tcp

CMD ["npm", "run", "start"]
