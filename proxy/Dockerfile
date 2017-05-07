# Use an official Python runtime as a base image
#FROM ubuntu:16.04
FROM python:2.7-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN cp -r .pip /root/
#RUN apt-get update
#RUN apt-get install python2.7-dev \
#python-pip -y
#RUN ln -s /usr/lib/python2.7/plat-*/_sysconfigdata_nd.py /usr/lib/python2.7/
RUN pip install shadowsocks
# Make port 80 available to the world outside this container
EXPOSE 8000

# Define environment variable
ENV NAME World

#CMD ["local", "-c", "shadowsocks.json"]

