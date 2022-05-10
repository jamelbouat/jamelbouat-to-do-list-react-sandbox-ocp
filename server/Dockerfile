FROM debian:10-slim

RUN npm install -g json-server

RUN echo '{
            "tasks": [
              {
                "title": "first",
                "description": "I ain't got no description",
                "id": 2,
                "status": true
              },
              {
                "title": "second",
                "description": "I ain't got no description",
                "id": 3,
                "status": true
              }
            ]
          }' > /tasks.json

ENTRYPOINT ["json-server", "--port", "4400", "--host", "0.0.0.0"]

CMD ["/tasks.json"]
