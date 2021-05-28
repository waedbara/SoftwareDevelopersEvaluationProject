FROM apache/nifi:latest

COPY ./nifi-graph-nar-1.13.2.nar /opt/nifi/nifi-current/lib
COPY ./nifi-graph-client-service-api-nar-1.13.2.nar /opt/nifi/nifi-current/lib
COPY ./nifi-neo4j-cypher-service-nar-1.13.2.nar /opt/nifi/nifi-current/lib
COPY ./nifi-other-graph-services-nar-1.13.2.nar /opt/nifi/nifi-current/lib

#USER root
#RUN chown nifi /opt/nifi/nifi-current/lib/nifi-graph-nar-1.13.2.nar
