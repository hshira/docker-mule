FROM java:7

WORKDIR /opt

ENV MULE_VERSION 3.6.0

RUN wget https://repository.mulesoft.org/nexus/content/repositories/releases/org/mule/distributions/mule-standalone/${MULE_VERSION}/mule-standalone-${MULE_VERSION}.tar.gz

RUN tar xvzf /opt/mule-standalone-${MULE_VERSION}.tar.gz

#RUN echo "4a94356f7401ac8be30a992a414ca9b9 mule-standalone-${MULE_VERSION}.tar.gz" | md5sum -c

RUN rm /opt/mule-standalone-${MULE_VERSION}.tar.gz

RUN ln -s /opt/mule-standalone-${MULE_VERSION} /opt/mule 

CMD [ "/opt/mule/bin/mule" ]