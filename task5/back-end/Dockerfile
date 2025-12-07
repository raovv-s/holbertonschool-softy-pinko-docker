FROM ubuntu:latest

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN pip3 install flask
RUN pip3 install flask-cors

COPY api.py /app/api.py

WORKDIR /app

EXPOSE 5252

CMD ["python3","api.py"]
#after  starting run the docker script: docker run -p 5252:5252 task1(without this, the server will be isolated)
