FROM java:8

WORKDIR /opt

ENV MULE_VERSION 3.7.0

RUN wget https://repository.mulesoft.org/nexus/content/repositories/releases/org/mule/distributions/mule-standalone/${MULE_VERSION}/mule-standalone-${MULE_VERSION}.tar.gz

RUN tar xvzf /opt/mule-standalone-${MULE_VERSION}.tar.gz


RUN rm /opt/mule-standalone-${MULE_VERSION}.tar.gz

RUN ln -s /opt/mule-standalone-${MULE_VERSION} /opt/mule 


EXPOSE 8081

RUN echo "Running mule"

CMD [ "/opt/mule/bin/mule" ]
