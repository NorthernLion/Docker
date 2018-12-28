FROM ubuntu:16.04 

WORKDIR /mydir
RUN touch scirpt
COPY scirpt . 
RUN apt-get update && apt-get install -y wget && apt-get install -y curl 
RUN chmod 755 scirpt
CMD ["/bin/bash"]

