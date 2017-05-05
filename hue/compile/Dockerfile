# Use an official Python runtime as a base image
FROM ubuntu:16.04

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt

#RUN cd hue
RUN apt-get update -y
#RUN apt-get install git -y
#RUN git clone https://github.com/cloudera/hue.git
RUN apt-get install python2.7-dev \
make \
libkrb5-dev \
libxml2-dev \
libffi-dev \
libxslt-dev \
libsqlite3-dev \
libssl-dev \
libldap2-dev \
python-pip -y
RUN ln -s /usr/lib/python2.7/plat-*/_sysconfigdata_nd.py /usr/lib/python2.7/
RUN apt-get install ant gcc g++ libkrb5-dev libffi-dev libmysqlclient-dev libssl-dev libsasl2-dev libsasl2-modules-gssapi-mit libsqlite3-dev libtidy-0.99-0 libxml2-dev libxslt-dev make libldap2-dev maven python-dev python-setuptools libgmp3-dev maven -y
# RUN add-apt-repository ppa:webupd8team/java
# RUN apt-get install oracle-java7-installer -y
# RUN apt-get install oracle-java7-set-default -y
# RUN  make apps
# Make port 80 available to the world outside this container
EXPOSE 8000

# Define environment variable
ENV NAME World

# Run app.py when the container launches
# CMD ["./hue/build/env/bin/hue", "runserver"]
