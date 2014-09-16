# Set the base image to use to Ubuntu w/ Java 7
FROM java:7

# Set the file maintainer
MAINTAINER Nick Richardson <richa283@uwm.edu>

RUN apt-get update
RUN apt-get install -y unzip wget git

ENV VERSION 1.2.7

RUN wget http://downloads.typesafe.com/typesafe-activator/$VERSION/typesafe-activator-$VERSION.zip 

RUN unzip typesafe-activator-$VERSION.zip -d /opt && chmod -R a+w /opt/activator-$VERSION
ENV PATH $PATH:/opt/activator-$VERSION/
