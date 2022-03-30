FROM node:16

LABEL version="1.0.0." description="Solution Sprint FIAP - Fase 4" maintainer="André Melo<andreluismelo@gmail.com>"

COPY app/* .

EXPOSE 8080

RUN npm install -g nodemon

COPY . .

CMD [ "node", "app.js" ]
