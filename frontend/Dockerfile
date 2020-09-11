FROM node:13.12.0-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

ENV NG_CLI_ANALYTICS=false


COPY . .
RUN npm install --silent --no-optional
RUN npm i -g @angular/cli

EXPOSE 4200

CMD ["npm", "run", "start"]
