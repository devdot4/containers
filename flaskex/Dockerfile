FROM python:3.9
RUN echo "Using Python v3.9"
RUN apt-get update
RUN echo "apt-get update went successfully."
RUN apt-get install python3 -y
RUN echo "python3 was installed successfully."
RUN apt-get install python3-pip -y
RUN echo "pip3 was installed successfully."
COPY . /app
RUN echo "Copied contents to /app"
WORKDIR /app
RUN echo "Work directory was updated to /app"
RUN pip3 install -r requirements.txt
RUN echo "Dependencies from requirements.txt were installed successfully."
EXPOSE 5000
RUN echo "Port 5000 is exposed."
CMD ["python3", "app.py"]
RUN echo "Running app.py"