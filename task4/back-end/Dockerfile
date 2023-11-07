# Use the latest version of Ubuntu as a parent image
FROM ubuntu:latest

# Update and upgrade the system
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask
RUN pip3 install flask-cors

WORKDIR /app
COPY api.py .

# When the container launches, echo "Hello, World!"
CMD ["python3", "/app/api.py"]
