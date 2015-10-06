FROM jeanblanchard/busybox-java

MAINTAINER larry13767@gmail.com version 1.0

# Sets working directory for the CMD instruction (also works for RUN, ENTRYPOINT commands)
# Create mount point, and mark it as holding externally mounted volume
WORKDIR /data
VOLUME /data

# Expose the container's network port: 8989 during runtime.
EXPOSE 8989

CMD java -jar /data/turbine.jar
ADD target/turbine.jar /data/turbine.jar