FROM java:8-jdk
VOLUME /tmp
RUN mkdir  -p /letv/web
#ARG JAR_FILE
COPY target/elastic-job-lite-console-3.0.0.M1-SNAPSHOT.tar.gz /letv/web/elastic-job-lite-console-3.0.0.M1-SNAPSHOT.tar.gz

RUN cd /letv/web && tar xfvz elastic-job-lite-console-3.0.0.M1-SNAPSHOT.tar.gz
#ENV PROFILE=prod
WORKDIR /letv/web/elastic-job-lite-console-3.0.0.M1-SNAPSHOT/bin
CMD ./start.sh
EXPOSE 8899