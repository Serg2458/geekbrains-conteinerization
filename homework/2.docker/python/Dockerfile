FROM python:3.9-alpine

WORKDIR /my_app

COPY . .

RUN adduser -D docker && chown -R docker /my_app && pip install -r requirements.txt && rm -rf /var/cache 

USER docker

EXPOSE 8080

ENTRYPOINT python app.py 	
