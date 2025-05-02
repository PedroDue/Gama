FROM node:20

RUN npm install -g @angular/cli@19.2.10

WORKDIR /app

COPY gama-front/package*.json ./gama-front/
RUN cd gama-front && npm install

COPY gama-front/ ./gama-front/

WORKDIR /app/gama-front

EXPOSE 4201
CMD ["npm", "start"]
