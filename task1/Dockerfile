FROM ubuntu

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip

RUN rm -f /usr/lib/python3.*/EXTERNALLY-MANAGED

RUN pip3 install flask

WORKDIR /app

COPY api.py .

EXPOSE 5252

CMD ["python3", "api.py"]

#after starting run the docker script: docker run -p 5252:5252 task1(without this, the server will be isolated)
