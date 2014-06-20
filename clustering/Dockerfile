FROM ubuntu
MAINTAINER Hiroki Kumazaki

RUN echo "deb http://download.jubat.us/apt binary/" >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y --allow-unauthenticated  jubatus

EXPOSE 9199

ENV JUBATUS_HOME /opt/jubatus
ENV PATH /opt/jubatus/bin:${PATH}
ENV LD_LIBRARY_PATH /opt/jubatus/lib:${LD_LIBRARY_PATH}
ENV LDFLAGS -L$/opt/jubatus/lib ${LDFLAGS}
ENV CPLUS_INCLUDE_PATH /opt/jubatus/include:${CPLUS_INCLUDE_Path}

# set filename
ADD kmeans.json /tmp/config.json
CMD jubaclustering -f /tmp/config.json
