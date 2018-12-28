FROM ubuntu:16.04 

WORKDIR /mydir
RUN apt-get update && apt-get install -y wget && apt-get install -y curl 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
COPY package*.json ./
RUN npm install
COPY . .
COPY logs.txt .
EXPOSE 8000
ENV FRONT_URL=http://localhost:5000
CMD npm start
