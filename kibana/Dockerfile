FROM kibana:4.6

# disable the standard kibana discovery, visualize & dashboard plugins 
# they aren't compatible with elasticsearch 1.7
RUN echo "kibana.enabled: false" >> /opt/kibana/config/kibana.yml
RUN echo "elasticsearch.enabled: false" >> /opt/kibana/config/kibana.yml

WORKDIR /opt/kibana
RUN ./bin/kibana plugin --install elastic/sense
