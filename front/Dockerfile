FROM node:14-slim

LABEL description="frontend"

WORKDIR .

COPY ./package.json .
COPY ./package-lock.json .
RUN npm install

RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
