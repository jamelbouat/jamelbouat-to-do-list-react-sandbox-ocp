FROM node:16-slim

RUN npm install -g json-server

RUN echo '{"tasks": [{"title": "first","description": "No description","id": 2,"status": true}]}' > tasks.json

ENTRYPOINT ["json-server", "--port", "4400", "--host", "0.0.0.0"]

CMD ["tasks.json"]
