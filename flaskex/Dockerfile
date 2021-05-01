FROM python:3.9
RUN apt-get update
RUN apt-get install python3 -y
RUN apt-get install python3-pip -y
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt
EXPOSE 5000
CMD ["python3", "/app/app.py"]